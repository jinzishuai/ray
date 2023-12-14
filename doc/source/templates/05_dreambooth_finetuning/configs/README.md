# Build docker image

Build at the parent folder:

```
╭─   ~/src/jinzishuai/ray/doc/source/templates/05_dreambooth_finetuning   master ·········································································  12:57:57
╰─❯ docker build -t ray-train-dreambooth  -f configs/Dockerfile .
```

It is then pushed to [jinzishuai/ray-train-dreambooth](https://hub.docker.com/repository/docker/jinzishuai/ray-train-dreambooth/general)
