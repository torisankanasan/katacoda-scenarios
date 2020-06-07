# リッチメニューの作成・設定

Step2 ではMessaging API を使ってリッチメニューを作成します。

## 2-1. チャネルアクセストークンを変数に設定する

先ほど発行したチャネルアクセストークンを使ってリッチメニューを作成します。

Terminal で以下のコマンドを実行し、チャネルアクセストークンを変数に設定します。

`LINE_TOKEN=${your_token}`

<font color="red">※ `${your_token}` 部分は先ほど発行したご自身のチャネルアクセストークンに置き換えてください。</font><br>

## 2-2. リッチメニューの画像を準備する

Terminal で以下のコマンドを実行し、リッチメニューに使う画像をダウンロードします。
（コマンド部分をクリックすると実行できます）

`curl -OL https://raw.githubusercontent.com/sumihiro3/line-kintone-azure-takeout/master/richmenu_default_ja.png`{{execute}}

## 2-3. タップ領域を指定してリッチメニューを作成し、richmenuIdをメモしておく

Terminal で以下のコマンドを実行し、タップ領域を指定してリッチメニューを作成します。
（コマンド部分をクリックすると実行できます）

レスポンスに含まれるrichmenuIdをメモしておく

`curl -v -X POST https://api.line.me/v2/bot/richmenu -H 'Authorization: Bearer '"$LINE_TOKEN"'' -H 'Content-Type: application/json' -d '{"size": {"width": 2500,"height": 843},"selected": true,"name": "richmenu-default","chatBarText": "メニュー","areas": [{"bounds": {"x": 0,"y": 0,"width": 1250,"height": 843},"action": {"type": "postback","data": "type=menu","displayText": "注文する"}},{"bounds": {"x": 1250,"y": 0,"width": 625,"height": 422},"action": {"type": "postback","data": "type=business-hour","displayText": "営業時間"}},{"bounds": {"x": 1875,"y": 0,"width": 625,"height": 422},"action": {"type": "postback","data": "type=access","displayText": "アクセス"}},{"bounds": {"x": 1250,"y": 422,"width": 1250,"height": 421},"action": {"type": "postback","data": "type=customer-support","displayText": "問い合わせ"}}]}'`{{execute}}

richmenuIdをメモしておく

![response](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/LINE_BotとリッチメニューとLIFFの設定___torisankanasan___Katacoda.png)

## 2-4. richMenuIdを変数に設定する

Terminal で以下のコマンドを実行し、richMenuIdを変数に設定します。

`richMenuId=${richMenuId}`

<font color="red">※ `${your_richMenuId}` 部分は先ほどメモしたご自身のrichMenuIdに置き換えてください。</font><br>

## 2-5. リッチメニューに画像をアップロードして添付する

Terminal で以下のコマンドを実行し、前の手順で作成したリッチメニューに、画像をアップロードして添付します。
（コマンド部分をクリックすると実行できます）

`curl -v -X POST https://api.line.me/v2/bot/richmenu/"$richMenuId"/content -H 'Authorization: Bearer '"$LINE_TOKEN"'' -H 'Content-Type: image/png' -T ./richmenu_default_ja.png`{{execute}}

以下のように空のJSONオブジェクトが返ってこれば、完了です。

![response](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/response.png)

### お疲れ様でした
### 次のStep では、LIFF の設定を行います