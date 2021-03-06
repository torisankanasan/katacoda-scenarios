# Bot チャネルの作成・設定

Step1 ではLINE 公式アカウントをBot として利用するためにチャネルの作成や設定を行います。

<font color="red">！注意！</font>アプリをherokuにデプロイしてから、公式アカウントと友達になってください。

## 1-1. LINE Developers にログイン

[LINE Developers](https://developers.line.biz/ja/) にアクセスしてログイン
![LINE Developers](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LineBotBasicCourse/LineBotBasicScenario/images/LINEDevelopers.png)


## 1-2. プロバイダーを選択

任意のプロバイダーを選択
![プロバイダー選択](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/LINE_Developers.png)

プロバイダー未作成の人は画面上の「作成」ボタンを押下して新規作成してください。

- *任意の「プロバイダー名」を入力して作成*
    - *LINE* という文字列は含められません


## 1-3. チャネルを新規作成

Botのチャネルを作成
![チャネル作成](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/チャネル作成_LINE_Developers.png)

「Messaging API」 を選択
![Messaging API](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LiffKintoneQuestionaryCourse/SetupBotAndLiff/images/SelectMessagingAPI.png)

チャネル情報を入力して、「入力内容を確認する」ボタンを押下する

### チャネル情報の入力例

|  項目名  |  値  |
| :-- | :-- |
|  アプリ名  |  テイクアウトアプリ  |
|  アプリ説明  |  LINE × kintone × Azure AIでテイクアウトアプリを作ってみよう！  |
|  大業種  |  個人  |
|  小業種  |  個人（その他）  |
|  メールアドレス  |  （ご自分のメールアドレス）  |
|  プライバシーポリシーURL  |  （入力不要）  |
|  サービス利用規約URL  |  （入力不要）  |


![チャネルの情報を入力](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/チャネル情報入力_LINE_Developers.png)

各種規約に同意してチャネルを作成する

![各種規約に同意](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LineBotBasicCourse/LineBotBasicScenario/images/AgreeTerms.png)

情報利用に関する事項に同意する

![情報利用に関する事項に同意する](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LineBotBasicCourse/LineBotBasicScenario/images/AgreeTerms02.png)


## 1-4. チャネルシークレット をメモしておく

チャネル基本情報画面に表示されているチャネルシークレット をメモしておく

![CopyChannelSecret](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/基本情報確認_LINE_Developers.png)

![CopyChannelSecret](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LineBotBasicCourse/LineBotBasicScenario/images/CopyChannelSecret_02.png)

## 1-5. Webhook 設定

次に、「Messaging API設定」タブに進みます。

<font color="red">！注意！</font>QRコードが表示されていますが、アプリをherokuにデプロイしてから、公式アカウントと友達になってください。

「Messaging API設定」タブ内にある、Webhook URL の「編集」ボタンを押下してWebhook URL を入力可能状態にする

![Webhook](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LineBotBasicCourse/LineBotBasicScenario/images/WebhookSetting_01.png)

![Webhook](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LineBotBasicCourse/LineBotBasicScenario/images/WebhookSetting_02.png)


Webhook URL に下記のダミーURL を入力して、「Webhookの利用」を有効にする

- `https://google.com` 

**後で正しい値に変更します**

![Webhook URL](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/webhook_LINE_Developers.png)
「Webhookの利用」を有効にする


## 1-6. 応答設定

LINE公式アカウント機能 の画面右側にある「編集」リンクを押下して、公式アカウントマネージャー画面を開く

![公式アカウントマネージャー画面](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LineBotBasicCourse/LineBotBasicScenario/images/MessageSetting01.png)

応答設定画面を開く

公式アカウントマネージャー画面左の「応答設定」を選択して応答設定画面を開く

![応答設定](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/応答設定_LINE_Official_Account_Manager.png)

応答設定を下記のように設定する

|  項目名  |  値  |
| :-- | :-- |
|  応答モード  |  Bot  |
|  あいさつメッセージ  |  オフ  |
|  応答メッセージ  |  オフ  |
|  Webhook  |  オン  |

![応答設定](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LiffKintoneQuestionaryCourse/SetupBotAndLiff/images/MessageSetting03.png)


## 1-7. チャネルアクセストークン を発行してメモしておく

 LINE Developersに戻り、「Messaging API 設定」タブ内にある、チャネルアクセストークンの「発行」ボタンを押下して発行し、メモしておく

![GenerateToken](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LineBotBasicCourse/LineBotBasicScenario/images/GenerateToken_01.png)

![GenerateToken](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LineBotBasicCourse/LineBotBasicScenario/images/GenerateToken_02.png)

### お疲れ様でした
### 次のStep では、リッチメニュー の設定を行います