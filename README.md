# pyenv-poetry
Macでpyenv+poetryで環境構築したので共有します。
1. ターミナルを起動し、ターミナル上で下記を実行
2. Homebrewをインストール`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
3. pyenvをインストール`brew install pyenv`
4. Pathの設定`export PYENV_ROOT="$HOME/.pyenv"`
5. `export PATH="$PYENV_ROOT/bin:$PATH"`
6. `eval "$(pyenv init --path)"`
7. `eval "$(pyenv init -)"`
8. Pathの設定ファイルを再読み込み`source ~/.bash_profile`
9. pyenvでインストールしたいバージョンを確認`pyenv install --list`
10. 今回は3.10をインストールする`pyenv install 3.10.0`
11. グローバルのバージョンを変更する`pyenv global 3.10.0`
12. ローカルのバージョンを変更する`pyenv local 3.10.0`
13. バージョンの変更が適用されているか確認する`python --version`
14. `git clone https://github.com/iamtatsuki05/pyenv-poetry.git`でディレクトリをインストール
15. `cd`コマンドでディレクトリに移動する
16. poetryをインストールする`poetry install`
17. poetryにライブラリーなどを追加したい場合`poetry add ライブラリー名`
