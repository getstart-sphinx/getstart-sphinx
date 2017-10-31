インストール手順
=================

インストール先のマシンにssh等でログインして以下の操作を行ってください。

1. 最初にPythonのアーカイブをpython.orgからダウンロードします::

     $ mkdir $HOME/src
     $ cd $HOME/src
     $ curl -L -O http://www.python.org/ftp/python/2.7.5/Python-2.7.5.tgz
       % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                   Dload  Upload   Total   Spent    Left  Speed
     100 15.9M  100 15.9M    0     0  4355k      0  0:00:03  0:00:03 --:--:-- 4730k
     $ ls
     Python-2.7.5.tgz

   curlコマンドを実行するとダウンロードが開始されます。
   少し待つとダウンロードが完了し、アーカイブである Python-2.7.5.tgz が保存されています。

2. ダウンロードしたアーカイブを展開し、Pythonをビルドします::

     $ tar xzf Python-2.7.5.tgz
     $ cd Python-2.7.5
     $ ./configure
     $ make

3. インストール先にファイルを配置します::

     $ sudo make install
