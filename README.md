# dotfiles

## 基本的な使い方
- GitHubにてdotfilesという名前のリポジトリを作成する(とりあえず、READMEだけでも作る)
- 自分のPCにdotfilesのリポジトリを git cloneしてくる(ここでは$HOME/dotfilesに置いたと想定する)
- とりあえず、使っているシェルの設定(~/.bashrc)をdotfiles以下にコピーする
- 元の~/.bashrcを退避させる mkdir backup && mv ~/.bashrc backup
- dotfilesの.bashrcにシンボリックリンクを貼る ln -s ~/dotfiles/.bashrc ~
- あとはdotfiles以下でコミットしてpushしたら出来上がり :tada:
- 同じように管理したいものdotfilesディレクトリにコピーしてシンボリックリンクを貼っていく
- gitconfig_sharedは`.gitconfig`に[include]以下でpathを追加する
```
[include]
        path = ~/.gitconfig_shared
```

## install via install.sh
```
./bin/install.sh
```

## 参考
- https://qiita.com/yutakatay/items/c6c7584d9795799ee164
- https://qiita.com/knt45/items/51b8a8645f36fb0a6d01
