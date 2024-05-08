# prost_scratch_env
Scratchで新たなブロック作成等を行えるリポジトリです。（主にプロスタ用）
これはJavascriptを使用して、scratchからrosに通信を行うためのブロックを作成することができます。

# How to Use
dockerでの開発をおすすめします。
これは[Docker Hub](https://hub.docker.com/)に移動し、SOBITSのアカウントでログインします。
Scratch npmというDocker imageをpullして使用してください。
※現状これ以外の環境だと、途中でエラーが出ます。（今後改善予定）

以下の３つのリポジトリをクローンして、npmをインストールし、guiにリンクしてください。[choi laboratory](https://github.com/Choi-Laboratory)にあります。
```
git clone https://github.com/Choi-Laboratory/scratch-vm.git
cd scratch-vm
npm install
sudo npm link
```
```
git clone https://github.com/Choi-Laboratory/scratch-blocks.git
npm install 
sudo npm link
```
```
git clone https://github.com/Choi-Laboratory/scratch-gui.git
cd scratch-gui
npm install
npm link scratch-vm scratch-blocks
npm start
```
ここで以下のようになれば、問題ありません。
