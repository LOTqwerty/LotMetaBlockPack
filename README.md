# LotMetaBlockPack

メタCTMを活用した建築を補助するMOD・Pluginです。

バニラでメタを持たないブロックでも、メタを保持したままスポイトや設置をできるようにします。


## ダウンロード

[LotMetaBlockMod MC1.7.10 Forge用 最新(v2.1.1)](https://drive.google.com/open?id=1fu36nYGB9F8M8B1yWHMI_nNhtUCzEI3M)

[全てのダウンロード](https://drive.google.com/drive/folders/1PPxjFPtVM3lspYbFkwAWdvSsfhQgEDie?usp=sharing)

## 導入方法

**このMod/Pluginは本来バニラでは存在しないブロックやアイテムを扱うため、 意図せずクラッシュする/ワールドを開けなくなるなどの事態が発生する可能性があります。必ず、導入前にデータのバックアップを作成してください。また、使用中も定期的にバックアップを作成することをお勧めします。導入・使用はすべて自己責任でお願いします。**

### シングルで遊ぶ/マルチプレイに参加するひと

1. Minecraft 1.7.10にForgeを導入する
2. 上のダウンロードリンクから"LotMetaBlockMod Forge用"をダウンロードする
3. ダウンロードしたjarファイルをmodsフォルダに移動する
4. Minecraftを起動し、LotMetaBlockModが導入されたことを確認し、Minecraftを閉じる(configファイルが生成されます)
5. config設定をする(下記)
6. 再度、Minecraftを起動する

### マルチプレイのForgeサーバを建てるひと

1. Minecraft 1.7.10のサーバを用意し、Forgeを導入する
2. 上のダウンロードリンクから"LotMetaBlockMod Forge用"をダウンロードする
3. ダウンロードしたjarファイルをmodsフォルダに移動する
4. サーバが正常に起動することを確認し、サーバをシャットダウンする(configファイルが生成されます)
5. config設定をする(下記)
6. 再度、Minecraftを起動する

### マルチプレイのBukkitサーバを建てるひと

1. Bukkitサーバを用意する
2. 上のダウンロードリンクから"LotMetaBlockPlugin"をダウンロードする
3. ダウンロードしたファイルをBukkitサーバのpluginsフォルダに移動する


## 機能と操作方法

多くの機能は初期状態で無効化されています。configファイルを編集し、必要な機能を有効化してください。

|機能|詳細|初期設定|
|-|-|-|
|メタ保持Pick|メタ情報を保ったままPickします。通常のPickより長距離でも動作します。|Fキー|
|メタ変更|キーを押している間、ホイールスクロールによって手に持っているアイテムのメタを変更します。|Rキー|
|メタ解除|手に持っているアイテムが固定メタなら固定解除、そうでなければメタを0にします。|Cキー|
|ダイレクトメタチェンジ|キーを押している間、ホイールスクロールによって視線の先にあるブロックのメタを変更します。|初期設定 Xキー|
|メタ+1|手に持っているアイテムのメタを+1します。メタが15の場合は0にします。|(無効)|
|メタ-1|手に持っているアイテムのメタを-1します。メタが0の場合は15にします。|(無効)|
|ダイレクトメタ+1|視線の先にあるブロックのメタを+1します。メタが15の場合は0にします。|(無効)|
|ダイレクトメタ-1|視線の先にあるブロックのメタを-1します。メタが0の場合は15にします。|(無効)|
|ダイレクトチェンジ|手に持っているアイテムがブロックである場合、視線の先にあるブロックを持っているブロックで上書きします。|(無効)|
