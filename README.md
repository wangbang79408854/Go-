
# 安装国内镜像,开启moudle11支持
```
go env -w GO111MODULE=on
go env -w GOPROXY=https://goproxy.io,direct
```



使用go get安装好 需要的安装包后，例如gin，下载好对应的版本，
项目中引用失败，报 cannot find module providing package github.com/gin-gonic/gin: working directory is not part of a module


需要使用 moudle管理   go mod init  
添加 require "github.com/gin-gonic/gin" v1.5.0 即可正常使用

