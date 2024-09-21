# 職務経歴書

## 基本情報

|Key|Value|
|---|---|
|氏名|鎌田 均（Hitoshi KAMADA）|
|生年月日|1992年2月26日|
|居住地|千葉県|
|最終学歴|愛知工業大学 情報科学部 情報科学科 メディア情報専攻|

## 各種アカウント

- Qiita : <https://qiita.com/hiesiea>
- Zenn : <https://zenn.dev/kmd_htsh0226>
- note : <https://note.com/kmd_htsh/>
- Speaker Deck : <https://speakerdeck.com/kmd_htsh0226>
- X : <https://x.com/kmd_htsh0226>
- Lapras : <https://lapras.com/public/PQIRUSU>

## スキルセット

### 強み

- Kotlin, Java, Flutter による Android アプリ開発および設計
- レガシーコードのリファクタリングおよびリプレイス
- アジャイル、スクラムによるチーム開発
- Android アプリ開発におけるテックリード
- プログラミング講師（Java, Android）

### 主な使用可能言語

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=hiesiea&layout=compact)](https://github.com/anuraghazra/github-readme-stats)

### 主な使用可能フレームワーク・ライブラリ等

Android Jetpack(Jetpack Compose, Navigation, Room, Hilt, WorkManager, DataStore, Media3), RxJava 3, Kotlin Coroutines, Kotlin Flow, OkHttp3, Retrofit2, Moshi, Glide, JUnit, Mockito, Flutter

## 職務経歴詳細

### 2019年4月〜現在 フリーランス

#### 2021年3月〜現在 ZEN Study（旧：N 予備校）開発支援業務

- 概要：ZEN Study（旧：N 予備校）Android アプリの開発支援業務
- 担当工程：要件定義、設計、コーディング、テスト、運用/保守
- 役割：当初は SE として参画、2023 年よりテックリード
- 規模：6 名（PM1 名、PL1 名、SE4 名）

##### 開発環境

- 言語：Kotlin, Markdown
- OS・DB：Android, Mac OS
- ライブラリ・フレームワーク：Android Jetpack(Jetpack Compose, Navigation, Media3, DataStore), Glide, Coil, Sentry, Firebase(Analytics, Messaging, Crashlytics, Remote Config), OkHttp3, Retrofit2, JUnit, kotlin.test, Mockito, Timber, Kotlin Coroutines, Kotlin Flow, ExoPlayer, RxJava 3, Version Catalog, Composite Build
- ツール：Android Studio, JIRA, Slack, Confluence, GitHub, Figma, avocado

##### 業務内容

- 機能追加、不具合改修
  - 接続先サーバの移行対応
- リファクタリング
  - Deprecated な処理の警告解消
  - ListView を RecyclerView に移行
  - View Binding の導入
  - ViewPager を ViewPager2 に移行
  - 画面遷移を Navigation に移行
  - Single アクティビティ に移行
  - UI を Jetpack Compose に移行、UI テストの導入
    - 影響範囲を限定するため、あまり使われていなく、ユーザへの影響が少なそうな画面から徐々に Compose 化した
  - マルチモジュールの導入
  - 通信処理を Retrofit に移行
  - JSON ライブラリを Moshi に一本化
    - org.json と Gson がごちゃ混ぜになっていたが、通信処理を Retrofit に移行した際、JSON パーサーとして Moshi を使用していたため、あわせて Moshi に一本化した
  - Serializable なデータクラスを Parcelable に移行
  - RxJava 3 から Kotlin Flow に移行
  - buildSrc から Composite Build に移行
- テックリードとしてチームメンバーのマネジメント
  - 新技術導入に向けた調査、ドキュメント作成および共有
  - タスクの作成、チームメンバーへの割り振り
  - リファクタリングタスクの工数見積もり、計画
  - Codelab にて学習コンテンツの選定
  - リファクタリングの取り組みを記事化
  - コードレビュー
  - GitHub のプルリクエストのテンプレート改善
- DroidKaigi への参加

#### 2020年6月〜2021年2月 屋外広告配信システム開発案件

- 概要：Windows および Android 向けの屋外広告配信システム開発案件
- 担当工程：要件定義、設計、コーディング、テスト、運用/保守
- 役割：SE
- 規模：6 名（PM1 名、PL1 名、SE4 名）

##### 開発環境

- 言語：Kotlin, C#
- OS・DB：Android, Windows, Mac OS, SQLite
- ライブラリ・フレームワーク：、Android Jetpack, OkHttp, Retrofit, JUnit, MockK, Timber, Kotlin Coroutines, WPF, UWP, Prism, RestSharp, EF Core、.NET Core, NLog, msix
- ツール：Android Studio, Visual Studio, JIRA, GitLab, GitHub, Slack, zoom, VS Code, LucidChart, Postman, Mmock, Docker, Confluence

##### 業務内容

- 主に Android アプリの機能追加、不具合改修、リリース作業を担当
  - 異常報告機能の過剰報告の抑止対応
  - Web ページ表示機能の実装
  - 広告の分割表示機能の実装
  - 他社向けへの新規アプリ追加
  - その他バグ調査、修正を担当
- 今後の機能追加のため、Android Jetpack を活用してのリプレイス対応
  - 公式ホームページのアプリアーキテクチャガイドをベースに MVVM アーキテクチャを採用
  - Room, Retrofit(OkHttp)を利用しての Repository クラスの実装
  - Kotlin Coroutines による非同期処理の実装
  - ViewModel, LiveData, DataBinding による View と ViewModel の連携
  - Hilt による DI の導入
  - JUnit, MockK によるテストコードの実装
  - グローバル変数、メソッドの排除
  - 複雑化していたロジックのシンプル化
  - 映像切り替え時のパフォーマンスチューニングを実施
  - Postman, Mmock, Docker によるモックサーバの構築
  - ビルドバリアントの整理
- Windows アプリの新規開発にあたっての技術選定
  - WPF, UWP などの各種プラットフォームの概要調査
  - ビジネスサイドとの機能要件、非機能要件の認識合わせおよび整理
  - 各機能要件、非機能要件についてサンプルアプリを作成しながらの技術検証
- 開発に関する問題改善のための提案および実施
  - 各社ごとの機能要望の整理ができていなかったのを指摘および整理
  - アプリのパッケージ化の検討
  - 開発体制やビジネスサイドとの進め方について見直しの提案
- チームメンバーの技術教育
  - 新人向けに開発ルールなどのドキュメント作成
  - コードレビュー、設計レビュー

#### 2020年2月〜2020年5月 バイトルApp機能拡張開発

- 概要：バイトルアプリ（Android・iOS）の追加開発・改修
- 担当工程：要件定義、設計、コーディング、テスト、運用/保守
- 役割：SE
- 規模：11〜50 名

##### 開発環境

- 言語：Java, Kotlin, Swift, Markdown
- OS・DB：Android, iOS, Mac OS, SQLite, Realm
- ライブラリ・フレームワーク：Retrofit, Swagger, Maps SDK for Android, Adobe Target
- ツール：Android Studio, Xcode, Redmine, Backlog, GitHub, VS Code, PlantUML, Postman, Mmock, ngrok, Toggl, DocBase, Bitrise, VS App Center, Slack

##### 業務内容

- コードレビュー
- AB テスト取込
  - AB テストの結果を機能概要書、ソースコードに反映
  - 単体、結合試験書の作成および実施
- 地図検索機能の開発
  - API チームとの仕様確認および調整
  - Maps SDK for Android の調査および DocBase への情報共有
  - 機能概要書の作成
  - プロトタイプ作成
  - 要求元チームとの要求仕様の確認および整理
- リリースに向けたブランチのマージ作業
- モックサーバの立て方について DocBase への情報共有
- バグ解析、調査

#### 2019年7月〜2020年1月 モバイルアプリの追加開発・改修

- 概要：格安 SIM を提供している会社様向けに、契約者のご利用状況などを確認できるスマホアプリの追加開発・改修
- 担当工程：要件定義、設計、コーディング、テスト
- 役割：開発メンバー
- 規模：6 名（プロダクトオーナー1 名、スクラムマスタ 1 名、開発メンバー4 名）

##### 開発環境

- 言語：Dart, Kotlin, Markdown, Swift
- OS・DB：Android, iOS, Mac OS, SQLite
- ライブラリ・フレームワーク：Flutter, Appium, Swagger, FCM, Mockito, Notification Hubs
- ツール：Azure DevOps, Git, Backlog, Toggl, Mmock, Docker, Typora, ngrok, Xcode, zoom, VS Code, Slack, Android Studio

##### 業務内容

- スクラム開発、1 週間スプリントによるイテレーション
- 開発メンバーとして、フロントエンドの要件定義、設計、実装、テストを担当
  - 設計に関しては、Markdown によるドキュメント作成および、元々 Excel で記載されていた設計書を Markdown 形式への移行作業も担当
  - UI に関してはマテリアルデザインをベースに設計
  - アーキテクチャは BLoC パターンを採用
  - プッシュ通知（Notification Hubs）の改修に関しては、ネイティブ側（Android）の実装を Kotlin で行った
  - テストに関しては、ロジック部分を Mockito でユニットテストを実装
  - Mmock と Docker によるモックサーバの構築および、YAML でのモックデータ作成を担当
  - Android 10 に関する調査およびリリース対応
  - 64bit 対応に関する調査およびリリース対応
  - Azure Pipelines による CI 環境の構築。ビルドおよびテスト実行結果を Slack へ通知する仕組みを実現
  - UI テストの自動化のための Appium の調査、Appium Desktop に接続するまでの環境構築、JavaScript によるテストコードのプロトタイプ作成
- iOS 版の開発にあたり、差分で開発する必要がある箇所について洗い出し、および iOS 版でどのように実現するかの調査および実装
  - プッシュ通知、データ暗号化、ユーザ認証の実現方法の調査および開発環境準備、データ暗号化の実装、ユーザ認証のプロトタイプ作成

#### 2019年4月〜2019年10月 Android TV お手続き資料請求アプリおよび、請求確認アプリの新規開発

- 概要：Android TV 搭載の STB 向けのプリインアプリの新規開発
  - テレビプランや各種サービスへのお手続き資料請求アプリ
  - 加入中のプランなどの料金詳細が確認できる請求確認アプリ
- 担当工程：要件定義、設計、コーディング、テスト
- 役割：開発メンバー
- 規模：7 名（プロダクトオーナー1 名、スクラムマスタ 1 名、開発メンバー5 名）

##### 開発環境

- 言語：Kotlin, Markdown, shell script, YAML
- OS・DB：Android TV, Mac OS, SQLite
- ライブラリ・フレームワーク：Kotlin Coroutines, Swagger, Timber, Leanback, Data Binding, Glide
- ツール：Android Studio, Azure DevOps, Backlog, Git, Toggl, zoom, miro, Docker, Slack, VS Code, Mmock

##### 業務内容

- スクラム開発、1 週間スプリントによるイテレーション
- 開発メンバーとして、フロントエンドの要件定義、設計、実装、テストを担当
  - 設計に関しては、Markdown によるドキュメント作成
  - UI に関してはマテリアルデザインをベースに設計
  - 実装に関しては、言語は Kotlin、アーキテクチャは MVVM パターンを採用
  - テストに関しては、ロジック部分を Kotlin でユニットテストを実装。また、Mmock と Docker によるモックサーバの構築および、YAML でのモック作成も担当
- お手続き資料請求アプリ、請求確認アプリそれぞれの共通処理を Git submodule で別リポジトリとして分割

### 2015年10月〜2019年3月 株式会社ASCOM

#### 2018年8月〜2019年1月 IPTV の Android FW 標準化検討

- 概要：MMT(MPEG Media Transport) を Android 上で実現するための検討および調査
- 担当工程：要件定義
- 役割：SE
- 規模：6〜10 名

##### 開発環境

- 言語：Java
- OS・DB：Android TV, Ubuntu, Windows
- ライブラリ・フレームワーク：Android SDK, ExoPlayer
- ツール：Android Studio, GitHub, Backlog, Redmine, Wireshark, tcpreplay

##### 業務内容

- MediaCas、MediaDescrambler、MediaCodec クラスに関するドキュメント調査、シーケンス図の作成
- マルチキャスト構成の調査と、配信ツールの比較選定、資料作成
- MMT(MPEG Media Transport)や、コーデックに関する調査
  - パケット構成の調査と、Reader と Demuxer の実装
  - ARIB、ISO 規格との差分調査、資料作成
- コードレビュー、メンバーが作成した資料のレビュー

#### 2017年12月〜2018年3月 ペット心電図アプリ開発

- 概要：ペット用の心電図アプリの開発
- 担当工程：実装、テスト
- 役割：PG
- 規模：1〜5 名

##### 開発環境

- 言語：C#, JavaScript, HTML
- OS・DB：Windows
- ライブラリ・フレームワーク：i18next, Windows Form
- ツール：Redmine, Git, Visual Studio 2017

##### 業務内容

- バグ修正
  - 環境による UI くずれの修正
  - 計測結果表示バグの修正
- エンドユーザ様との合同デバッグ
- i18next による多言語化対応

#### 2017年11月〜2019年3月 Android TV 衛星放送プレイヤーの追加開発・改修

- 概要：Androit TV 搭載の STB 専用の、IPTV アプリの衛星放送プレイヤー部分の追加開発・改修
- 担当工程：設計、コーディング、テスト、運用/保守
- 役割：SE
- 規模：5 名（PM1 名、PL1 名、SE3 名）

##### 開発環境

- 言語：Java
- OS・DB：Android TV, Windows
- ライブラリ・フレームワーク：Android SDK, OkHttp、Volley, ExoPlayer
- ツール：Android Studio, Subversion, Redmine, Wireshark

##### 業務内容

- ザッピング機能の詳細設計、実装、結合試験、総合試験の実施、リリース作業を担当
  - 設計に関しては、シーケンス図作成と Word による仕様書の修正
  - 実装は Java で、リモコンのキーイベント制御の実装
- 不具合解析および改修。不具合解析のため、Wireshark によるパケット解析の実施。API との疎通確認や、ルータとの IGMP パケットの疎通確認などを実施
- Volley から別の通信ライブラリへの置き換えのため、通信ライブラリの比較選定および、実際に置き換えての動作検証
- Android Oreo へのアップデート対応。具体的には、新機能に関する調査、非推奨 API となった API の置き換えを実施

#### 2017年11月〜2018年5月 スマートスピーカー検討

- 概要：スマートスピーカーと STB の連携方法に関する調査・検討
- 担当工程：要件定義
- 役割：SE
- 規模：1〜5 名

##### 開発環境

- 言語：JavaScript, HTML, CSS
- OS・DB：Windows, SQLite
- ライブラリ・フレームワーク：Node.js, JQuery, Bootstrap
- ツール：ngrok, Redmine, Dialogflow, Alexa Skills Kit, IFTTT, Git, Actions on Google, Node-RED

##### 業務内容

- スマートスピーカー(Google Home、Amazon Echo)に関する調査
  - アプリのシーケンス図の作成
  - 各スマートスピーカーの機能一覧および比較表の作成
- STB 連携に関する調査検討
  - 各スマートスピーカーのサンプルアプリの作成
  - 調査報告書の作成
  - 客先での打ち合わせ、デモ実施

#### 2017年10月〜2017年11月 社内新人研修

- 概要：新入社員向けのプログラミング研修
- 役割：講師
- 規模：11〜20 名

##### 開発環境

- 言語：Java, C#
- OS・DB：Windows, Mac
- ツール：GitHub

##### 業務内容

- スケジュール、カリキュラム作成
  - 2 か月間、1 日 8 時間のスケジュール作成、各日の到達目標設定
- 研修内で作成したアプリの評価
- コードレビュー、設計書レビュー
- 新人へのマネジメント、進捗管理

#### 2017年4月〜2017年9月 Android 搭載 の IoT デバイスの新規開発

- 概要：Android 搭載の非接触センサー付 IoT デバイスの新規開発
- 担当工程：設計、コーディング、テスト
- 役割：PG
- 規模：31 名（PM1 名、PL5 名、SE・PG15 名、テスター10 名）
  - 各機能ごとでチームに分かれ、各チームに PL1 名、SE・PG1〜3 名の構成 テストチームに関しては PL1 名、テスター
10 名の構成

##### 開発環境

- 言語：Java
- OS・DB：Android, Windows, Ubuntu, SQLite
- ライブラリ・フレームワーク：Andorid SDK, Javadoc
- ツール：Android Studio, JIRA, Redmine, Gerrit, Repo, Git, Mattermost

##### 業務内容

- スマホアプリ側に提供する I/F 仕様書作成（Javadoc）および、Service コンポーネントを利用した IoT デバイス側の実装、結合試験書の作成および実施を担当
  - 実装として、IoT デバイスが収集したデータを分析して DB に格納し、定期的に DB データをバイナリデータ化して ZIP 圧縮してサーバに送信する処理の実装を担当
  - 結合試験書の作成では、2 機能分で項目数 400 項目弱の項目の洗い出しを行った

#### 2016年10月〜2017年3月 Android 搭載のコミュニケーションロボットの新規開発

- 概要：Android 搭載の音声認識、顔認識によるコミュニケーションロボットの新規開発
- 担当工程：要件定義、設計、コーディング、テスト
- 役割：SE
- 規模：12 名（マネージャー1 名、デザイナー1 名、SE10 名）

##### 開発環境

- 言語：Java
- OS・DB：Android, Windows
- ライブラリ・フレームワーク：Android SDK, Data Binding, JUnit, AssertJ
- ツール：Android Studio, JIRA, GitHub, Checkstyle, FindBugs, astah, Coverity, Jenkins

##### 業務内容

- アジャイル開発、2 週間スプリントによるイテレーション
- 要件定義書の作成、astah によるクラス図作成、Java によるフロントエンドの実装、JUnit による内部ロジックのテストコードの実装を担当
  - フロントエンドの実装として、正規表現によるパラフレーズ対応、UI ロジックおよび UI の実装を担当
- 音声認識率の低下の問題が発生したため、場所を変えての環境音の収集、および動作時の認識率といった、原因の調査に必要なデータの収集

#### 2016年5月〜2016年8月 大手物流企業向け宅配管理システム開発

- 概要：大手物流企業向けの宅配管理を行うための Andorid アプリの開発
- 担当工程：設計、コーディング
- 役割：SE
- 規模：11〜50 名

##### 開発環境

- 言語：Java
- OS・DB：Android, Windows, SQLite
- ライブラリ・フレームワーク：Android SDK
- ツール：Eclipse, Redmine, JIRA, CAT, TortoiseSVN

##### 業務内容

- ソースコードの解析および詳細設計書の修正といったリバースエンジニアリング対応
- 他機能との連携処理の設計〜実装、設計案の検討および、エンドユーザへの提案
- 新規参入者への引き継ぎ作業

#### 2016年4月〜2016年5月 社外研修

- 概要：若者正社員チャレンジ事業で受け入れたインターン生向けのプログラミング講習（Android アプリ開発）の実施
- 役割：講師
- 規模：6〜10 名

##### 開発環境

- 言語：Java, Markdown
- OS・DB：Android, Mac OS
- ライブラリ・フレームワーク：Android SDK
- ツール：Android Studio, GitHub, Qiita

##### 業務内容

- 15 日間、1 日 8 時間のスケジュールおよびカリキュラムの作成、各日の到達目標設定
- Qiita での教材作成
- 当日のメイン講師

#### 2015年10月〜2016年3月 iOS・Android 向け観光支援スマホゲームアプリの新規開発

- 概要：iOS、Android 向けの地方観光支援のためのスマホゲームアプリの新規開発
- 担当工程：コーディング、テスト
- 役割：SE
- 規模：6〜10 名

##### 開発環境

- 言語：C#, JavaScript
- OS・DB：Android, iOS, Windows, Mac OS
- ライブラリ・フレームワーク：d3.js, Cardboard SDK, Joker Script
- ツール：Unity, Backlog, TortoiseSVN, Xcode

##### 業務内容

- アプリのフロントエンド全ての実装および、ライブラリやフレームワーク等の選定を担当
  - フロントエンドの実装として、uGUI を用いた各画面の UI、画面遷移処理の実装
  - iTween による画面タッチ時のエフェクト等のアニメーション実装
  - Joker Script を用いたアドベンチャー（ノベル形式）モードの実装
  - Cardboard SDK を用いた VR 機能の実装
  - d3.js を用いた画像プレビュー機能の実装
- Google Play および App Store へのリリース作業
  - リリースにあたって無駄なリソースの削除
  - apk ファイルや ipa ファイルの書き出し及び署名実施
  - プロビジョニングプロファイルの作成、ストアへの提出
  - リジェクト対応

### 2014年4月〜2015年8月 株式会社ケイ・アイ・テック

#### 2015年4月〜2015年8月 収納家具見積 Web システムの新規開発

- 概要：収納家具のレイアウトを作図し、作図内容をもとに見積もり金額を算出するための Web システム
- 担当工程：コーディング、テスト
- 役割：PG
- 規模：6〜10 名

##### 開発環境

- 言語：Java
- OS・DB：Windows
- ライブラリ・フレームワーク：Jakarta Tomcat, Swing
- ツール：Eclipse, GitHub, Redmine, SQL Server, Sourcetree

##### 業務内容

- Swing を用いた 画面 UI の実装
  - 全体的な画面構成、画面遷移の実装
  - 社内の独自ライブラリを用いた家具の設置、移動などの制御実装
  - XML 形式でのデータ保存機能の実装

#### 2014年7月〜2015年3月 プレゼンボード作成 Web システムの新規開発

- 概要：プレゼンボードやチラシを作成するための Web システム
- 担当工程：コーディング、テスト
- 役割：PG
- 規模：6〜10 名

##### 開発環境

- 言語：Java, HTML, JavaScript
- OS・DB：Windows, MySQL
- ライブラリ・フレームワーク：PDFLib, Apache Tomcat, SAStruts, Seasar2, Swing
- ツール：Eclipse, GitLab, Redmine, MySQL Workbench

##### 業務内容

- Swing を用いての図形や画像などのオブジェクトの描画、回転、縮小機能の実装
- PDF 出力機能の実装
- MySQL を用いた DB チューニング、テスト用データの作成
- SAStruts, Seasar2 による API の実装
  - 画像アップロード、コピー、更新、削除機能の実装
  - ディレクトリトラバーサル対策

#### 2014年5月〜2014年6月 ウッドデッキ見積 Web システムの不具合改修

- 概要：ウッドデッキを作図し、作図内容をもとに見積もり金額を算出するための Web システム
- 担当工程：コーディング、テスト、運用/保守
- 役割：PG
- 規模：1〜5 名

##### 開発環境

- 言語：Java
- OS・DB：Windows
- ライブラリ・フレームワーク：Jakarta Tomcat, Swing
- ツール：Eclipse, Subversion

##### 業務内容

- 不具合調査および修正
  - 文言修正
  - 計算ロジック修正

## 免許・資格

|年月|免許・資格|
|---|---|
|2009年11月|基本情報技術者試験|
|2010年2月|日商簿記2級|
|2010年3月|全商検定5冠（電卓、ワープロ、プログラミング、ビジネス情報、簿記）|
|2011年9月|普通自動車第一種運転免許|
|2023年5月|整理収納アドバイザー2級|
|2023年6月|クリンネスト2級|

## 学会発表

- 電子情報通信学会総合大会 ISS 特別企画「学生ポスターセッション」発表
  - 鎌田均、 丸橋駿平、 澤野弘明： “指差し動作を利用したカーナビのための助手席ユーザの経路指示方法の一調査”, 電子情報通信学会総合大会 ISS 特別企画「学生ポスターセッション」, ISS-SP-317, 1 page (2013-3)

## 業務外活動

- ワールドビジネスサテライト 2015 年 1 月 22 日出演
  - TimeTicket というサービスにて、プログラミング関連の相談に乗っていました
  - <https://blog.timeticket.jp/post/108879706835/%E3%83%86%E3%83%AC%E3%83%93%E6%9D%B1%E4%BA%AC%E3%83%AF%E3%83%BC%E3%83%AB%E3%83%89%E3%83%93%E3%82%B8%E3%83%8D%E3%82%B9%E3%82%B5%E3%83%86%E3%83%A9%E3%82%A4%E3%83%88%E3%81%A7%E7%B4%B9%E4%BB%8B%E3%81%95%E3%82%8C%E3%81%BE%E3%81%97%E3%81%9F>
- スパルタキャンプ Java/Android 編 講師（2015 年 10 月、2016 年 3 月）
  - 3、4 日間かけて Android アプリの開発を学べるプログラミング教室で講師を務めました
  - ![sparta_camp.jpg](img/sparta_camp.jpg)
- 妖怪笑い袋（スマートスピーカーアプリ）の開発およびリリース
  - 全てのキーワードに対して、ランダムに笑い声を返すだけのスキルです
  - リリース初月で利用者数 100 人突破
    - Google アシスタント版 **※公開停止**
      - 動画 : <https://www.youtube.com/watch?v=N-AQ-Q36Ts0>
    - Alexa 版 **※公開停止**
      - 動画 : <https://www.youtube.com/watch?v=2d-1DX_Zojc>
- かんたん食事管理（iOS アプリ）の開発およびリリース **※公開停止**
  - ソースコード : <https://github.com/hiesiea/SimpleMealManager>
  - その日に食べた食事の画像とテキスト情報を入力して一覧表示してくれるアプリです
- PHP 勉強会
- 技術発信
  - 主に Qiita, Zenn などで実務等で得られた技術的知見を発信しています
- OSS 活動
  - DroidKaigi 2021〜2024 official app コントリビューター

## 今後の展望

- 新しいことが好きなので、Android アプリの開発以外にも挑戦したりなど、さまざまな知識や経験を貪欲に吸収していきたいです
- テックリードとしての経験をもっと積んでいき、技術にも携わりつつマネジメントもできる人材を目指したいです
- 可能であれば日常会話程度以上の英語力を身に付けたいです
- 将来的に技術書を出版したり、カンファレンスでの登壇を目指したいです

## 希望条件

- リモートワークでの勤務を希望します
  - 出社が必要な場合、東京都 23 区内もしくは千葉県内への出社であれば可能です
- 言われたとおりにただ作るのではなく、機能要件に対しても一緒に考えたり、提案しやすい環境を希望します
- 役職関係なく、フラットにコミュニケーションを取り合える環境を希望します
- 新しい挑戦（新技術の導入など）に積極的に取り組める環境を希望します
- フレックス制度や育休制度などがあり、その時の状況によって労働環境や労働時間を変えやすい環境を希望します
  - 2024 年 5 月に第 1 子が生まれ、育児中であるため急な休みや早退などの可能性があることを承知いただけると幸いです
- 技術発信や勉強会、カンファレンスへの参加に対して会社として支援いただける環境を希望します