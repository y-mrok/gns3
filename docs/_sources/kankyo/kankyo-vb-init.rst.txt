.. _kankyo-vb-init:

**************************************************
VirtualBox：GNS3 の初期設定
**************************************************

.. _kankyo-vb-init-setup-wizard:

セットアップウィザード
==================================================
初めて GNS3 を起動したとき、セットアップウイザードが実行されます。

#. GNS3 を起動

   .. image:: img/2020-09-06_21h46_26.png

   |

#. :guilabel:`Next` をクリック

   .. image:: img/2020-09-06_21h47_26.png

   |

#. :guilabel:`Next` をクリック

   .. image:: img/2020-09-06_21h47_51.png

   |

#. :guilabel:`Next` をクリック

   .. image:: img/2020-09-06_21h48_10.png

   |

#. :guilabel:`OK` をクリック

   .. image:: img/2020-09-06_21h48_34.png

   |

   .. note::

      このエラーは仮想化プラットホームに VMware を使用している場合のものです。今回は Oracle VirtualBox を使用しているので無視して良い。

   |

#. :guilabel:`Virtualization software` は :guilabel:`VirtualBox` を選択

   .. image:: img/2020-09-06_21h51_58.png

   |

#. :guilabel:`VirtualBox` を選択　→　GNS3 VM に割り当てるリソース（ vCPU 数 /メモリサイズ）を指定

   .. note::

      割り当てるリソースに関して「 `Local GNS3 VM Setup Wizard <https://docs.gns3.com/docs/getting-started/setup-wizard-gns3-vm/#local-gns3-vm-setup-wizard>`_ 」に次の記述があります。

      .. image:: img/2020-09-06_21h59_46.png

      |

      `翻訳サイト <https://www.deepl.com/translator>`_ で翻訳した結果です。
      
      重要
      
      GNS3では、最低1つのvCPUコアと2GBのRAMを推奨しています。しかし、多くのデバイスで大規模なトポロジを実行したい場合は、より多くのCPUコアとRAMを推奨します。設定は後からGNS3のGUIを使って調整できます。経験則としては、PCで利用可能なvCPUコアと物理RAMの合計量の半分を割り当てるのが良いでしょう。以下の例では、ラップトップで実行しているため、最小限のリソース割り当てを使用しています。ハイパースレッディングと32GBのRAMを持つi7クアッドコアCPUを持つデスクトップでは、GNS3 VMを4-6個のvCPUと16GBのRAMに割り当てることで、立派なGNS3トポロジを実行することができ、同時にGNS3とWindows（またはLinux）の間でタスクを切り替えるのに十分なリソースを確保することができます。

   .. image:: img/2020-09-06_21h52_34.png

   ↓

   .. image:: img/2020-09-06_21h52_56.png

   |

#. :guilabel:`Next` をクリック

   .. image:: img/2020-09-06_21h53_12.png

   |

#. GNS3 VM の起動待ち

   .. image:: img/2020-09-06_21h53_27.png

   |

#. Oracle VirtualBox が起動　→　GNS3 VM が起動　→　:guilabel:`OK` を押下

   .. image:: img/2020-09-06_21h57_28.png

   |

#. GNS3 VM の起動終了

   .. image:: img/2020-09-06_21h57_53.png

   |

#. :guilabel:`Finish` をクリック

   .. image:: img/2020-09-06_21h58_11.png

   |

#. GNS3 の起動終了

   .. image:: img/2020-09-06_21h58_31.png

   |

.. _kankyo-vb-init-teraterm:

ターミナルソフトを TeraTerm Pro に変更
==================================================
「 :ref:`kankyo-install-gns3` 」で putty をインストールしなかったので、使用するターミナルソフトを TeraTerm に変更します。

#. :guilabel:`Edit` をクリック

   .. image:: img/2020-09-06_22h00_16.png

   |

#. :guilabel:`Preferences...` をクリック

   .. image:: img/2020-09-06_22h00_34.png

   |

#. :guilabel:`Console Applications` をクリック

   .. image:: img/2020-09-06_22h00_55.png

   |

#. :guilabel:`Edit` をクリック

   .. image:: img/2020-09-06_22h00_59.png

   |

#. :guilabel:`Choose a predefined command` のプルダウンリストから :guilabel:`TeraTerm Pro` を選択

   .. image:: img/2020-09-06_22h01_29.png

   ↓

   .. image:: img/2020-09-06_22h01_47.png

   |

#. コマンドを次のように変更

   .. code-block:: none

      "C:\Program Files (x86)\teraterm\ttermpro.exe" /W="%d" /T=1 %h %p

   .. image:: img/2020-09-06_22h02_32.png

   |

#. :guilabel:`OK` をクリック

   .. image:: img/2020-09-06_22h02_47.png

   |

#. :guilabel:`OK` をクリック

   .. image:: img/2020-09-06_22h03_03.png

   |

#. 変更終了

   .. image:: img/2020-09-06_22h03_17.png

   |
