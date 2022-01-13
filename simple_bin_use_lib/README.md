# simplest-cmake
How to use

step 1. make build folder
```
mkdir build
cd build
```

step 2. configure cmake
```
export PKG_CONFIG_PATH=/opt/install
cmake ../
```

step 3. build
```
make
make install
# or
# make DESTDIR=$PWD install
```
