.. _kankyo:

**************************************************
環境構築
**************************************************
Windows 10 上に GNS3 の実行環境を構築します。

| ● :ref:`kankyo-spec`
| ● :ref:`kankyo-chuui`
| ● :ref:`kankyo-packages`
| 　・ :ref:`kankyo-packages-common`
| 　・ :ref:`kankyo-packages-vmware`
| 　・ :ref:`kankyo-packages-virtualbox`
| 　・ :ref:`kankyo-packages-vmware-pro`
| ● :ref:`kankyo-install`
| 　・ :ref:`kankyo-install-vmware`
| 　・ :ref:`kankyo-install-virtualbox`
| 　・ :ref:`kankyo-install-vmware-pro`

.. _kankyo-spec:

GNS3 を実行するパソコンのスペック
==================================================
GNS3 を実行するパソコンの必要スペックです（リンク先をご確認ください）。

- `最小構成 <https://docs.gns3.com/docs/getting-started/installation/windows#minimum-requirements>`_
- `推奨構成 <https://docs.gns3.com/docs/getting-started/installation/windows#recommended-requirements>`_
- `最適な構成 <https://docs.gns3.com/docs/getting-started/installation/windows#optimal-requirements>`_

今回 GNS3 をインストールするパソコンのスペックです。

.. image:: img/2020-09-02_20h47_07.png

|

.. _kankyo-chuui:

VMware Workstation Player で環境構築するときの注意
==================================================
VMware Workstation Player と VMware VIX の組み合わせは「 `GNS3 Setup wizard with the GNS3 VM <https://docs.gns3.com/docs/getting-started/setup-wizard-gns3-vm/>`_ 」内の「 `VMware Workstation vs. Player <https://docs.gns3.com/docs/getting-started/setup-wizard-gns3-vm/#vmware-workstation-vs-player>`_ 」によると次のとおりです。

- VMware Workstation 14 Player + VMware VIX 1.17
- VMware Workstation 12 Player + VMware VIX 1.15 （以降のバージョン）

現行バージョンである VMware Workstation 15 Player に対応する VMware VIX はリリースされていません。そのため VMware Workstation 15 Player 上で GNS3 を動作させる方法はフォーラム「 `GNS3 with Workstation Player 15.5 <https://gns3.com/community/featured/gns3-with-workstation-player-15->`_ 」で議論中なので本ドキュメントでは取り扱いません。なお、 VMware Workstation 15 Pro は VMware VIX を内蔵しているので、 VMware VIX のインストールなしで環境構築ができます。

本ドキュメントで VMware を使用する場合は下記の組み合わせで環境を構築します。

- VMware Workstation 14 Player + VMware VIX 1.17

|

.. _kankyo-packages:

インストールするアプリケーション
==================================================
インストールするアプリケーションの一覧です。一部のアプリケーションのダウンロードにアカウントが必要です。アカウントは無料で作成できます。

.. note::

   VMware と Oracle VirtualBox で GNS3 のバージョンが異なるのは、異なる日にダウンロードしたためです。 Oracle VirtualBox 用をダウンロードしたとき、少しだけバージョンが上がっていました。

.. _kankyo-packages-common:

共通
--------------------------------------------------
VMware / Oracle VM VirtualBox のどちらの環境で使用するアプリケーションです。これらは環境構築に着手する前にインストールします。

.. list-table::

   * - アプリケーション名
     - ファイル名
     - 備考
   * - `teraterm 4.105 <https://ja.osdn.net/projects/ttssh2/releases/72009>`_
     - teraterm-4.105.exe
     - ターミナルソフト
   * - `Sakura Editor 2.4.1 <https://github.com/sakura-editor/sakura/releases>`_
     - sakura-tag-v2.4.1-build2849-ee8234f-Win32-Release-Installer.zip
     - テキストエディタ（使い慣れたもので良い）

|

.. _kankyo-packages-vmware:

VMware Workstation Player 編
--------------------------------------------------
.. list-table::

   * - アプリケーション名
     - ファイル名
     - 備考
   * - `GNS3 2.2.12 <https://www.gns3.com/software/download>`_
     - GNS3-2.2.12-all-in-one-regular.exe
     - Windows
   * - `GNS3 VM <https://gns3.com/software/download-vm>`_
     - GNS3.VM.VMware.Workstation.2.2.12.zip
     - VMware Workstation and Fusion
   * - `VMware Workstation 14.1.8 Player <https://my.vmware.com/jp/web/vmware/downloads/details?downloadGroup=PLAYER-1418&productId=687&rPId=39191>`_
     - VMware-player-14.1.8-14921873.exe
     - Windows 64-bit Operating Systems
   * - `VMware VIX 1.17.0 API <https://my.vmware.com/group/vmware/downloads/details?downloadGroup=PLAYER-1400-VIX1170&productId=687>`_
     - VMware-VIX-1.17.0-6661328.exe
     -  Windows 64-bit Operating Systems

環境構築は赤枠で囲んだものを使用します。

.. image:: img/2020-09-02_21h20_02.png

|

.. _kankyo-packages-virtualbox:

Oracle VM VirtualBox 編
--------------------------------------------------
.. list-table::

   * - アプリケーション名
     - ファイル名
     - 備考
   * - `GNS3 2.2.13 <https://www.gns3.com/software/download>`_
     - GNS3-2.2.13-all-in-one-regular.exe
     - Windows
   * - `GNS3 VM <https://gns3.com/software/download-vm>`_
     - GNS3.VM.VirtualBox.2.2.13.zip
     - VirtualBox
   * - `Oracle VirtualBox 6.1.14 <https://www.virtualbox.org/wiki/Downloads>`_
     - VirtualBox-6.1.14-140239-Win.exe
     - Windows hosts
   * - `Oracle VM VirtualBox Extension Pack <https://www.virtualbox.org/wiki/Downloads>`_
     - Oracle_VM_VirtualBox_Extension_Pack-6.1.14.vbox-extpack
     - All supported platforms

環境構築は赤枠で囲んだものを使用します。

.. image:: img/2020-09-06_18h30_02.png

|

.. _kankyo-packages-vmware-pro:

VMware Workstation Pro 編
--------------------------------------------------
.. list-table::

   * - アプリケーション名
     - ファイル名
     - 備考
   * - `GNS3 2.2.14 <https://www.gns3.com/software/download>`_
     - GNS3-2.2.14-all-in-one-regular.exe
     - Windows
   * - `GNS3 VM <https://gns3.com/software/download-vm>`_
     - GNS3.VM.VMware.Workstation.2.2.14.zip
     - VMware Workstation and Fusion
   * - `VMware Workstation 16 Pro <https://www.vmware.com/jp/products/workstation-pro/workstation-pro-evaluation.html>`_
     - VMware-workstation-full-16.0.0-16894299.exe
     - 試用版

環境構築は赤枠で囲んだものを使用します。

.. image:: img/2020-09-19_10h59_07.png

|

.. _kankyo-install:

アプリケーションのインストールと初期設定
==================================================

.. _kankyo-install-vmware:

VMware Workstation Player 編
--------------------------------------------------
#. :ref:`VMware Workstation 14 Player <kankyo-install-vmware-workstation-player>`
#. :ref:`VMware VIX <kankyo-install-vmware-vix>`
#. :ref:`GNS3 VM のインポート <kankyo-install-gns3-vm>`
#. :ref:`GNS3 <kankyo-install-gns3>`
#. :ref:`GNS3 の初期設定 <kankyo-init>`


.. _kankyo-install-virtualbox:

Oracle VM VirtualBox 編
--------------------------------------------------
#. :ref:`Oracle VM VirtualBox <kankyo-install-oracle-virtualbox>`
#. :ref:`GNS3 VM のインポート <kankyo-install-vb-gns3-vm>`
#. :ref:`GNS3 <kankyo-install-vb-gns3>`
#. :ref:`GNS3 の初期設定 <kankyo-vb-init>`

.. _kankyo-install-vmware-pro:

VMware Workstation Pro 編
--------------------------------------------------
#. :ref:`VMware Workstation 16 Pro （試用版） <kankyo-install-vmware-workstation-pro>`
#. :ref:`GNS3 VM のインポート <kankyo-install-pro-gns3-vm>`
#. :ref:`GNS3 <kankyo-install-pro-gns3>`
#. :ref:`GNS3 の初期設定 <kankyo-pro-init>`

.. toctree::
   :hidden:

   ./kankyo-install-vmware-workstation-player
   ./kankyo-install-vmware-vix
   ./kankyo-install-gns3-vm
   ./kankyo-install-gns3
   ./kankyo-init
   ./kankyo-install-oracle-virtualbox
   ./kankyo-install-vb-gns3-vm
   ./kankyo-install-vb-gns3
   ./kankyo-vb-init
   ./kankyo-install-vmware-workstation-pro
   ./kankyo-install-pro-gns3-vm
   ./kankyo-install-pro-gns3
   ./kankyo-pro-init
