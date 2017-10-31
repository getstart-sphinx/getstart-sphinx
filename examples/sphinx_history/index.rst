============
Sphinxの歴史
============

.. _beginning:

はじまり
===========

Sphinxは Georg Brandl というPythonのリリースマネージャーによって2007年
の前半に開発がスタートしました。当時のPythonドキュメントはLaTeXで書かれ
ていました。しかし、LaTeXは難解で、ドキュメントを自分から更新したいと言
い出すユーザが少なかったようです。

そのため、当時一部で使われていた **reStructuredText** とその実装の
**docutils** を使ってコードを書きはじめたのです。

Sphinxという名前について
============================

Sphinxという名前はpython.orgのwebサイトで使用している「pyramid」システ
ムに関連した名前、ということで付けられたようです。当時すでにCMU Sphinx
やSphinx searchがありましたが、Georgは知らなかったようです。

.. _sphinx-logo:

.. figure:: images/sphinx-logo.jpg

   Sphinxのロゴ

   ホルスの目と呼ばれる古代エジプトのシンボルをモチーフとしています

reStructuredText
=======================

:ref:`beginning` で書いたように、Georgは reStructuredText を選択しまし
た。その理由は以下の通りです。

- 軽量なマークアップ言語(シンプルで、読むのに「邪魔」になる文字がない)
- 簡単に拡張できる (codeでも記法でも)
- Python実装がある
- Pythonと強い結びつきがある (reSTはいくつかのPEPでマークアップ言語とし
  て指定されている)
