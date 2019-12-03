# flatbuf_rh6.10
Binary of FlatBuffers 1.11.0 for CentOS/RedHat v6.10
## Building on MacOSX
* ```wget https://github.com/google/flatbuffers/archive/v1.11.0.tar.gz```
* ```tar xzf v1.11.0.tar.gz```
* ```cd flatbuffers-1.11.0```
* ```cmake -G "Unix Makefiles"```
* ```make```
The resulting file ```flatc``` is in the source directory

### Work based on resources (attempt to build on linux WIP):
* Using Docker centos:9.10 image with source code of FlatBuffers 1.11.0 https://github.com/google/flatbuffers/archive/v1.11.0.tar.gz
* Install CLang: https://www.vultr.com/docs/how-to-install-llvm-and-clang-on-centos-6
*  ```yum install cmake gcc```
* Upgrade gcc to 9.2.0 (using 5.1.0 as intermediate compilable version) https://www.vultr.com/docs/how-to-install-gcc-on-centos-6
* ....
