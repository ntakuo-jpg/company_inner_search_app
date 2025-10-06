# 社内情報特化型生成AI検索アプリ

このアプリケーションは、社内文書を検索・問い合わせできる生成AI検索システムです。

## 機能

- **社内文書検索**: 入力内容に関連性の高い社内文書を検索
- **社内問い合わせ**: 質問に対する回答と参照文書を提供

## セットアップ

### 必要な環境

- Python 3.8以上
- OpenAI APIキー

### インストール手順

1. リポジトリをクローン

```bash
git clone <your-repository-url>
cd company_inner_search_app
```

2. 依存パッケージのインストール

**macOS の場合:**
```bash
pip install -r requirements_mac.txt
```

**Windows の場合:**
```bash
pip install -r requirements_windows.txt
```

3. 環境変数の設定

プロジェクトルートに `.env` ファイルを作成し、以下の内容を設定してください：

```
OPENAI_API_KEY=your-openai-api-key-here
```

4. アプリケーションの起動

```bash
streamlit run main.py
```

## プロジェクト構成

```
company_inner_search_app/
├── main.py                 # メインアプリケーション
├── initialize.py          # 初期化処理
├── utils.py              # ユーティリティ関数
├── components.py         # UI コンポーネント
├── constants.py          # 定数定義
├── requirements_mac.txt  # macOS用パッケージ
├── requirements_windows.txt  # Windows用パッケージ
└── data/                # 社内文書データ
    ├── MTG議事録/
    ├── サービスについて/
    ├── 会社について/
    ├── 社員について/
    └── 顧客について/
```

## 使い方

1. アプリケーションを起動すると、2つのモードが選択できます
   - **社内文書検索**: 関連文書を探す
   - **社内問い合わせ**: 質問に回答を得る

2. モードを選択後、チャット入力欄に質問や検索キーワードを入力

3. AIが関連する文書や回答を提供します

## ライセンス

このプロジェクトは教育目的で作成されています。

## 注意事項

- `.env` ファイルには機密情報が含まれるため、絶対にGitにコミットしないでください
- データフォルダには社内の機密文書が含まれる可能性があるため、公開リポジトリにアップロードする際は注意してください

