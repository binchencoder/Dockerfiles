# python3.9

## 构建需要的镜像

```shell
docker build -t python-obs:3.9 -f Dockerfile.obs .
```

## 构建测试镜像

```shell
docker build -t python-test:3.9 -f Dockerfile.test .
```

### 测试

```shell
docker run --rm -it -p 9999:9999 python-test:3.9 /bin/bash
```

