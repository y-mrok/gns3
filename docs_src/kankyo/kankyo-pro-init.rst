.. _kankyo-pro-init:

**************************************************
VMware Pro：GNS3 の初期設定
**************************************************

.. _kankyo-pro-init-setup-wizard:

セットアップウィザード
==================================================
初めて GNS3 を起動したとき、セットアップウイザードが実行されます。

#. GNS3 を起動

   .. image:: img/2020-09-19_14h00_00.png

   |

#. :guilabel:`Next` をクリック

   .. image:: img/2020-09-19_14h01_03.png

   |

#. :guilabel:`Next` をクリック

   .. image:: img/2020-09-19_14h01_26.png

   |

#. :guilabel:`Next` をクリック

   .. image:: img/2020-09-19_14h02_16.png

   |

#. GNS3 VM に割り当てるリソース（ vCPU 数 /メモリサイズ）を指定

   .. note::

      割り当てるリソースに関して「 `Local GNS3 VM Setup Wizard <https://docs.gns3.com/docs/getting-started/setup-wizard-gns3-vm/#local-gns3-vm-setup-wizard>`_ 」に次の記述があります。

      .. image:: img/2020-09-19_14h06_08.png

      |

      `翻訳サイト <https://www.deepl.com/translator>`_ で翻訳した結果です。
      
      重要
      
      GNS3では、最低1つのvCPUコアと2GBのRAMを推奨しています。しかし、多くのデバイスで大規模なトポロジを実行したい場合は、より多くのCPUコアとRAMを推奨します。設定は後からGNS3のGUIを使って調整できます。経験則としては、PCで利用可能なvCPUコアと物理RAMの合計量の半分を割り当てるのが良いでしょう。以下の例では、ラップトップで実行しているため、最小限のリソース割り当てを使用しています。ハイパースレッディングと32GBのRAMを持つi7クアッドコアCPUを持つデスクトップでは、GNS3 VMを4-6個のvCPUと16GBのRAMに割り当てることで、立派なGNS3トポロジを実行することができ、同時にGNS3とWindows（またはLinux）の間でタスクを切り替えるのに十分なリソースを確保することができます。

   .. image:: img/2020-09-19_14h06_58.png

   ↓

   .. image:: img/2020-09-19_14h07_24.png

   |

#. :guilabel:`Next` をクリック

   .. image:: img/2020-09-19_14h07_37.png

   |

#. GNS3 VM の起動待ち

   .. image:: img/2020-09-19_14h08_11.png

   |

#. VMware Workstation Pro が起動　→　GNS3 VM が起動　→　:guilabel:`OK` を押下

   .. image:: img/2020-09-19_14h09_25.png

   |

#. GNS3 VM の起動終了

   .. image:: img/2020-09-19_14h09_54.png

   |

#. :guilabel:`Finish` をクリック

   .. image:: img/2020-09-19_14h10_19.png

   |

#. GNS3 の起動終了

   .. image:: img/2020-09-19_14h10_39.png

   |

.. _kankyo-pro-init-teraterm:

ターミナルソフトを TeraTerm Pro に変更
==================================================
「 :ref:`kankyo-install-pro-gns3` 」で putty をインストールしなかったので、使用するターミナルソフトを TeraTerm に変更します。

#. :guilabel:`Edit` をクリック

   .. image:: img/2020-09-19_14h11_57.png

   |

#. :guilabel:`Preferences...` をクリック

   .. image:: img/2020-09-19_14h12_12.png

   |

#. :guilabel:`Console Applications` をクリック

   .. image:: img/2020-09-19_14h12_31.png

   |

#. :guilabel:`Edit` をクリック

   .. image:: img/2020-09-19_14h12_50.png

   |

#. :guilabel:`Choose a predefined command` のプルダウンリストから :guilabel:`TeraTerm Pro` を選択

   .. image:: img/2020-09-19_14h13_11.png

   ↓

   .. image:: img/2020-09-19_14h13_31.png

   |

#. コマンドを次のように変更

   .. code-block:: none

      "C:\Program Files (x86)\teraterm\ttermpro.exe" /W="%d" /T=1 %h %p

   .. image:: img/2020-09-19_14h14_14.png

   |

#. :guilabel:`OK` をクリック

   .. image:: img/2020-09-19_14h14_26.png

   |

#. :guilabel:`OK` をクリック

   .. image:: img/2020-09-19_14h14_43.png

   |

#. 変更終了

   .. image:: img/2020-09-19_14h14_56.png

   |
