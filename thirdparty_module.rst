サードパーティのモジュール
==========================

標準モジュール意外にも、サードパーティ製のモジュールがたくさんあります。

サードパーティ製のモジュールを探す
----------------------------------

サードパーティ製モジュールの探し方ですが、おおむね次のような方法になります。

* Google検索などの検索エンジンでWeb検索
* `PyPI(Python Package Index) <http://pypi.python.org/pypi>`_ から探す
* `Github <https://github.com/>`_ から探す
* `Google Project Hosting <http://code.google.com/hosting/>`_ から探す

distributeのインストール
------------------------

サードパーティ製のモジュールのインストール方法は、モジュールによって異なる場合もありますが、ほとんどの場合 **easy_install** コマンドでインストールできます。

`distribute <http://pypi.python.org/pypi/distribute>`_ をインストールすることで、easy_installコマンドが使えるようになります。

distributeのインストールはWebインストール用のスクリプトを使うと簡単です。

`http://python-distribute.org/distribute_setup.py`_

PythonでWebインストール用のスクリプトを実行すると、インストールされます。MacOSXやUbuntuの場合はsudoでPythonを実行する必要があります。

::

   > python http://python-distribute.org/distribute_setup.py

distributeをインストールしたら、easy_installコマンドが使えるか試してみましょう。

::

   > easy_install

easy_installコマンドはパッケージ名を指定した場合、PyPIから該当パッケージのダウンロードとインストールを行ってくれます。

例えば、 ``tweepy`` という名前のパッケージをインストールする場合はこうなります。

::

   > easy_install tweepy
