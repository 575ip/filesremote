From original repo https://github.com/allanrbo/filesremote

FOR VOID LINUX MUSL

sudo xbps-install -S wxWidgets-devel libssh-devel base-devel cmake git

git clone https://github.com/575ip/filesremote

cd filesremote

mkdir build && cd build

cmake .. -DwxWidgets_CONFIG_EXECUTABLE=/usr/bin/wx-config

make -j$(nproc)

sudo make install
