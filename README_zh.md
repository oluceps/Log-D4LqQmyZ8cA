

+ test env：
```console
$ cat /etc/os-release
PRETTY_NAME="Ubuntu Lunar Lobster (development branch)"
NAME="Ubuntu"
VERSION_ID="23.04"
VERSION="23.04 (Lunar Lobster)"
VERSION_CODENAME=lunar
ID=ubuntu
ID_LIKE=debian
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
UBUNTU_CODENAME=lunar
LOGO=ubuntu-logo
```

+ gcc version

```console
$ gcc --version
gcc (Ubuntu 12.2.0-14ubuntu2) 12.2.0
```

+ clang version
```console
$ clang --version
Ubuntu clang version 15.0.7
Target: x86_64-pc-linux-gnu
Thread model: posix
InstalledDir: /usr/bin
```


eunomia-bpf                           
rev: 044c17573ac6101d28dfb102143cc1a4115e01ed

wasm-bpf （wasm-runtime)      
rev: 2b9b93bb8cf8affadc281082e91a2c1960290236

---

预先在开启 GEN BTF DEBUG INFO 生成可用内核BTF信息的内核上进行测试，确认全部通过；
```console
$ uname -r
6.1.0-16-generic
```


关闭GEN BTF DEBUG INFO 内核编译选项重新编译并安装内核，确认不携带BTF信息，继续测试：
```console
$ uname -r
6.1.0
```

clone `eunomia-bpf`仓库，并同步更新远程子模块

```console
git clone https://github.com/eunomia-bpf/eunomia-bpf.git
cd eunomia-bpf
git submodule update --init --recursive --remote
```




进入 `examples/test` 目录，执行测试
```console
$ make test --keep-going

```

在不使用外源btf信息的情况下，正常编译通过 ecc 和 ecli
examples 编译无报错，但都无法正常运行
[log](./log.md)