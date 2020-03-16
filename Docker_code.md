# Website for the image container for Ali CLoud

https://cr.console.aliyun.com/

### Docker login
```
sudo docker login --username=d.ai94.sh@gmail.com registry-intl.cn-shenzhen.aliyuncs.com
```
First type in the computer admin pw, then the docker container pw

### Build docker image
```
docker build -t registry.cn-shenzhen.aliyuncs.com/tc_comp/tc_comp_submit:1.0 .
```

### 构建完成后可先验证是否正常运行，正常运行后再进行推送。
CPU image：`docker run your_image sh run.sh`

GPU image：`nvidia-docker run your_image sh run.sh`

推送到镜像仓库 docker push registry.cn-shenzhen.aliyuncs.com/test_for_tianchi/test_for_tianchi_submit:1.0
