# Text Analytics API を利用するためのエンドポイントURLとアクセスキーの作成

Step2 ではText Analytics API を利用するためのエンドポイントURLとアクセスキーを作成します。

## 2-1. リソースの作成

先ほど、ログインしたAzure portal のメニューまたはホームで [リソースの作成] を選択
![ホーム_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/ホーム_Microsoft_Azure.png)

検索ボックスに「text analytics」と入力して Enter キーを押す
![新規_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/新規_-_Microsoft_Azure.png)

検索結果から [Text Analytics] を選択し、 [作成] ボタンをクリック

表示された [作成] ページで、各入力欄に次の値を入力し、下部にある [確認および作成] ボタンをクリック

### 入力例

|  項目名  |  値  |
| :-- | :-- |
|  サブスクリプション  |  ご自身が利用したいもの  |
|  リソース グループ  |  ldc_handson_20200609（なんでも）  |
|  リージョン  |  東アジア  |
|  Name  |  ldc-handson-translator  |
|  Pricing tier |  F0 （Free レベルの選択がオススメ）  |

![Translator_の作成_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/Translator_の作成_-_Microsoft_Azure.png)

下部にある [作成] ボタンをクリック

![Translator_の確認_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/Translator_の確認_Microsoft_Azure.png)

## 2-2. エンドポイントURLとアクセスキーの確認

 [リソースに移動] ボタンをクリック
 ![Microsoft_CognitiveServicesTextTranslation-20200607132704___概要_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/Microsoft_CognitiveServicesTextTranslation-20200607132704___概要_-_Microsoft_Azure.png)

左側のメニューの [キーとエンドポイント]、または[キーを管理するにはここをクリック]をクリック
![ldc-handson-translator_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/ldc-handson-translator_-_Microsoft_Azure.png)

## 2-4. エンドポイントURLとアクセスキー をメモしておく

コピー ボタンをクリックして、いずれかのキーとエンドポイントURLをコピーし、メモしておく

![ldc-handson-translator___キーとエンドポイント_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/ldc-handson-translator___キーとエンドポイント_-_Microsoft_Azure.png)

### お疲れ様でした
### 次は、LINE Bot とリッチメニュー、そしてLIFF の設定を行います。