# Libxml2
Download [libxml2](https://gitlab.gnome.org/GNOME/libxml2/-/releases) :

1. Copy the downloaded libxml2 tar into the folder __/data/data/ru.iiec.pydroid3/app_HOME/__
2. Unpack libxml2 with 
   ```sh
   tar xvf lib*
   ```
3. Go to the libxml2 directory with 
   ```sh 
   cd lib*
   ```
4. execute commands in libxml2 
   ```sh
    ./configure --prefix=/data/data/ru.iiec.pydroid3/files/arm-linux-androideabi --with-pic --enable-shared --with-history --without-zlib --without-lzma PYTHON=/data/data/ru.iiec.pydroid3/files/arm-linux-androideabi/bin/python && make all -j80 && make -j80 install
    ```
5. Try executing the command line `xmllint` directly, If it fails, please repeat the build.

# libxslt 
Download [libxslt](https://download.gnome.org/sources/libxslt/1.1):
do the same thing as steps 1 and 4 in the libxml2 point above, to install libxslt do the commandline below:
1. Unpack and enter the libxslt folder
    ```sh
    cd libxslt*
    ```
  
2. Use Installation
   ```sh
    ./configure --prefix=$(pwd)/out --enable-shared PYTHON=/data/data/ru.iiec.pydroid3/files/arm-linux-androideabi/bin/python && make all -j80 && make -j80 install
    ```
3. Copy the build results in the out folder
   ```sh
   cp out/* /data/data/ru.iiec.pydroid3/files/arm-linux-androideabi
   ```

Video Doc: https://youtu.be/3_CAb_vPTJQ
