# luci-app-rtp2httpd

[![GitHub Release](https://badgen.net/github/release/xuanranran/openwrt-rtp2httpd/stable)](https://github.com/xuanranran/openwrt-rtp2httpd/releases)

🎥 Convert RTP/UDP/RTSP streams into HTTP streams with FCC support for OpenWrt.

## How to build

- Enter in your openwrt dir

- Openwrt official SnapShots or ImmortalWrt

  *1. get luci-app-rtp2httpd code & building*
  ```shell
  git clone https://github.com/xuanranran/openwrt-rtp2httpd package/rtp2httpd
  make menuconfig # choose LUCI -> Applications -> luci-app-rtp2httpd
  make package/rtp2httpd/luci-app-rtp2httpd/compile V=s # build luci-app-rtp2httpd
  ```

--------------

## How to install prebuilt packages (LuCI2)

- Login OpenWrt terminal (SSH)

- Install `curl` package
  ```shell
  # for opkg package manager (openwrt 21.02 ~ 24.10)
  opkg update
  opkg install curl
  
  # for apk package manager
  apk update
  apk add curl
  ```

- Execute install script (Multi-architecture support)
  ```shell
  sh -c "$(curl -ksS https://raw.githubusercontent.com/xuanranran/openwrt-rtp2httpd/master/install.sh)"
  ```

  install via ghproxy:
  ```shell
  sh -c "$(curl -ksS https://ghproxy.net/https://raw.githubusercontent.com/xuanranran/openwrt-rtp2httpd/master/install.sh)" _ gh_proxy="https://ghproxy.net/"
  ```

--------------
