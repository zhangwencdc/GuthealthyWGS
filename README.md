# GuthealthyWGS
A pipeline for evaluating the human health status associated with the microbiome and DRM pattern in the faecal samples
 GuthealthyWGS version2.0
 2021-9-14
 author：Wen Zhang, zhangwen@icdc.cn

## 1、Docker download

docker pull docker.io/zhangwen2001/guthealthywgs:v2

## 2、Install
GuthealthyWGS version 2.0 only work in Linux system with Docker version 1.7.1 or better.
docker load < guthealthy.tar
docker images

## 3、Run
docker run -it -v workdir:/test --privileged=true guthealthywgs:v2
"workdir "is the local workdir for input file
cd /test
perl /bioapp/GuthealthyWGS.pl -fq1 /test/input.fq 

All results will be shown in wordir/Reprot.txt 
