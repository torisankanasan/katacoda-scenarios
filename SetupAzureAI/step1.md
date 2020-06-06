# Translator Text API を利用するためのアクセスキーの作成

Step1 ではAzure Cognitive ServicesのTranslator Text APIを利用するためのアクセスキーを作成します。

Text Analytics API を呼び出すためにアクセス キーが必要になります。
まずAzure portal を使用してアクセスキーを取得します。

## 1-1. Azure Portal にログイン

[Azure Portal](https://azure.microsoft.com/ja-jp/features/azure-portal/) にアクセスしてログイン
![Azure Portal](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/Microsoft_Azure_Portal___Microsoft_Azure.png)

## 1-2. リソースの作成

Azure portal のメニューまたは [ホーム] ページで [リソースの作成] を選択します。
![プロバイダー選択](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LineBotBasicCourse/LineBotBasicScenario/images/ProviderList.png)

## 1-2. リソースの作成

[Marketplace を検索] 検索ボックスに「text analytics」と入力して Enter キーまたは Return キーを押します。
![プロバイダー選択](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LineBotBasicCourse/LineBotBasicScenario/images/ProviderList.png)

## 1-2. リソースの作成
検索結果で [Text Analytics] を選択し、画面の右下にある [作成] ボタンをクリックします。

## 1-2. リソースの作成
表示された [作成] ページで、各フィールドに次の値を入力します。

## 1-3. チャネルを新規作成

Botのチャネルを作成
![チャネル作成](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LineBotBasicCourse/LineBotBasicScenario/images/NewChannel.png)

「Messaging API」 を選択
![Messaging API](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LiffKintoneQuestionaryCourse/SetupBotAndLiff/images/SelectMessagingAPI.png)

チャネル情報を入力して、「入力内容を確認する」ボタンを押下する

## 1-4. アクセスキー をメモしておく

チャネル基本情報画面に表示されているアクセスキーをメモしておく

![CopyChannelSecret](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LiffKintoneQuestionaryCourse/SetupBotAndLiff/images/CopyChannelSecret_01.png)

![CopyChannelSecret](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LineBotBasicCourse/LineBotBasicScenario/images/CopyChannelSecret_02.png)

### お疲れ様でした
### 次のStep では、Text Analytics APIのアクセスキーを作成します