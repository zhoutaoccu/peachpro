# Key Point Changes (Base on Win11 Docker Desktop)
- 更新为国内的sources.list，解决无法安装软件
- 无法访问github的Paket 5.257.0,用离线下载文件替换代替，暂未找到github无法访问的原因和解决方法

# peach pro

Dockerfile for [peach pro](https://gitlab.com/gitlab-org/security-products/protocol-fuzzer-ce)
with everything set up as needed plus some extras.


## Why

The newly released peach pro source code does not compile on any Linux variant,
@Goldstar611 on Gitlab/Github created a shell script that makes it build on Debian Stretch
with quite some effort.
Hence I created a Dockerfile based on it that also generates documenation.

This container has quite a few extra tools for when using `--entrypoint /bin/bash`
that are likely only useful for me :)
