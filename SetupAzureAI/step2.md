# リッチメニューの作成

Step2 ではLINE の設定画面でLIFF アプリを利用するためのリッチメニューを作成します。


先ほど発行したチャネルアクセストークンを使ってリッチメニューを作成します。

先ほど生成したアクセストークンを変数に設定します。
`LINE_BOT_CHANNEL_ACCESS_TOKEN=`

## リッチメニューの領域を作成し、レスポンスに含まれるrichmenuIdをメモしておく

`curl -v -X POST https://api.line.me/v2/bot/richmenu -H 'Authorization: Bearer '"$LINE_BOT_CHANNEL_ACCESS_TOKEN"'' -H 'Content-Type: application/json' -d '{"size": {"width": 2500,"height": 843},"selected": true,"name": "richmenu-default","chatBarText": "メニュー","areas": [{"bounds": {"x": 0,"y": 0,"width": 1250,"height": 843},"action": {"type": "postback","data": "type=menu","displayText": "注文する"}},{"bounds": {"x": 1250,"y": 0,"width": 625,"height": 422},"action": {"type": "postback","data": "type=business-hour","displayText": "営業時間"}},{"bounds": {"x": 1875,"y": 0,"width": 625,"height": 422},"action": {"type": "postback","data": "type=access","displayText": "アクセス"}},{"bounds": {"x": 1250,"y": 422,"width": 1250,"height": 421},"action": {"type": "postback","data": "type=customer-support","displayText": "問い合わせ"}}]}'`{{execute}}

レスポンスの以下の箇所に書かれているrichmenuIdを変数に設定します。
`richMenuId=`

リッチメニューに使う画像をダウンロードします。
`curl -OL https://raw.githubusercontent.com/sumihiro3/line-kintone-azure-takeout/master/richmenu_default_ja.png`{{execute}}

リッチメニューに画像を紐付けます。
`curl -v -X POST https://api.line.me/v2/bot/richmenu/"$richMenuId"/content -H 'Authorization: Bearer '"$LINE_BOT_CHANNEL_ACCESS_TOKEN"'' -H 'Content-Type: image/png' -T ./richmenu_default_ja.png`{{execute}}

### お疲れ様でした
### 次のStep では、LIFF の設定を行います