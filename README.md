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

### CentOS 6.10 with linux kernel v3+:
* Using Docker centos:latest image with source code of FlatBuffers https://github.com/google/flatbuffers/commit/99d11e279f290c0ad0e835b7c257dbc84a2161c9 (use host's volume directory for building)
<Docker> Enable CentOS PowerTools 
* TODOS: https://handbrake.fr/docs/en/latest/developer/install-dependencies-centos.html
* Enable option ```FLATBUFFERS_STATIC_FLATC ON``` in CMakeLists.txt
* Install static libraries ```dnf cmake install -y glibc-static llvm libstdc++-static```
* ```cmake .; make```
  
Stored on ```flatc-linux-static.zip``` (Statically linked for x64 platforms only works with 3+ linux kernel)

### CentOS 6.10 with linux kernel v2.6.32:
* https://www.vultr.com/docs/how-to-install-llvm-and-clang-on-centos-6 (Install clang)


