.. _walkthru:

**************************************************
ウォークスルー
**************************************************
新規プロジェクトの作成　～　オブジェクトの配置／設定　～　動作確認までを通しで行います。

#. 新規プロジェクトの作成

   .. image:: img/2020-09-05_18h26_06.png

   |

#. オブジェクトの配置

   .. image:: img/2020-09-05_18h28_23.png

   |

#. インターフェース名を表示

   .. image:: img/2020-09-05_18h28_54.png

   |

#. 全オブジェクトの電源 ON

   .. image:: img/2020-09-05_18h29_13.png

   |

.. note::

   以下は :ref:`object-console` して実行します。

5. R1 の設定

   ■ 実行するコマンド

   .. literalinclude:: ./r1.txt
      :language: none

   ■ 実行ログ

   .. literalinclude:: ./r1.log
      :language: none

#. R2 の設定

   ■ 実行するコマンド

   .. literalinclude:: ./r2.txt
      :language: none

   ■ 実行ログ

   .. literalinclude:: ./r2.log
      :language: none

#. PC1 の設定

   ■ 実行するコマンド

   .. code-block:: none

      ip 192.168.11.1 255.255.255.0 192.168.11.254
      ping 192.168.31.1

   ■ 実行ログ　：　``ping`` コマンドは PC2 に IP アドレスを設定後に実行した

   .. literalinclude:: ./pc1.log
      :language: none

#. PC2 の設定

   ■ 実行するコマンド

   .. code-block:: none

      ip 192.168.31.1 255.255.255.0 192.168.31.254
      ping 192.168.11.1

   ■ 実行ログ

   .. literalinclude:: ./pc2.log
      :language: none
    