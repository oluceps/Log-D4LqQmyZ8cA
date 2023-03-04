```
ls ../bpftools/bashreadline/bashreadline.h && ../../compiler/workspace/bin/ecc ../bpftools/bashreadline/bashreadline.bpf.c ../bpftools/bashreadline/bashreadline.h \
|| ../../compiler/workspace/bin/ecc ../bpftools/bashreadline/bashreadline.bpf.c
../bpftools/bashreadline/bashreadline.h
Compiling bpf object...
Generating export types...
Packing ebpf object and config into ../bpftools/bashreadline/package.json...
sudo timeout --preserve-status -s 2 2 ./ecli run ../bpftools/bashreadline/package.json
arg: ../bpftools/bashreadline/package.json
failed to find vmlinux BTF. please provide btf file with env BTF_FILE_PATH.
Error: BpfError("load and attach ebpf program failed")


make: *** [Makefile:27: bashreadline] Error 1


ls ../bpftools/bootstrap/bootstrap.h && ../../compiler/workspace/bin/ecc ../bpftools/bootstrap/bootstrap.bpf.c ../bpftools/bootstrap/bootstrap.h \
|| ../../compiler/workspace/bin/ecc ../bpftools/bootstrap/bootstrap.bpf.c
../bpftools/bootstrap/bootstrap.h
Compiling bpf object...
Generating export types...
Packing ebpf object and config into ../bpftools/bootstrap/package.json...
sudo timeout --preserve-status -s 2 2 ./ecli run ../bpftools/bootstrap/package.json
arg: ../bpftools/bootstrap/package.json
failed to find vmlinux BTF. please provide btf file with env BTF_FILE_PATH.
Error: BpfError("load and attach ebpf program failed")


make: *** [Makefile:27: bootstrap] Error 1


ls ../bpftools/fentry-link/fentry-link.h && ../../compiler/workspace/bin/ecc ../bpftools/fentry-link/fentry-link.bpf.c ../bpftools/fentry-link/fentry-link.h \
|| ../../compiler/workspace/bin/ecc ../bpftools/fentry-link/fentry-link.bpf.c
ls: cannot access '../bpftools/fentry-link/fentry-link.h': No such file or directory
Compiling bpf object...
Packing ebpf object and config into ../bpftools/fentry-link/package.json...
sudo timeout --preserve-status -s 2 2 ./ecli run ../bpftools/fentry-link/package.json
arg: ../bpftools/fentry-link/package.json
failed to find vmlinux BTF. please provide btf file with env BTF_FILE_PATH.
Error: BpfError("load and attach ebpf program failed")


make: *** [Makefile:27: fentry-link] Error 1


ls ../bpftools/kprobe-link/kprobe-link.h && ../../compiler/workspace/bin/ecc ../bpftools/kprobe-link/kprobe-link.bpf.c ../bpftools/kprobe-link/kprobe-link.h \
|| ../../compiler/workspace/bin/ecc ../bpftools/kprobe-link/kprobe-link.bpf.c
ls: cannot access '../bpftools/kprobe-link/kprobe-link.h': No such file or directory
Compiling bpf object...
Packing ebpf object and config into ../bpftools/kprobe-link/package.json...
sudo timeout --preserve-status -s 2 2 ./ecli run ../bpftools/kprobe-link/package.json
arg: ../bpftools/kprobe-link/package.json
failed to find vmlinux BTF. please provide btf file with env BTF_FILE_PATH.
Error: BpfError("load and attach ebpf program failed")


make: *** [Makefile:27: kprobe-link] Error 1


ls ../bpftools/lsm-connect/lsm-connect.h && ../../compiler/workspace/bin/ecc ../bpftools/lsm-connect/lsm-connect.bpf.c ../bpftools/lsm-connect/lsm-connect.h \
|| ../../compiler/workspace/bin/ecc ../bpftools/lsm-connect/lsm-connect.bpf.c
ls: cannot access '../bpftools/lsm-connect/lsm-connect.h': No such file or directory
Compiling bpf object...
Packing ebpf object and config into ../bpftools/lsm-connect/package.json...
sudo timeout --preserve-status -s 2 2 ./ecli run ../bpftools/lsm-connect/package.json
arg: ../bpftools/lsm-connect/package.json
unknown type: __u32
failed to find vmlinux BTF. please provide btf file with env BTF_FILE_PATH.
Error: BpfError("load and attach ebpf program failed")


make: *** [Makefile:27: lsm-connect] Error 1


ls ../bpftools/mdflush/mdflush.h && ../../compiler/workspace/bin/ecc ../bpftools/mdflush/mdflush.bpf.c ../bpftools/mdflush/mdflush.h \
|| ../../compiler/workspace/bin/ecc ../bpftools/mdflush/mdflush.bpf.c
../bpftools/mdflush/mdflush.h
Compiling bpf object...
error: unknown argument: '-target bpf'
warning: unknown warning option '-Wno-unknown-attributes '; did you mean '-Wno-unknown-attributes'? [-Wunknown-warning-option]
/tmp/eunomia.3g4Abv/include/vmlinux/x86/vmlinux.h:5:46: warning: unknown attribute 'preserve_access_index' ignored [-Wunknown-attributes]
/tmp/eunomia.3g4Abv/include/vmlinux/x86/vmlinux.h:111:9: note: when applied to this declaration
<omitted warnings>
/tmp/eunomia.E55hcn/include/vmlinux/x86/vmlinux.h:128565:1: note: when applied to this declaration
/tmp/eunomia.E55hcn/include/vmlinux/x86/vmlinux.h:5:46: warning: unknown attribute 'preserve_access_index' ignored [-Wunknown-attributes]
/tmp/eunomia.E55hcn/include/vmlinux/x86/vmlinux.h:128595:1: note: when applied to this declaration
/home/user/test-doc/eunomia-bpf/examples/bpftools/runqlat/core_fixes.bpf.h:18:18: warning: unknown attribute 'preserve_access_index' ignored [-Wunknown-attributes]
/home/user/test-doc/eunomia-bpf/examples/bpftools/runqlat/core_fixes.bpf.h:22:18: warning: unknown attribute 'preserve_access_index' ignored [-Wunknown-attributes]
/home/user/test-doc/eunomia-bpf/examples/bpftools/runqlat/core_fixes.bpf.h:28:6: error: use of unknown builtin '__builtin_preserve_field_info' [-Wimplicit-function-declaration]
/home/user/test-doc/eunomia-bpf/examples/bpftools/runqlat/core_fixes.bpf.h:41:18: warning: unknown attribute 'preserve_access_index' ignored [-Wunknown-attributes]
/home/user/test-doc/eunomia-bpf/examples/bpftools/runqlat/core_fixes.bpf.h:45:18: warning: unknown attribute 'preserve_access_index' ignored [-Wunknown-attributes]
/home/user/test-doc/eunomia-bpf/examples/bpftools/runqlat/core_fixes.bpf.h:51:6: error: use of unknown builtin '__builtin_preserve_field_info' [-Wimplicit-function-declaration]
/home/user/test-doc/eunomia-bpf/examples/bpftools/runqlat/core_fixes.bpf.h:69:18: warning: unknown attribute 'preserve_access_index' ignored [-Wunknown-attributes]
/home/user/test-doc/eunomia-bpf/examples/bpftools/runqlat/core_fixes.bpf.h:75:18: warning: unknown attribute 'preserve_access_index' ignored [-Wunknown-attributes]
/home/user/test-doc/eunomia-bpf/examples/bpftools/runqlat/core_fixes.bpf.h:79:6: error: use of unknown builtin '__builtin_preserve_type_info' [-Wimplicit-function-declaration]
/home/user/test-doc/eunomia-bpf/examples/bpftools/runqlat/core_fixes.bpf.h:79:6: warning: indirection of non-volatile null pointer will be deleted, not trap [-Wnull-dereference]
/home/user/test-doc/eunomia-bpf/examples/bpftools/runqlat/core_fixes.bpf.h:79:6: note: consider using __builtin_trap() or qualifying pointer with 'volatile'
/home/user/test-doc/eunomia-bpf/examples/bpftools/runqlat/core_fixes.bpf.h:96:18: warning: unknown attribute 'preserve_access_index' ignored [-Wunknown-attributes]
/home/user/test-doc/eunomia-bpf/examples/bpftools/runqlat/core_fixes.bpf.h:101:18: warning: unknown attribute 'preserve_access_index' ignored [-Wunknown-attributes]
/home/user/test-doc/eunomia-bpf/examples/bpftools/runqlat/core_fixes.bpf.h:107:6: error: use of unknown builtin '__builtin_preserve_field_info' [-Wimplicit-function-declaration]
Generating export types...
Packing ebpf object and config into ../bpftools/runqlat/package.json...
sudo timeout --preserve-status -s 2 2 ./ecli run ../bpftools/runqlat/package.json
arg: ../bpftools/runqlat/package.json
failed to find vmlinux BTF. please provide btf file with env BTF_FILE_PATH.
Error: BpfError("load and attach ebpf program failed")


make: *** [Makefile:27: runqlat] Error 1


ls ../bpftools/sigsnoop/sigsnoop.h && ../../compiler/workspace/bin/ecc ../bpftools/sigsnoop/sigsnoop.bpf.c ../bpftools/sigsnoop/sigsnoop.h \
|| ../../compiler/workspace/bin/ecc ../bpftools/sigsnoop/sigsnoop.bpf.c
../bpftools/sigsnoop/sigsnoop.h
Compiling bpf object...
Generating export types...
Packing ebpf object and config into ../bpftools/sigsnoop/package.json...
sudo timeout --preserve-status -s 2 2 ./ecli run ../bpftools/sigsnoop/package.json
arg: ../bpftools/sigsnoop/package.json
failed to find vmlinux BTF. please provide btf file with env BTF_FILE_PATH.
Error: BpfError("load and attach ebpf program failed")


make: *** [Makefile:27: sigsnoop] Error 1


ls ../bpftools/tc/tc.h && ../../compiler/workspace/bin/ecc ../bpftools/tc/tc.bpf.c ../bpftools/tc/tc.h \
|| ../../compiler/workspace/bin/ecc ../bpftools/tc/tc.bpf.c
ls: cannot access '../bpftools/tc/tc.h': No such file or directory
Compiling bpf object...
Packing ebpf object and config into ../bpftools/tc/package.json...
sudo timeout --preserve-status -s 2 2 ./ecli run ../bpftools/tc/package.json
arg: ../bpftools/tc/package.json
failed to find vmlinux BTF. please provide btf file with env BTF_FILE_PATH.
Error: BpfError("load and attach ebpf program failed")


make: *** [Makefile:27: tc] Error 1


ls ../bpftools/tcpstates/tcpstates.h && ../../compiler/workspace/bin/ecc ../bpftools/tcpstates/tcpstates.bpf.c ../bpftools/tcpstates/tcpstates.h \
|| ../../compiler/workspace/bin/ecc ../bpftools/tcpstates/tcpstates.bpf.c
../bpftools/tcpstates/tcpstates.h
Compiling bpf object...
Generating export types...
Packing ebpf object and config into ../bpftools/tcpstates/package.json...
sudo timeout --preserve-status -s 2 2 ./ecli run ../bpftools/tcpstates/package.json
arg: ../bpftools/tcpstates/package.json
failed to find vmlinux BTF. please provide btf file with env BTF_FILE_PATH.
Error: BpfError("load and attach ebpf program failed")


make: *** [Makefile:27: tcpstates] Error 1


make: Target 'test' not remade because of errors.
```