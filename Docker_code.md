# Website for the image container for Ali Cloud

https://cr.console.aliyun.com/

### Docker login
```
sudo docker login --username=d.ai94.sh@gmail.com registry-intl.cn-shenzhen.aliyuncs.com
```
First type in the computer admin pw, then the docker container pw

### Build docker image
Navigate to the folder where you have the Dockerfile on your local computer and then run the code in the terminal
```
docker build -t registry-intl.cn-shenzhen.aliyuncs.com/tc_comp/tc_comp_submit:1.0 .
```

### After finish building the image, run locally before pushing to the container
CPU image：`docker run [your_image_id] sh run.sh`

GPU image：`nvidia-docker run [your_image_id] sh run.sh`

### Push to the container
```
docker push registry-intl.cn-shenzhen.aliyuncs.com/tc_comp/tc_comp_submit:1.0
```
