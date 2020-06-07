## この教材について

この教材はLINE とkintone、そしてAzure AI を使ったテイクアウトアプリを開発するハンズオンで使用します。

## シナリオについて

このシナリオではAzure AI の紹介と設定を行います。

## Azure Cognitive Services とは？

![画像]()

Azure Cognitive Services は、開発者が直接的な AI またはデータ サイエンスのスキルや知識がなくてもインテリジェントなアプリケーションを構築するために使用できる API、SDK、およびサービスです。 Azure Cognitive Services によって、開発者は簡単にアプリケーションに Cognitive 機能を追加できます。 Azure Cognitive Services の目標は、開発者が、聞いたり、話したり、理解したり、推論し始めたりできるアプリケーションの作成を支援することです。 Azure Cognitive Services 内のサービス カタログは、5 つの主要な柱として、視覚、音声、言語、Web 検索、および意思決定に分類できます。

このAzure Cognitive Services を使って、より便利なテイクアウトアプリを作ります。

## 今回使う2つのAPI

今日作るアプリではユーザーからの問い合わせに対してAzure AIを使うことで、翻訳と優先度付けを行っています。

ユーザーが送信したお問い合わせ内容を翻訳するために、Translator API を利用します。
Text Translatorサービスは、60を超える言語間のテキストからテキストへの翻訳をサポートしています。

問い合わせ内容の感情分析には、Text Analytics API を利用します。
Text Analytics API は、未加工のテキストに対して高度な自然言語処理を実行できるクラウドベースのサービスであり、主要な機能として感情分析、キー フレーズ抽出、言語検出、名前付きエンティティの認識の 4 つを備えています。
Text Analytics API は、テキストからの情報の抽出に役立つように設計された Cognitive Service です。 このサービスを使用して、言語の特定、センチメントの検出、キー フレーズの抽出、テキストからの既知のエンティティの検出を行うことができます。

![システム構成](https://raw.githubusercontent.com/torisankanasan/katacoda-scenarios/master/SetupAzureAI/images/handson_sysytem_archtecture.png)

これらのAPIを利用するためにアクセスキーが必要となります。

START SCENARIO ボタンを押して、アクセスキー取得の手順を確認しましょう！
