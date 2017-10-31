前提条件の確認
===============

各種コマンドを使って前提となる環境がセットアップされているか確認します。
インストール先のマシンにssh等でログインして以下の操作を行なってください。

ディストリビューションの確認
  redhat-releaseファイルの内容を表示し、CentOS 6.4であることを確認します::

    $ cat /etc/redhat-release
    CentOS release 6.4 (Final)

インストールパッケージの確認
  rpmコマンドを利用して、各インストールパッケージのバージョンを確認します::

    $ rpm -q gcc make openssl-devel bzip2-devel expat-devel db4-devel sqlite-devel ncurses-devel readline-devel gdbm-devel tk-devel
    gcc-4.4.7-3.el6.x86_64
    make-3.81-20.el6.x86_64
    openssl-devel-1.0.0-27.el6_4.2.x86_64
    bzip2-devel-1.0.5-7.el6_0.x86_64
    expat-devel-2.0.1-11.el6_2.x86_64
    db4-devel-4.7.25-17.el6.x86_64
    sqlite-devel-3.6.20-1.el6.x86_64
    ncurses-devel-5.7-3.20090208.el6.x86_64
    readline-devel-6.0-4.el6.x86_64
    gdbm-devel-1.8.0-36.el6.x86_64
    tk-devel-8.5.7-5.el6.x86_64

sudo権限の確認
  sudoを実行し、root権限を獲得できるか確認します::

    $ sudo cat /etc/redhat-release
    [sudo] password for tkomiya:
    CentOS release 6.3 (Final)

  sudoが設定されていない場合は、次のようなエラーとなります::

    $ sudo cat /etc/redhat-release
    [sudo] password for tkomiya:
    tkomiya is not in the sudoers file.  This incident will be reported.
