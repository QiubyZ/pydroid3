# Libxml2
Download [libxml2](https://gitlab.gnome.org/GNOME/libxml2/-/releases) :

1. Copy libxml2 tar yang telah didownload ke dalam folder __/data/data/ru.iiec.pydroid3/app_HOME/__
2. Unpack libxml2 dengan 
   ```sh
   tar xvf lib*
   ```
3. Masuk ke directory libxml2 dengan 
   ```sh 
   cd lib*
   ```
4. eksekusi command didalam libxml2 
   ```sh
    ./configure --prefix=/data/data/ru.iiec.pydroid3/files/arm-linux-androideabi --with-pic --enable-shared --with-history --without-zlib --without-lzma PYTHON=/data/data/ru.iiec.pydroid3/files/arm-linux-androideabi/bin/python && make all -j80 && make -j80 install
    ```
5. Coba eksekusi command line `xmllint` secara langsung, jika gagal, silahkan mengulang buildnya.

# libxslt 
Download [libxslt](https://download.gnome.org/sources/libxslt/1.1):
lakukan hal yang sama seperti langkah 1 dan 4 pada point libxml2 diatas, untuk penginstalan libxslt lakukan commandline dibawah ini:
1. Unpack dan Masuk ke folder libxslt
    ```sh
    cd libxslt*
    ```
  
2. Gunakan Penginstallan
   ```sh
    ./configure --prefix=$(pwd)/out --enable-shared PYTHON=/data/data/ru.iiec.pydroid3/files/arm-linux-androideabi/bin/python && make all -j80 && make -j80 install
    ```
3. Copy hasil build di folder out
   ```sh
   cp out/* /data/data/ru.iiec.pydroid3/files/arm-linux-androideabi
   ```
