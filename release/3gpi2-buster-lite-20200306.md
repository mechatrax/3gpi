# 3gpi2-buster-lite-20200306
Raspbian Buster Lite February 2020 を元に変更を加えています。

## イメージファイル  
イメージファイルは次のリンクからダウンロードできます。  
[3gpi2-buster-lite-20200306.zip](https://mechatrax.com/data/3gpi/3gpi2-buster-lite-20200306.zip)  

イメージファイルのハッシュは次のとおりです。

| アルゴリズム | ハッシュ |
| :-- | :-- |
| SHA256 | d1d8639ee9c078cf0fd469f50e1ce67ca77ff50793ea358b499b8a49de9f7106 |
| SHA1 | 471803b2fb99a5835555b15b1f9c7cadc7fbb395 |
| MD5 | a1e06277c5f100882b7015a64841cd0d |

## 変更点  
  * 3GPi 用パッケージをインストール
  * 3G ネットワークの管理に NetworkManager を使用
  * ファイアウォールに ufw を使用（デフォルトは許可、wwan0 と ppp0 のみ受信拒否）
  * シリアルコンソールを有効化
  * rootfs で ext4 の ⁠metadata_csum と 64bit オプションを有効化
  * ハードウェアウォッチドッグタイマの監視に systemd を使用
  * APT::Periodic の無効化
  * avahi-daemon で ppp0 を無視
  * Raspbian のパッケージを 20200306 時点の最新版に更新

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
