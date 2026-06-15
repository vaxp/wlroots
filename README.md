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
    libxcb-res0-dev \



meson setup build --prefix=/usr --buildtype=release
meson compile -C build
sudo meson install -C build# wlroots
