## 镜像同步

```shell
# multi-arch 镜像同步
工具：quay.io/skopeo/stable:latest
# 下载镜像
skopeo copy dir:img docker://build-harbor.alauda.cn/solutions/dicastal/middle-server:v0.0.0-default.3.ga6857a6b-v1.0.1 --dest-creds {user}:{password} --src-tls-verify=false
# 上传镜像
skopeo copy dir:img docker://build-harbor.alauda.cn/solutions/dicastal/middle-server:v0.0.0-default.3.ga6857a6b-v1.0.1 --dest-creds {user}:{password} --src-tls-verify=false
```