スクリプトファイルとモジュール化
================================

Pythonでは作成したプログラムを再利用するために、ファイルにコードを記述して実行することができます。

ここでは、スクリプトファイルの作成とモジュールについて説明していきます。

スクリプトファイルからの実行
----------------------------

Pythonのスクリプトファイルの拡張子は ``.py`` です。

``hello.py`` という名前のファイルを以下の内容で作成してみます。

.. code-block:: python

   # coding: utf-8
   print("Hello, World!")

先頭の ``# coding: utf-8`` という記述は、スクリプトファイルのエンコーディングを指定するものです。スクリプト内で日本語を扱うときは必ず指定してください。

``python`` コマンドにファイルパスを指定することで、スクリプトファイルを実行できます。

::

   > python hello.py
   Hello, World!

モジュールを作る
----------------

``.py`` の拡張子のファイルはPythonモジュールとして ``import`` で読み込んで使用できます。

mymodule.py という名前のPythonモジュールを作成し、読み込んで使用する例を以下に示します。

**mymodule.py**:

.. code-block:: python

   # coding: utf-8
   def hello():
       print("Hello, World")

   def add(a, b):
       return a + b

モジュールをインポートする場合、該当するモジュールのパスがPythonパス(PythonPath, PYTHONPATH)に含まれている必要があります。Pythonパスは ``sys.path`` で確認できます。

.. code-block:: pycon

   >>> import mymodule
   >>> mymodule.hello()
   Hello, World!
   >>> mymodule.add(1, 2)
   3

標準ライブラリ
--------------

Pythonの標準の配布物には、多くのライブラリ(**標準ライブラリ**)が含まれています。これらのモジュールを使うことにより、迅速に目的のアプリケーションを作成できます。

標準ライブラリについては、ここでは説明しきれません。Pythonのドキュメントの標準ライブラリのページを参照して下さい。

http://www.python.jp/doc/2.7/library/index.html

次は
----

これでモジュールについて学ぶことができました。

次はサードパーティのライブラリについて少し説明します。
