# crypro-training-environment
Training environment for algo & ctf (c++, python)

## 概要
WSL2 + Docker + VSCodeの開発環境を構築しました。\
この環境ではVSCodeのRemote Developmentの拡張機能を使用しています。\
これがあれば、WindowsでVSCodeで快適に開発ができます！

## インストール
おおまかに以下の流れで進めていきます。
1. WSL2の有効化
2. VSCodeと拡張機能のインストール
3. Docker for Windowsのインストール
4. Githubのインストール
5. コンテナのクローンとリモート接続

### WSL2の有効化
WSL2とはWindows OS上でLinuxを動かすことができる機能で最新のWindows10,11で利用することができます。\
公式の[インストール方法](https://docs.microsoft.com/ja-jp/windows/wsl/install)に従ってWSL2を導入してください。\
導入するOSについてはお好みでいいですがUbuntuを想定しています。

### VSCodeと拡張機能のインストール
高機能エディタの[VSCode](https://azure.microsoft.com/ja-jp/products/visual-studio-code/)をインストールします。 \
日本語化したい方は「[Japanese Language Pack](https://marketplace.visualstudio.com/items?itemName=MS-CEINTL.vscode-language-pack-ja)」を導入してください。 \
次に、VSCodeからWSL2上のコンテナにリモート接続するための拡張機能を導入します。
- [Remote Development](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack)
  - VSCodeがコンテナやWSL2にリモート接続するために必要な拡張機能

### Docker for Windowsのインストール
続いて[Docker](https://www.docker.com/products/docker-desktop/)をインストールします。 \
インストーラが起動しますがデフォルトの設定で進めて大丈夫です。

### Githubのインストール
続いてバージョン管理ツールのGithubをインストールします。\
WSL2上では通常インストールされてると思いますが、\
念のため`sudo apt install git`とインストールしてください。

### コンテナのクローンとリモート接続
WSL2上で好きなところで`git clone https://github.com/funanox/crypro-training-environment.git`としてください。\
次に`crypro-training-environment`フォルダ以下でVSCodeを起動します。\
そして左下の「><」をクリックして`Reopen in Container`を選択すると接続が完了します。

## その他
初版は競技プログラミングとCTFのCryptoの範囲のソフトしかサポートしていません。\
ですので、「こんなソフトも入れておいてくれると嬉しい」みたいな要望があればご連絡ください。

## ライセンス
ライセンスは特段設けていないので自由にお使いください。
