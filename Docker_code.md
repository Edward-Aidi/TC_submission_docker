# Website for the image container for Ali CLoud
https://cr.console.aliyun.com/

```
docker build -t registry.cn-shenzhen.aliyuncs.com/tc_comp/tc_comp_submit:1.0 .
```

CPU镜像：`docker run your_image sh run.sh`
GPU镜像：`nvidia-docker run your_image sh run.sh`
