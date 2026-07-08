```
sudo apt update && sudo apt install -y \
    xwayland \
    liblcms2-dev \
    libxcb-ewmh-dev \
    libxcb-icccm4-dev \
    libxcb-render-util0-dev \
    libxcb-xinput-dev \
    libxcb-composite0-dev \
    libxcb-dri3-dev \
    libxcb-present-dev \
    libxcb-res0-dev 

apt install libexpat1-dev libxml2-dev libegl1-mesa-dev libgles2-mesa-dev libdrm-dev libgbm-dev libinput-dev libxkbcommon-dev libudev-dev libpixman-1-dev libseat-dev libvulkan-dev hwdata libxcb-shm0-dev glslang-tools libcairo2-dev libpango1.0-dev libgdk-pixbuf-2.0-dev



```

```
CFLAGS="-Wno-error" CXXFLAGS="-Wno-error" meson setup build --prefix=/usr --buildtype=release --wrap-mode=default -Dwerror=false

meson compile -C build
sudo meson install -C build
pkg-config --modversion wlroots-0.19

```
