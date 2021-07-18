.. _kankyo-init:

**************************************************
VMware Player：GNS3 の初期設定
**************************************************

.. _kankyo-init-setup-wizard:

セットアップウィザード
==================================================
初めて GNS3 を起動したとき、セットアップウイザードが実行されます。

#. GNS3 を起動

   .. image:: img/2020-09-04_22h03_17.png

   |

#. :guilabel:`Next` をクリック

   .. image:: img/2020-09-04_22h04_03.png

   |

#. :guilabel:`Next` をクリック

   .. image:: img/2020-09-04_22h04_18.png

   |

#. :guilabel:`Next` をクリック

   .. image:: img/2020-09-04_22h04_45.png

   |

#. GNS3 VM に割り当てるリソース（ vCPU 数 /メモリサイズ）を指定

   .. note::

      割り当てるリソースに関して「 `Local GNS3 VM Setup Wizard <https://docs.gns3.com/docs/getting-started/setup-wizard-gns3-vm/#local-gns3-vm-setup-wizard>`_ 」に次の記述があります。

      .. image:: img/2020-09-05_05h35_47.png

      |

      `翻訳サイト <https://www.deepl.com/translator>`_ で翻訳した結果です。
      
      重要
      
      GNS3では、最低1つのvCPUコアと2GBのRAMを推奨しています。しかし、多くのデバイスで大規模なトポロジを実行したい場合は、より多くのCPUコアとRAMを推奨します。設定は後からGNS3のGUIを使って調整できます。経験則としては、PCで利用可能なvCPUコアと物理RAMの合計量の半分を割り当てるのが良いでしょう。以下の例では、ラップトップで実行しているため、最小限のリソース割り当てを使用しています。ハイパースレッディングと32GBのRAMを持つi7クアッドコアCPUを持つデスクトップでは、GNS3 VMを4-6個のvCPUと16GBのRAMに割り当てることで、立派なGNS3トポロジを実行することができ、同時にGNS3とWindows（またはLinux）の間でタスクを切り替えるのに十分なリソースを確保することができます。

   .. image:: img/2020-09-05_05h38_46.png

   ↓

   .. image:: img/2020-09-05_05h40_05.png

   |

#. :guilabel:`Next` をクリック

   .. image:: img/2020-09-05_05h40_34.png

   |

#. GNS3 VM の起動待ち

   .. image:: img/2020-09-05_05h40_50.png

   |

#. VMware Workstation Player が起動　→　GNS3 VM が起動　→　:guilabel:`OK` を押下

   .. note::

      VMware Workstation Player が起動すると、下図のような VMware Tools のダウンロードを確認されることがあります。この図が表示されたら :guilabel:`ダウンロードしてインストール(D)` を選択してください。
   
      .. image:: img/2020-09-05_05h41_17.png

   .. image:: img/2020-09-05_05h42_03.png

   |

#. GNS3 VM の起動終了

   .. image:: img/2020-09-05_05h42_36.png

   |

#. :guilabel:`Finish` をクリック

   .. image:: img/2020-09-05_05h42_58.png

   |

#. GNS3 の起動終了

   .. image:: img/2020-09-05_05h43_36.png

   |

.. _kankyo-init-teraterm:

ターミナルソフトを TeraTerm Pro に変更
==================================================
「 :ref:`kankyo-install-gns3` 」で putty をインストールしなかったので、使用するターミナルソフトを TeraTerm に変更します。

#. :guilabel:`Edit` をクリック

   .. image:: img/2020-09-05_05h58_15.png

   |

#. :guilabel:`Preferences...` をクリック

   .. image:: img/2020-09-05_05h58_24.png

   |

#. :guilabel:`Console Applications` をクリック

   .. image:: img/2020-09-05_05h58_37.png

   |

#. :guilabel:`Edit` をクリック

   .. image:: img/2020-09-05_05h58_47.png

   |

#. :guilabel:`Choose a predefined command` のプルダウンリストから :guilabel:`TeraTerm Pro` を選択

   .. image:: img/2020-09-05_05h59_05.png

   ↓

   .. image:: img/2020-09-05_05h59_22.png

   |

#. コマンドを次のように変更

   .. code-block:: none

      "C:\Program Files (x86)\teraterm\ttermpro.exe" /W="%d" /T=1 %h %p

   .. image:: img/2020-09-05_06h04_04.png

   |

#. :guilabel:`OK` をクリック

   .. image:: img/2020-09-05_06h04_08.png

   |

#. :guilabel:`OK` をクリック

   .. image:: img/2020-09-05_06h04_15.png

   |

#. 変更終了

   .. image:: img/2020-09-05_06h04_26.png

   |
