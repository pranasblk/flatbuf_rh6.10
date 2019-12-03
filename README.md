# flatbuf_rh6.10
Binary of FlatBuffers 1.11.0 for CentOS/RedHat v6.10
## Building on MacOSX
* ```wget https://github.com/google/flatbuffers/archive/v1.11.0.tar.gz```
* ```tar xzf v1.11.0.tar.gz```
* ```cd flatbuffers-1.11.0```
* ```cmake -G "Unix Makefiles"```
* ```make```
The resulting file ```flatc``` is in the source directory
```
$ uname -a
Darwin xxx.local 18.7.0 Darwin Kernel Version 18.7.0: Sat Oct 12 00:02:19 PDT 2019; root:xnu-4903.278.12~1/RELEASE_X86_64 x86_6
```
Stored on ```flatc_darwin-18.7.0.zip```

### Work based on resources (attempt to build on linux WIP):
* Using Docker centos:9.10 image with source code of FlatBuffers 1.11.0 (use host's volume directory for building)
* Original source files from: https://github.com/google/flatbuffers/archive/v1.11.0.tar.gz
*  ```yum install cmake gcc wget```
* Upgrade gcc to 5.1.0 https://www.vultr.com/docs/how-to-install-gcc-on-centos-6
* Install CLang: https://www.vultr.com/docs/how-to-install-llvm-and-clang-on-centos-6
* ....
