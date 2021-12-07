<!-- pdf化用 -->
<link href="./css/document.css" rel="stylesheet"></link>

# Curriculum Vitae

## 基本情報

key|value
--|--
名前|木戸 康介
出身|大阪府

## 近況

2018年7月Arithmerに入社。

### 2018年7月〜 OCR開発チーム

入社後Python,OpenCV,Kerasで免許証OCRを実装。CNNベースでパラメータの調整や学習データの調整を実施。2018年10月から免許証OCRのAndroidライブラリを開発担当(Android Studio, Kotlin, OpenCV, TensorFlow Lite)し、PC、Pythonで使用していたモデルをモバイル向けにTensorFlow Liteへコンバート、前後処理をポーティング。  
モバイル向けのポーティングにあたり、モデルの一部にモバイルでは実現が難しい構造があり、代替となる構造を検討、評価して一定の精度が出せることを確認、ポーティングを実施。

その他、以下のような事も実施。

- PC上で作成していたOCRプログラムから派生した、AWSのSQS、S3と組み合わせて、常駐してポーリングでOCRを実施するDockerイメージの作成
- GCPのDataflowでOCRをバッチ処理する実験
- オンプレ提供用OCR学習プログラム、推論プログラムの開発

### 2020年12月〜 スクラムマスター

2020年4月から同じくOCR開発チームにて自社Webサービスのスクラムマスター兼開発者。自身を含めた全メンバーがスクラム未経験、社内では初のスクラム開発を実施。スクラム開発の浸透のため読書会を実施。
VSCode, Remote Containerを用いて標準の開発環境を整備。マイクロサービス化を提案して各処理をAPI化して開発。

### 2021年2月〜 SREチーム

主にterraform, Github Actions, ArgoCDなどを用いてGCP上での環境構築や、GCPサービスを用いた監視など。チーム内でサービスの構築方法やレポジトリの構造の共通化活動なども実施。また、ソフトウェア品質向上ワーキンググループのメンバーに選出され、開発プロセスの改善などに取り組み。2021年12月から本ワーキンググループをリードするように任命される。

## 学歴・職歴

年月|学歴・職歴|備考  
--|--|--
2021/02〜|Arithmer株式会社 SRE Team|現職 主にGCP周り
2018/07〜|Arithmer株式会社 OCR開発|OCRアプリケーションの研究開発
2012/04〜2018/06|三菱重工業株式会社（中略）ソフトウェア設計課|自社製品の組み込みソフトウェア開発
2010/04〜2012/03|神戸大学 システム情報学研究科計算科学専攻|上肢リハビリテーション用ロボットの制御則
2006/04〜2010/03|神戸大学 工学部情報知能工学科|知能ロボティクス研究室
2003/04〜2006/03|大阪府立富田林高校|

## 資格

取得年月|資格名
--|--
2019/12|Professional Cloud Developer (GCP)
2019/10|Professional Cloud Architect (GCP)
2019/08|Professional Data Engineer (GCP)
2017/11|基本情報技術者
2017/07|TOEIC820
2017/07|IELTS academic Overall:6.0<br>Listening:5.5 Reading:6.5 Writing:5.5 Speaking:5.5

## 技術スタック

### スキルレベル定義

レベル|定義
--|--
7|自分でもっといいもの作れるのではないかと思うレベル
6|githubでプルリク投げたりissue投げて指摘できるレベル。
5|指導できるレベル。公式ドキュメント等どこを見ればいいか、調べ方をほとんど理解している。
4|たまに参考を見ながら独力でできるレベル。公式ドキュメント等どこを見ればいいか、調べ方をなんとなく理解している。
3|調べながら独力でできるレベル。公式ドキュメントや個人ブログを辿りながら作業をしたことがある。
2|少し触ったことがあるレベル。簡単に実装をしたことがある。
1|概要を知っているレベル。本を読んだ、チュートリアルで触れた程度

基本的に評価レベルは１〜５想定。

### インフラ周辺技術

名称|経験年数|レベル|備考
--|--|--|--
Docker|3年|3|開発環境イメージ、本番イメージ、ちょっとしたバッチ処理など
GitlabCI|3ヶ月|3|自動難読化・デプロイに使用、Slackとの連携も。
Github Actions|1年|4|基本的な実装なら可能。push時のテスト実行、イメージのビルド、クラウドサービスのデプロイ、Slack通知など。
DGX Station|1ヶ月|1|前任者がRancher等でクラスタ構築し、jobを投げれるようにしてあるものを引き継いだ。
Terraform|1年|4|主に環境の構築|
Argo CD|1年|3|Github Actions、GKEと組み合わせ|

### クラウド技術

#### GCP

名称|経験年数|レベル|備考
--|--|--|--
GCE|-|2|社内リソース不足時の学習用マシンとして
GKE|-|3|既に構築済みのプロジェクトでデバッグのためのログの確認やPodの状態確認など。Cloud Endpointなど組み合わせて社内用webチュートリアル作成。
GCS|-|3|Webサービスのストレージとして
Dataflow|-|2|OCRをバッチ処理化して動かしてみた
Firestore|-|3|WebサービスのDBとして
VPC, PubSub, Cloud Endpoints, Cloud Functions, GAE, BigQuery, StackDriver, Firebase Authentication|-|1|資格取得時のQwiklabsのハンズオン等で触った程度

### 言語

名称|経験年数|レベル|備考
--|--|--|--
Python|3年|4|バックエンドやAIの学習など。
Kotlin|2年|4|Android用のライブラリ（AAR）開発のメイン言語
JavaScript|1年|3|Reactで自社製品のfront-end開発
Java|3年|3|Android用ライブラリ（AAR）開発、学生時代の演習
C|6年|3|組み込みプログラム開発, Texas Instruments
Ruby|3ヶ月|2|単純業務のスクリプト化など
Julia|1ヶ月|2|バックエンドの高速化に一部使用

### フレームワーク・ライブラリ

名称|経験年数|レベル|備考
--|--|--|--
TensorFlow, Keras|3年|3|社内の既存のモデルのパラメータ調整、学習、評価など
OpenCV|3年|3|前処理などで使用。
numpy|3年|3|TensorFlowと組み合わせて。
pandas|3ヶ月|3|アプリケーションの一部に使用。データサイエンティスト100本ノックなど実施。
Flask|3ヶ月|3|実験としてOCRアプリケーションをAPI化してみた。製品開発の一部にも使用。
FastAPI|3ヶ月|2|社内用webチュートリアル作成に使用
React|6ヶ月|3|自社製品のfront-end開発

### 開発ツール

名称|経験年数|レベル|備考
--|--|--|--
Git|3年|4|
Github|2年|3|Github Actionsによる自動テストやSlack通知なども。
Gitlab|1.5年|3|Gitlab CIも多少。
Slack|3年|-|GithubやGitlabでのCI、運用でのWebhook連携等も行ったことあり。
Redmine|3年|-|Agile plugin使用。
Visual Studio Code|3年|4|Remote Containers, Remote SSH, Poetry等を用いてチームでの開発環境統一など。

### その他

#### 組織改善

- 運用・保守のガイドライン策定（メンバー）
- Redmineの運用フロー策定（メンバー）
- スクラム開発の提案、実施（スクラムマスター）

## 主な担当プロジェクト

### DXプロジェクト

#### 期間

- 開発：2021/02〜2021/12
- 運用：2021/12〜

#### プロジェクト概要

スマホアプリを通じて洋服販売店の顧客へのリコメンド通知などを実施するシステムの開発。スマホアプリはパートナーの開発、自社ではスマホアプリから呼び出されるAPIなどを開発。

#### 担当

クラウド基盤整備、CI/CD構築、運用

#### 内容

- terraformによる基盤構築
- Github Actions、ArgoCDなどによるCI/CDの構築
- アプリケーション開発者と協調して開発やトラブルシュートなど
- パフォーマンスの計測、改善

#### 担当フェーズ

フェーズ|担当
--|--
要件定義|×
基本設計|〇
詳細設計|〇
実装/単体テスト|〇
結合テスト|〇
総合テスト|〇
運用/保守|〇(予定)

#### 開発規模

- チーム: 約10人

#### 備考

- CI/CDについて開発メンバーに共有し、効率的な開発を目指す
- できるだけ一つのレポジトリで完結する構成を検討

### OCR開発A

#### 期間

- 開発：2020/04～2020/12

#### プロジェクト概要

書類等のOCR領域などの定義と設定をユーザーに行ってもらい、OCRするSaaSの開発

#### 担当

スクラムマスター
開発：主にアプリケーション、フロントエンド

#### 内容

- マイクロサービスの提案
- マイクロサービス開発のためのスケルトンプロジェクト（各APIを開発する際にベースとして使えるリポジトリ）の整備を提案
- Visual Studio Code, RemoteContainerで標準開発環境の整備
- アプリケーションプログラムの開発
- フロントエンド開発
- SREを主担当とする他のメンバと協調してGCP上にデプロイした環境でのトラブルシュート

#### 担当フェーズ

フェーズ|担当
--|--
要件定義|〇
基本設計|〇
詳細設計|〇
実装/単体テスト|〇
結合テスト|〇
総合テスト|〇
運用/保守|〇(予定)

#### 開発規模

- チーム: 6人

#### 備考

- 追加学習や機能追加もできるような設計を意識
- フロントエンド要員が足りなかったため、途中からフロントエンドも覚えながら開発

### OCR開発B

#### 期間

- 開発：2018/07～
- 運用：2019/06～

#### プロジェクト概要

特定の書類をOCRを実施する製品群の開発

#### 担当

プログラム開発

#### 内容

- OCRモデル
  - ネットワーク検討、パラメータ調整
  - 学習データ検討、収集
  - モバイルへポーティングの際のネットワーク検討
- PC、Pythonでの開発
  - ターミナルから実行するバッチ用プログラム
  - Web APIで実行する常駐用プログラム
- Android用ライブラリ（AAR）
  - PCからポーティング、モデルのコンバート
- ライセンスの発行
- 導入手順等のマニュアル作成
- 運用保守は主に問合せ対応と機能追加対応

#### 担当フェーズ

フェーズ|担当
--|--
要件定義|×
基本設計|〇
詳細設計|〇
実装/単体テスト|〇
結合テスト|〇
総合テスト|×
運用/保守|〇

#### 開発規模

- チーム: 4人

#### 備考

- Androidで模擬アプリケーションも作成
- モバイル特有の問題も意識しながら開発

### 組み込み制御プログラム開発 (前職)

#### 期間

- 開発：2012/07～2018/06

#### プロジェクト概要

自社製品に組み込まれて製品を制御するためのプログラム開発

#### 担当

プログラム開発

#### 内容

- 上流設計課との要求仕様の調整（問題点の指摘、代替案の提案）
- プログラム基本設計〜実機同等回路での試験まで
- 後工程での試験のトラブル発生時の問い合わせ対応、トラブルシュート

#### 担当フェーズ

フェーズ|担当
--|--
要件定義|×
基本設計|〇
詳細設計|〇
実装/単体テスト|〇
結合テスト|〇
総合テスト|×
運用/保守|×

#### 開発規模

- チーム: 1〜3人

#### 備考

- 全工程ほぼ一人での実施経験あり
- 名指しでトラブルシュート支援要請があり、解決・代替案の策定に至った件数複数あり
