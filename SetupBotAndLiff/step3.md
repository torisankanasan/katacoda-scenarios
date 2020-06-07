# LIFF 用チャネルの作成・設定

Step3 ではLIFF アプリを利用するためのチャネルの作成や設定を行います。


## 3-1. LINE Developers にログイン

[LINE Developers](https://developers.line.biz/ja/) にアクセスしてログイン
![LINE Developers](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LineBotBasicCourse/LineBotBasicScenario/images/LINEDevelopers.png)


## 3-2. プロバイダーを選択

 Bot を作ったときと同じプロバイダーを選択
 
![プロバイダー選択](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/provider_LINE_Developers.png)

## 3-3. LIFF 用のチャネルを作成

チャネルを作成
![チャネル作成](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/loginchannel_LINE_Developers.png)

「LINE ログイン」 を選択

![LINE ログイン](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LiffKintoneQuestionaryCourse/SetupBotAndLiff/images/SelectLineLogin.png)

チャネル情報を入力して、「入力内容を確認する」ボタンを押下する

### チャネル情報の入力例

|  項目名  |  値  |
| :-- | :-- |
|  チャネル名  |  テイクアウトアプリ  |
|  チャネル説明  |  LINE × kintone × Azure AIでテイクアウトアプリを作ってみよう！  |
|  アプリタイプ  |  ウェブアプリ  |
|  メールアドレス  |  （ご自分のメールアドレス）  |
|  プライバシーポリシーURL  |  （入力不要）  |
|  サービス利用規約URL  |  （入力不要）  |


![チャネルの情報を入力](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/input_LINE_Developers.png)

規約に同意してチャネルを作成する

![規約に同意](https://raw.githubusercontent.com/sumihiro3/katacoda-scenarios/master/LiffKintoneQuestionaryCourse/SetupBotAndLiff/images/AgreeTerms.png)

## 3-4. LIFF アプリを追加する

「LIFF」タブを選択して、LIFF アプリを追加する

![LIFF アプリを追加](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/liff_LINE_Developers.png)

LIFF アプリ基本情報を入力して、「追加」ボタンを押下する

### LIFF アプリ基本情報の入力例

|  項目名  |  値  |
| :-- | :-- |
|  LIFFアプリ名  |  商品の準備状況  |
|  サイズ  |  Full  |
|  エンドポイントURL（この時点ではダミー）  |  https://www.google.com  |
|  Scope  |  profile, openid, chat_message.write  |
|  ボットリンク機能  |  On (Aggressive)  |

![基本情報を入力](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/inputdetail_LINE_Developers.png)

LIFF アプリが追加されたことを確認する

![LIFFアプリ追加](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/addliff_LINE_Developers.png)

「LIFF URL」をメモしておく

![LIFF URL](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/liffurl_LINE_Developers.png)


## 3-5. LINE ログインチャネルを公開する

画面上部の「非公開」をチェックして公開する

![公開する](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/open_LINE_Developers.png)

「公開済み」となっていればOK

![公開済み](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/opencheck_LINE_Developers.png)

### お疲れ様でした
### 次は、kintone のアプリ作成です！