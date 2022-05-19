```
curl -i -X GET \\
    -H "Authorization: Bearer ${FLY\_API\_TOKEN}" -H "Content-Type: application/json" \\
    "http://${FLY\_API\_HOSTNAME}/v1/apps/my-awesome-machine-app/machines" 

```
**Status: 200**
```json
[
  {
    "id": "24d899e0b99879",
    "name": "quirky-machine",
    "state": "started",
    "region": "cdg",
    "instance\_id": "01G3C47GRZQTA5RBF85R3WFJ60",
    "private\_ip": "fdaa:0:3ec2:a7b:5adc:ad42:c773:2",
    "config": {
      "env": null,
      "init": {
        "exec": null,
        "entrypoint": null,
        "cmd": null,
        "tty": false
      },
      "image": "library/nginx:latest",
      "metadata": {
      },
      "restart": {
        "policy": "",
        "max\_retries": 3
      },
      "size": "shared-cpu-1x"
    },
    "image\_ref": {
      "registry": "registry-1.docker.io",
      "repository": "library/nginx",
      "tag": "latest",
      "digest": "sha256:61face6bf030edce7ef6d7dd66fe452298d6f5f7ce032afdd01683ef02b2b841",
      "labels": {
        "maintainer": "NGINX Docker Maintainers <docker-maint@nginx.com>"
      }
    },
    "created\_at": "2022-05-18T17:42:41Z"
  }
]
```