## この教材について

この教材はLINE とkintone、そしてAzure AI を使ったテイクアウトアプリを開発するハンズオンで使用します。

## シナリオについて

このシナリオではAzure AI の紹介と設定を行います。

## Azure Cognitive Services とは？

Azure Cognitive Services は、開発者が直接的な AI またはデータ サイエンスのスキルや知識がなくてもインテリジェントなアプリケーションを構築するために使用できる API、SDK、およびサービスです。 Azure Cognitive Services によって、開発者は簡単にアプリケーションに Cognitive 機能を追加できます。 Azure Cognitive Services の目標は、開発者が、聞いたり、話したり、理解したり、推論し始めたりできるアプリケーションの作成を支援することです。 Azure Cognitive Services 内のサービス カタログは、5 つの主要な柱として、視覚、音声、言語、Web 検索、および意思決定に分類できます。（[引用元](https://docs.microsoft.com/ja-jp/azure/cognitive-services/welcome)）

![AzureCognitiveServicesとは？](https://image.slidesharecdn.com/20170805cntkhandsonmsai-170805043722/95/microsoft-cognitive-toolkit-cntk-on-azure-microsoft-azure-ai-15-638.jpg?cb=1502010994)
([画像引用元](https://www.slideshare.net/satonaoki/20170805cntkhandsonmsai))

本日のハンズオンでは、このAzure Cognitive Services を使って、より便利なテイクアウトアプリを作ります。

## 本日のハンズオンで使う2つのAPI

![問い合わせ管理_-_Records.png](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/【テイクアウト】問い合わせ管理_-_Records.png)

### Translator API
ユーザーが送信したお問い合わせ内容を日本語に翻訳するために、Translator API を利用します。
Translator API は、60を超える言語間のテキストからテキストへの翻訳をサポートしています。

### Text Analytics API
ユーザーが送信したお問い合わせ内容を感情分析するために、Text Analytics API を利用します。
Text Analytics API は、未加工のテキストに対して高度な自然言語処理を実行できるクラウドベースのサービスであり、主要な機能として感情分析、キーフレーズ抽出、言語検出、名前付きエンティティの認識の4つを備えています。


これらのAPIを利用するためにアクセスキーが必要となります。

START SCENARIO ボタンを押して、アクセスキー取得の手順を確認しましょう！
