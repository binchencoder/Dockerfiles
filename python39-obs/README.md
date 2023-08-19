# python3.9



## 构建需要的镜像

```shell
docker build -t python3.9-obs -f Dockerfile.obs .
```

## 构建测试镜像

```shell
docker build -t python3.9-test -f Dockerfile.test .
```

### 测试

```shell
docker run --rm -it -p 9999:9999 python3.9-test /bin/bash
```

