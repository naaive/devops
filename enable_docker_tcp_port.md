```shell
mkdir -p /etc/docker &\
echo '{
  "registry-mirrors": [
    "https://7t1lqjog.mirror.aliyuncs.com"
  ],
  "hosts": [
    "tcp://0.0.0.0:2375",
    "unix:///var/run/docker.sock"
  ]
}'>/etc/docker/daemon.json & \
mkdir -p "/etc/systemd/system/docker.service.d/"  & \
echo '[Service]
        ExecStart=
        ExecStart=/usr/bin/dockerd'>/etc/systemd/system/docker.service.d/override.conf &\
        systemctl daemon-reload & \
        systemctl restart docker.service
```