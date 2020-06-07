# Text Analytics API を利用するためのエンドポイントURLとアクセスキーの作成

Step2 ではText Analytics API を利用するためのエンドポイントURLとアクセスキーを作成します。

## 2-1. リソースの作成

先ほど、ログインしたAzure portal のメニューまたはホームで [リソースの作成] を選択
![ホーム_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/ホーム_Microsoft_Azure.png)

検索ボックスに「テキスト分析」と入力して Enter キーを押す
![analytics_新規_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/analytics_新規_-_Microsoft_Azure.png)

検索結果から [テキスト分析] を選択し、 [作成] ボタンをクリック
![analytics_Marketplace_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/analytics_Marketplace_-_Microsoft_Azure.png)

![テキスト分析_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/テキスト分析_-_Microsoft_Azure.png)

表示された [作成] ページで、各入力欄に次の値を入力し、下部にある [作成] ボタンをクリック

### 入力例

|  項目名  |  値  |
| :-- | :-- |
|  名前  |  ldc-handson-text-analytics-${ご自身のお名前など}（他の人と被らなければOK）  |
|  サブスクリプション  |  ご自身が利用したいもの  |
|  場所  |  （Asia Pacific）東日本  |
|  価格レベル |  Free F0 （Free レベルの選択がオススメ）  |
|  リソース グループ  |  ldc_handson_20200609（先ほどと同じでOK）  |

![作成_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/作成_-_Microsoft_Azure.png)

## 2-2. エンドポイントURLとアクセスキーの確認

 [リソースに移動] ボタンをクリック
 ![Microsoft_CognitiveServicesTextAnalytics___概要_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/Microsoft_CognitiveServicesTextAnalytics___概要_-_Microsoft_Azure.png)

左側のメニューの [キーとエンドポイント]、または[キーを管理するにはここをクリック]をクリック
![ldc-handson-text-analytics_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/ldc-handson-text-analytics_-_Microsoft_Azure.png)

## 2-4. エンドポイントURLとアクセスキー をメモしておく

コピー ボタンをクリックして、いずれかのキーとエンドポイントURLをコピーし、メモしておく

![ldc-handson-text-analytics___キーとエンドポイント_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/ldc-handson-text-analytics___キーとエンドポイント_-_Microsoft_Azure.png)

### お疲れ様でした
### 次は、LINE Bot とリッチメニュー、そしてLIFF の設定を行います。