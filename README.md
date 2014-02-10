### Vagrant

```
1) vagrant init centos64
2) edit Vagrantfile # sshで接続出来るように
3) vagrant up
4) vagrant ssh-config --host melody >> ~/.ssh/config # 仮想サーバのホスト名がmelody
```

### Chef

```
1) knife solo prepare melody
2) knife cookbook create iptables -o site-cookbooks # クックブックの作成
3) knife solo cook melody # 実行先のサーバを指定する
```
