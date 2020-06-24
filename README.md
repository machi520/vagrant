# vagrant
virtual box/vagrantの使い方メモ

# reference
-- vagrant list-commands  コマンド一覧の表示
-- vagrant -h  ヘルプ

# boxの作成から起動・終了・削除まで
-- vagrant box add {name,url or path}  ボックスの追加
-- vagrant init {name}  初期化
-- vagrant up  起動
-- vagrant reload  再起動
-- vagrant halt  終了
-- vagrant box remove {name}  削除

※-hを最後につけると、個別にコマンドのヘルプが詳細表示される

# Vagrantfileの編集
-- httpサーバーを使えるように以下の行の先頭のコメントアウト(#)を消す  config.vm.network "private_network", ip: "192.168.33.10"
-- 仮想マシンとローカルマシンの共有フォルダは以下の行を参照・編集  config.vm.synced_folder