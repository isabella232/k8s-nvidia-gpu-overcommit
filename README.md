# nvidia-gpu-device-plugin with GPU overcommitmemt

This repository is a fork of the nvidia-gpu-device-plugin in Google Kubernetes Engine. This fork allows overcommitment of GPU resources, meant so multiple pods can share 1 GPU by reporting more actual available GPUs to Kubernetes.
This can be set by setting `-overcommit-multiply-by=2` or a higher number, this specifies how many times 1 GPU will be reported.

More details on the nvidia-gpu-device-plugin are [here](cmd/nvidia_gpu/README.md).
