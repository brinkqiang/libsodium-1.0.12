# libsodium-1.0.12
libsodium-1.0.12

## Get the latest source code

To get the latest source code, you should also update the submodules as following:

```bash
yum -y install git
yum -y install gcc autoconf libtool automake make

git clone https://github.com/brinkqiang/libsodium-1.0.12.git
pushd libsodium-1.0.12
git submodule update --init --recursive

sh autogen.sh
sh configure --prefix=/tmp --disable-dependency-tracking --disable-shared
make
make install
popd
```
