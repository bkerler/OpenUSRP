# FakeUSRP

FakeUSRP can using LimeSDR to simulate USRP B210 Device

Dependencies
------------
LimeSuite: [https://github.com/myriadrf/LimeSuite.git][1]
Boost: [http://www.boost.org/users/download/][2]

Installation
----------

LIBUHD mode

```sh
git clone https://github.com/EttusResearch/uhd.git
cd uhd/host/lib/usrp
git clone https://github.com/jocover/FakeUSRP.git
```
add line INCLUDE_SUBDIRECTORY(FakeUSRP) to uhd/host/lib/usrp/CMakeLists.txt file
```sh
echo "INCLUDE_SUBDIRECTORY(FakeUSRP)">>CMakeLists.txt

```
Rebuild UHD driver
[Building and Installing UHD from source][3]

----------
UHD MODULE mode
```sh
git clone https://github.com/jocover/FakeUSRP.git
mkdir build && cd build
cmake ..
make -j4
make install
```

Windows Binarie
---------
x86 version:[FakeUSRP_x86.zip][4]

x64 version:[FakeUSRP_x64.zip][5]


  [1]: https://github.com/myriadrf/LimeSuite.git
  [2]: http://www.boost.org/users/download/
  [3]: http://files.ettus.com/manual/page_build_guide.html
  [4]: https://www.jiangwei.org/download/fackusrp_x86.zip
  [5]: https://www.jiangwei.org/download/fakeusrp_x64.zip