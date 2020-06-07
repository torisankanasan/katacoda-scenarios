# Text Analytics API を利用するためのエンドポイントURLとアクセスキーの作成

Step2 ではText Analytics API を利用するためのエンドポイントURLとアクセスキーを作成します。

## 2-1. リソースの作成

先ほど、ログインしたAzure portal のメニューまたはホームで [リソースの作成] を選択
![ホーム_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/ホーム_Microsoft_Azure.png)

検索ボックスに「text analytics」と入力して Enter キーを押す
![新規_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/新規_-_Microsoft_Azure.png)

検索結果で [Text Analytics] を選択し、画面の右下にある [作成] ボタンをクリックします。

表示された [作成] ページで、各フィールドに次の値を入力します。

ページの下部にある [作成] を選択して、アカウントの作成プロセスを開始します。 デプロイが進行中であることを示す通知を監視します。

## 2-2. エンドポイントURLとアクセスキーの確認
Cognitive Services アカウントを用意できたので、API の呼び出しを開始できるようにアクセス キーを見つけましょう。

"デプロイメントに成功しました" という通知の [リソースに移動] ボタンをクリックします。 この操作により、アカウントのクイック スタートが開きます。

左側のメニューまたはクイック スタートの [Grab your keys](キーの取得) セクションで、[キー] メニュー項目を選択します。 この操作により、[キーの管理] ページが開きます。

デプロイすると Key と Endpoint が生成されますので、それをメモに残しておきます。Cognitive Services は Key を生成するだけなので、デプロイの時間は 10秒ほどです。
AZURE_TEXT_ANALYTICS_URL=https://xxxxx.cognitiveservices.azure.com/
AZURE_TEXT_ANALYTICS_KEY=xxxxxxxxxxxxxxxxxx
AZURE_TRANSLATOR_KEY=xxxxxxxxxxxxxxxxxx

## 2-4. エンドポイントURLとアクセスキー をメモしておく
コピー ボタンを使用して、いずれかのキーをコピーします。
チャネル基本情報画面に表示されているアクセスキーをメモしておく

![CopyChannelSecret](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LiffKintoneQuestionaryCourse/SetupBotAndLiff/images/CopyChannelSecret_01.png)

![CopyChannelSecret](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LineB

### お疲れ様でした
### 次は、LINE Bot とリッチメニュー、そしてLIFF の設定を行います。