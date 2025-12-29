sudo xbps-install -S wxWidgets-devel libssh-devel base-devel cmake git

git clone 
cd filesremote

mkdir build && cd build

cmake .. -DwxWidgets_CONFIG_EXECUTABLE=/usr/bin/wx-config

make -j$(nproc)

sudo make install
