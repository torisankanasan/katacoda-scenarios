This is your first step.

## リッチメニューの作成

APIを使ってリッチメニューを作成します。

`echo 'Hello World'`{{execute}}

`curl -v -X POST https://api.line.me/v2/bot/richmenu -H 'Authorization: Bearer {channel access token}' -H 'Content-Type: application/json' -d '{"size": {"width": 2500,"height": 1686},"selected": false,"name": "Nice richmenu","chatBarText": "Tap here","areas": [{"bounds": {"x": 0,"y": 0,"width": 2500,"height": 1686},"action": {"type": "postback","data": "action=buy&itemid=123"}}]}'`{{execute}}