<h1 align="center">Mac簡易セットアップ</h1>
<p align="center"><img src="./docs/pc.png" alt="Systems"></p>

# 概要
開発用Macのプレイブックです。  
Ansibleに詳しくない方でもパッケージの選択が出来るよう単一ファイルにしています。

## 利用手順
### OSのアップデート
OS本体のアップデートをして下さい。

### Homebrew / Ansible のインストール
```.shell script
# Install homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"

# Install ansible
brew install ansible
``` 

### Ansibleの実行
Playbookの内容は適宜カスタマイズして下さい
```.shell script
ansible-playbook playbook.yml -i inventory
``` 

### Homebrew未対応パッケージの追加インストール
- [Zoom](https://zoom.us/)
- [prezto](https://github.com/sorin-ionescu/prezto)
- [GVM](https://github.com/moovweb/gvm)
- [NVM](https://github.com/nvm-sh/nvm)
- Xcode  

### 再起動
OSを再起動して完了です。  
お疲れさまでした。
