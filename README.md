

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

Compile in kernel with option `Generate BTF typeinfo` enabled, and ensure that tests all passed.
```console
$ uname -r
6.1.0-16-generic
```


Disable option `Generate BTF typeinfo` then recompile kernel, ensure there contains no BTF info. Continue tests:
```console
$ uname -r
6.1.0
```


clone repo `eunomia-bpf`, and sync submodules

```console
git clone https://github.com/eunomia-bpf/eunomia-bpf.git
cd eunomia-bpf
git submodule update --init --recursive --remote
```


Enter `examples/tests` , run test
```console
$ make test --keep-going

```


`ecc` and `ecli` compile successfully with no btf info,
`ecc`  compile examples reports no error, but run failed.
[log](./log.md)