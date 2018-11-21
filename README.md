# MtgArenaJaCardViewer

![imgicon](https://raw.githubusercontent.com/WestHillApps/westhillapps.github.io/master/res/mtga-ja-card-viewer-icon.png)  
**Magic: The Gathering Arena（MTGA、MTG Arena、MTG アリーナ）**  
で日本語版のカード画像を表示するツールです。  

**※ご利用は自己責任でお願いします。**  
<br />
![img01](https://raw.githubusercontent.com/WestHillApps/westhillapps.github.io/master/res/mtga-ja-card-viewer-01.gif)  

## ダウンロード
* [**リリースページ**](https://github.com/WestHillApps/MtgArenaJaCardViewer/releases) から最新版の **MtgArenaJaCardViewer_vXXX.zip** を保存してください。  

## 使い方
* 事前に [**Microsoft Visual C++ 2015 再頒布可能パッケージ (x64)**](https://www.microsoft.com/ja-jp/download/details.aspx?id=53840) のインストールが必要です。  

* zipを解凍して **MtgArenaJaCardViewer.exe** を実行すると起動します。  
MTGAを起動してから実行してください。  
カード画像ダウンロードのために通信を行いますので、自己判断で通信許可をしてください。  
MTGAに更新があった場合は、更新後に1度MTGAを終了して再起動してから本ツールを起動してください。  

* 終了するときは、タスクバーから右クリックで終了してください。  

* 画面上でマウスを止めた時に、近くのカード画像を解析して、日本語版のカード画像を表示します。

* スクリーン下部のチェックボックスで機能のON/OFFを切り替えられます。

* スクリーン下部で丸いアイコンが回転している間は、画面の解析中です。  

![img02](https://raw.githubusercontent.com/WestHillApps/westhillapps.github.io/master/res/mtga-ja-card-viewer-02.png)  

* **v0.0.5** 以降はツールに更新がある場合、以下のダイアログが表示されます。  
「はい」を選ぶとリリースページが開くので、最新バージョンをダウンロードしてフォルダ毎置き換えてください。  

![img04](https://raw.githubusercontent.com/WestHillApps/westhillapps.github.io/master/res/mtga-ja-card-viewer-04.png)

## 仕様
* **Windows10 64bit版** 専用です。  
**Windows8.1 64bit版** でも動作するみたいですが、手元に環境がないためサポート外となります。    
 [**Microsoft Visual C++ 2015 再頒布可能パッケージ (x64)**](https://www.microsoft.com/ja-jp/download/details.aspx?id=53840) のインストールが必要です。  
上記を満たしていても、環境やスペックによっては動かないこともあるようです。  

* 日本語版カード画像は初回表示時のみダウンロードされ、以下のフォルダに保存されます。  
**{ユーザーフォルダ}/AppData/LocalLow/WestHillApps/MtgArenaJaCardViewer/CardTextureCache/**  
カード画像のダウンロード中は黒い半透明のカード枠が表示されます。  
カード1枚あたりの容量は **100KB ～ 200KB** くらいです。  

* 以下のカードには対応していません。  
**基本土地カード**  
**スタンダードフォーマット以外のカード**  
**チュートリアル専用カード、MTGA専用カード、未発売のセット等の日本語版が存在しないカード**  
![img03](https://raw.githubusercontent.com/WestHillApps/westhillapps.github.io/master/res/mtga-ja-card-viewer-03.png)  

* カードによっては認識・マッチしない場合があります。  
対戦中にカードを右クリックすると画面左側に拡大画像が表示されるので、そちらだと認識しやすいです。

* 現在のバージョンで認識しにくいカードの一覧は → [**こちら**](https://github.com/WestHillApps/MtgArenaJaCardViewer/blob/master/UnmatchCardMemo.txt)  
コレクション画面でチェックしているため、試合中や他の画面では異なる可能性があります。  

* カード以外の空間を誤認することがあります。  

* **1920x1080**の画面サイズで動作確認しています。  
これより小さい画面では動作しないかもしれません。  
画面サイズは大きいほうが認識しやすいです。

* リアルタイムで画像解析を行っているため、CPU負荷はそれなりにあります。  
ある程度のスペックが無いと厳しいかも…

* 動作を改善していくために [**Unityアナリティクス**](https://unity.com/solutions/analytics) を使用しています。（[**プライバシーポリシー**](https://unity3d.com/legal/privacy-policy)）

* 開発中のため、不具合等色々問題あるかと思いますが、ご容赦ください。

* ツール更新情報等はTwitterアカウントでお知らせします。

## 連絡先
[@westhillapps](https://twitter.com/westhillapps)  

<a href="https://twitter.com/westhillapps">
<img alt="Follow me on Twitter"
src="https://raw.githubusercontent.com/WestHillApps/westhillapps.github.io/master/res/twitter.png" width="75"/>
</a>

## クレジット
以下のライブラリを使用しています。  
[MTG Developers SDK](https://magicthegathering.io/)  
[OpenCV for Unity](https://assetstore.unity.com/packages/tools/integration/opencv-for-unity-21088)  
[uWindowCapture](https://github.com/hecomi/uWindowCapture)  