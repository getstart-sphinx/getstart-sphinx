文書の目的
===========

この手順書ではPython 2.7のインストールを行います。
2013年8月現在、Python 2.7系の最新版は2.7.5です。

この手順書ではCentOS 6.4環境を想定しています。
また以下のパッケージがインストールされているものとします。

.. list-table:: Pythonの想定環境
   :header-rows: 1

   * - ソフトウェア
     - バージョン
   * - gcc
     - 4.4.7-3.el6
   * - make
     - 3.81-20.el6
   * - openssl-devel
     - 1.0.0-27.el6_4.2
   * - bzip2-devel
     - 1.0.5-7.el6_0
   * - expat-devel
     - 2.0.1-11.el6_2
   * - db4-devel
     - 4.7.25-17.el6
   * - sqlite-devel
     - 3.6.20-1.el6
   * - ncurses-devel
     - 5.7-3.20090208.el6
   * - readline-devel
     - 6.0-4.el6
   * - gdbm-devel
     - 1.8.0-36.el6
   * - tk-devel
     - 8.5.7-5.el6

インストール作業中にroot権限を必要とするため、
あらかじめ作業ユーザがsudoできるよう設定しておく必要があります。
