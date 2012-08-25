Pythonプログラミング環境の用意
==============================

自分のPCに合ったPythonプログラミング環境を用意します。今回はPython2.7系を使います。

Pythonのインストール
--------------------

まずはPythonをインストールします。OSによって対応が違うので注意してください。

Windowsの場合
~~~~~~~~~~~~~

python.orgのダウンロードページから、Windows用のインストーラーをダウンロードしてインストールします。

`Download Python <http://www.python.org/download/>`_

インストーラでインストールした後、 ``Path`` という名前の環境変数に、 python.exe の存在するディレクトリと、その階層にあるScriptsディレクトリのパスを追加します。

Mac OS Xの場合
~~~~~~~~~~~~~~

Mac OS X(10.7, 10.8)であれば、Python2.7が最初からインストールされています。

それ以外のバージョンを使っている場合は、python.orgからMac用のインストーラーをダウンロードするか、MacPortsなどでインストールすると良いでしょう。

`Download Python <http://www.python.org/download/>`_

Ubuntuの場合
~~~~~~~~~~~~

Ubuntu12.04, 12.10であれば、最初からPython2.7がインストールされているでしょう。もしインストールされていないならば、aptでpython2.7とpython2.7-devパッケージをインストールしておくと良いでしょう。

開発スタイルについて
--------------------

Pythonをインストールできましたか？

他に必要なものは、最低限だと使い慣れたテキストエディタだけです。

さて、PythonのプログラミングをPythonシェルとテキストエディタのみで行うのも良いですが、開発を補助する様々な機能を詰め込んだ統合開発環境(IDE)というものもあります。他にもリモートで開発するスタイルなどをここでは少し紹介します。

IDEの利用
~~~~~~~~~

PythonをサポートするIDEはいくつかあり、そのほとんどがプロジェクト管理機能や高機能エディタ、デバッガ、統合されたシェルなどを持っています。ここではPyScripter、PyDev、PyCharmを紹介します。

PyScripter
^^^^^^^^^^

PyScripterは、Windowsで動作するオープンソースのPython IDEです。複数のPythonバージョンをサポートしている他、プロジェクト管理、ファイルエクスプローラ、シェル、単体テスト、正規表現テスターなどを備えています。比較的軽量なIDEです。

.. figure:: images/ss_pyscripter.png

   PyScripter

`PyScripter <http://code.google.com/p/pyscripter/>`_

PyDev
^^^^^

PyDevはEclipseのためのオープンソースのPython IDEです。EclipseやAptanaStudioにプラグインとして追加できます。

`PyDev.org <http://pydev.org/>`_

PyCharm
^^^^^^^

PyCharmは、JetBrains社が開発している有償のPython IDEです。IntelliJベースで補完機能やリファクタリング、バージョン管理ツールの統合、virtualenvサポートなどを備えたとても強力なIDEです。

仮想マシン上での開発
~~~~~~~~~~~~~~~~~~~~

Webアプリケーションの開発などで、別のOSを使用したい場合におすすめのスタイルです。

VMwareやVirtualBoxでLinuxなどを動かし、SSHでログインしてVimやEmacsなどのCUIのテキストエディタで開発します。

.. figure:: images/ss_sshvim.png

   仮想マシンで動作しているUbuntuにSSH(PuTTY)でログインしてVimで開発

次は
----

これでPythonのプログラミング環境は用意できました。次はいよいよPythonプログラミングを始めます。
