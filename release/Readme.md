# リリースノート  
ここでは、3GPI付属のSDカードにインストールされているOSイメージのリリースノートを公開しています。  

OSイメージは下記のリンク先からダウンロードできます。  
http://mechatrax.com/data/3gpi/  


# 3gpi-20151204

2015/12/4以降に出荷された量産版のSDカードのイメージです。  
2015-09-24-raspbian-jessie を元に変更を加えています。  

## 更新内容  
  3gpi-20150209 からは以下の項目が更新されています。  
  * 3gpi-utils を v0.3-1 から v0.4-1 に更新  
  * 3gpi-network-manager を v0.1-3 から v0.2-1 に更新  
  * 3gpi-archive-keyring を 20150114 から 20150114.1 に更新  
  * ruby-soracom を追加
  * sleepi-archive-keyring を追加  
  * その他のパッケージは 20151204 時点の最新版に更新  
  * ホームディレクトリの python_games と Documents を削除  
  * アンインストール済み GUI パッケージのメニューを不可視化  

詳細は、[3gpi-20150209.md](./3gpi-20151204.md)を参照してください。


# 3gpi-20150209

2015/2/9以降に出荷された量産版のSDカードのイメージです。  
2015-01-31-raspbian を元に wheezy(stable) から jessie(testing) に upgrade しています。  

## 更新内容
  3gpi-20141118 からは以下の項目が更新されています。  
  * 起動カーネルを raspbian から raspberry pi オリジナルに変更  
  * キーマップを jp106 に変更  
  * タイムゾーンを JST に変更  
  * 3gpi-utils を v0.2-1 から v0.3-1 に更新  
  * 3gpi-network-manager を v0.1-2 から v0.1-3 に更新  
  * 3gpi-archive-keyring を追加
  * その他のパッケージは 20150209 時点の最新版に更新  

詳細は、[3gpi-20150209.md](./3gpi-20150209.md)を参照してください。


# 3gpi-20141118

初期量産版のSDカードのイメージです。  
2014-09-09-wheezy-raspbian を元に wheezy(stable) から jessie(testing) に upgrade しています。  

## 更新内容
  3gpi-20140912 からは以下の項目が更新されています。  
  * 起動時のデフォルトターゲットを graphical.target から multi-user.target に変更  
  * 3gpi-utils を v0.1-1 から v0.2-1 に更新  
  * 3gpi-network-manager を v0.1-1 から v0.1-2 に更新  
  * その他のパッケージは 20141118 時点の最新版に更新  

詳細は、[3gpi-20141118.md](./3gpi-20141118.md)を参照してください。


# 3gpi-20140912

先行出荷版のSDカードのイメージです。  
2014-06-20-wheezy-raspbian を元に wheezy(stable) から jessie(testing) に upgrade しています。  

## 変更点
  * ブート時のカーネルを raspberry pi オリジナルから raspbian の linux-image-rpi に変更  
  * 死活監視に watchdog を導入  
  * ネットワークの管理に NetworkManager を導入  
  * 3GPI 用独自パッケージ (3gpi-utils, 3gpi-network-manager) を導入  
  * その他のパッケージは 20140912 時点の最新版に更新  

詳細は、[3gpi-20140912.md](./3gpi-20140912.md)を参照してください。

