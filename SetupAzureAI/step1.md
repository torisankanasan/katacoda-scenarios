# Translator API を利用するためのアクセスキーの作成

Step1 ではTranslator API を利用するためのアクセスキーを作成します。

まずAzure Portal を使用してアクセスキーを取得します。

## 1-1. Azure Portal にログイン

[Azure Portal](https://azure.microsoft.com/ja-jp/features/azure-portal/) にアクセスしてログイン
![Azure Portal](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/Microsoft_Azure_Portal___Microsoft_Azure.png)

## 1-2. リソースの作成

Azure Portal のメニューまたはホームで [リソースの作成] を選択
![ホーム_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/ホーム_Microsoft_Azure.png)

検索ボックスに「translator」と入力して Enter キーを押す
![新規_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/新規_-_Microsoft_Azure.png)

検索結果から [Translator] を選択し、[作成] ボタンをクリック
![Marketplace_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/Marketplace_-_Microsoft_Azure.png)

![Translator_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/Translator_Microsoft_Azure.png)

表示された作成ページで、各入力欄に次の値を入力し、下部にある [確認および作成] ボタンをクリック

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

## 1-3. アクセスキーの確認

 [リソースに移動] ボタンをクリック
 ![Microsoft_CognitiveServicesTextTranslation-20200607132704___概要_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/Microsoft_CognitiveServicesTextTranslation-20200607132704___概要_-_Microsoft_Azure.png)

左側のメニューの [キーとエンドポイント]、または [キーを管理するにはここをクリック] をクリック
![ldc-handson-translator_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/ldc-handson-translator_-_Microsoft_Azure.png)

## 1-4. アクセスキー をメモしておく

コピー ボタンをクリックして、いずれかのキーをコピーし、メモしておく

![ldc-handson-translator___キーとエンドポイント_-_Microsoft_Azure](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/ldc-handson-translator___キーとエンドポイント_-_Microsoft_Azure.png)

### お疲れ様でした
### 次のStep では、Text Analytics APIのアクセスキーを作成します