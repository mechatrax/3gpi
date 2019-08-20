# 3gpi2-buster-lite-20190808
Raspbian Buster Lite July 2019 を元に変更を加えています。

## イメージファイル  
イメージファイルは次のリンクからダウンロードできます。  
[3gpi2-buster-lite-20190820.zip](https://mechatrax.com/data/3gpi/3gpi2-buster-lite-20190820.zip)  

イメージファイルのハッシュは次のとおりです。

| アルゴリズム | ハッシュ |
| :-- | :-- |
| SHA256 | be612ddf7f50caa35b72215509df35972216c1a8e4e9b3e0961be6582fcc0987 |
| SHA1 | 310ad5aaf5e79a4a4dbbc91afa49b76bcbae0de4 |
| MD5 | 074365e14d3034a0d6f74f3ec5cdfb64 |

## 変更点  
  * 3GPi 用パッケージをインストール
  * 3G ネットワークの管理に NetworkManager を使用
  * ファイアウォールに ufw を使用（デフォルトは許可、wwan0 と ppp0 のみ受信拒否）
  * シリアルコンソールを有効化
  * rootfs で ext4 の ⁠metadata_csum と 64bit オプションを有効化
  * ハードウェアウォッチドッグタイマの監視に systemd を使用
  * APT::Periodic の無効化
  * Raspbian のパッケージを 20190820 時点の最新版に更新

## インストールパッケージ
  * Raspbian パッケージ  
    jo  
    jq  
    gpsd
    gpsd-clients
    modemmanager  
    network-manager  
    ufw

  * 独自パッケージ  
    3gpi-utils  
    3gpi-network-manager  
    4gpi-net-mods  
    mechatrax-archive-keyring  
    soracom-cli  

## 削除パッケージ  
  * 不要なライブラリ等を削除  
    gcc-4.9-base  
    gcc-5-base  
    gcc-6-base  
    gcc-7-base  
    libboost-iostreams1.58.0  
    libudev0  
    libsigc++-1.2-5c2

  * 容量削減のため削除  
    freetype2-doc  
    libraspberrypi-doc

