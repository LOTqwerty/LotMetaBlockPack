# LotMetaBlockPack

メタCTMを活用した建築を補助するMOD・Pluginです。

バニラでメタを持たないブロックでも、メタを保持したままスポイトや設置をできるようにします。

1.6.4 / 1.7.10 に対応しています。

※ LotTweaks for 1.12.2 は こちら → https://lotqwerty.github.io/LotTweaks/


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


## 機能とConfig

### クライアント側 (シングル または マルチプレイに参加するひと)

**LotMetaBlockMod.cfg** を編集します。

key の項目では、以下のキーの有効/無効の切り替えができます。  
キーを有効化しても、サーバconfig側が無効の場合は機能を使用できません。  
編集後は必ずMinecraftを再起動してください。

|名前|動作|
|-|-|
|Meta Pick|メタ情報を保ったままPickします。通常のPickより長距離でも動作します。|
|Meta Change|キーを押している間、ホイールスクロールによって手に持っているアイテムのメタを変更します。|
|Meta Remove|手に持っているアイテムが固定メタなら固定解除、そうでなければメタを0にします。|
|Meta Up|手に持っているアイテムのメタを+1します。メタが15の場合は0にします。|
|Meta Down|手に持っているアイテムのメタを-1します。メタが0の場合は15にします。|
|Direct Meta Change|キーを押している間、ホイールスクロールによって視線の先にあるブロックのメタを変更します。|
|Direct Meta Up|視線の先にあるブロックのメタを+1します。メタが15の場合は0にします。|
|Direct Meta Down|視線の先にあるブロックのメタを-1します。メタが0の場合は15にします。|
|Direct Change|手に持っているアイテムがブロックである場合、視線の先にあるブロックを持っているブロックで上書きします。|

range の項目では、各機能の有効範囲の変更ができます。
値を大きくしすぎると(200超など)、正しく動作しない場合があります。

### Forgeサーバ側 (シングル または Forgeサーバを建てるひと)

**LotMetaBlockMod_Server.cfg** を編集します。  
多くの機能は初期状態で無効化されています。configファイルを編集し、必要な機能を有効化してください。  
編集後は必ずMinecraftサーバを再起動してください。

block,itemid : メタ関連機能を使うブロック/アイテムIDを設定します。  
directmetachange : trueに変更すると、ダイレクトメタチェンジの使用を許可します。  
directchange : trueに変更すると、ダイレクトチェンジの使用を許可します。
