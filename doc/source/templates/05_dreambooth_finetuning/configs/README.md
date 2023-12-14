# Build docker image

Build at the parent folder:

```
╭─   ~/src/jinzishuai/ray/doc/source/templates/05_dreambooth_finetuning   master ·········································································  12:57:57
╰─❯ docker build -t ray-train-dreambooth  -f configs/Dockerfile .
```

It is then pushed to [jinzishuai/ray-train-dreambooth](https://hub.docker.com/repository/docker/jinzishuai/ray-train-dreambooth/general)


## Run shell in the container

```
╭─   ~/src/jinzishuai/ray/doc/source/templates/05_dreambooth_finetuning   master ···································································  24s  17:10:30
╰─❯ docker run -it ray-train-dreambooth /bin/bash
WARNING: The requested image's platform (linux/amd64) does not match the detected host platform (linux/arm64/v8) and no specific platform was requested

==========
== CUDA ==
==========

CUDA Version 11.8.0

Container image Copyright (c) 2016-2023, NVIDIA CORPORATION & AFFILIATES. All rights reserved.

This container image and its contents are governed by the NVIDIA Deep Learning Container License.
By pulling and using the container, you accept the terms and conditions of this license:
https://developer.nvidia.com/ngc/nvidia-deep-learning-container-license

A copy of this license is made available in this container at /NGC-DL-CONTAINER-LICENSE for your convenience.

WARNING: The NVIDIA Driver was not detected.  GPU functionality will not be available.
   Use the NVIDIA Container Toolkit to start this container with GPU support; see
   https://docs.nvidia.com/datacenter/cloud-native/ .

(base) ray@75e55c0a70bc:~$ whoami
ray
(base) ray@75e55c0a70bc:~$ sudo whoami
root
(base) ray@75e55c0a70bc:~$ cat /etc/os-release 
NAME="Ubuntu"
VERSION="20.04.6 LTS (Focal Fossa)"
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 20.04.6 LTS"
VERSION_ID="20.04"
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
VERSION_CODENAME=focal
UBUNTU_CODENAME=focal
(base) ray@75e55c0a70bc:~$ conda env list
# conda environments:
#
base                  *  /home/ray/anaconda3

(base) ray@75e55c0a70bc:~$ which python
/home/ray/anaconda3/bin/python
(base) ray@75e55c0a70bc:~$ 
```
