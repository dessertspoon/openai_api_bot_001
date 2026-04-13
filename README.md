# openai_api_bot_001

ChatGPT API（OpenAI）と Streamlit を使ったシンプルなチャットボットアプリです。

## 概要

テキスト入力でメッセージを送ると、GPT-3.5-turbo が返答するチャットボットです。会話履歴はセッション中保持されます。

## 機能

- OpenAI ChatGPT API（gpt-3.5-turbo）による自然言語応答
- Streamlit による Web UI
- セッション内での会話履歴の保持
- 最新メッセージを上部に表示

## セットアップ

### 前提条件

- Python 3.8 以上
- OpenAI API キー

### インストール

```bash
pip install -r requirements.txt
```

### API キーの設定

**ローカルで実行する場合：**

`.streamlit/secrets.toml` ファイルを作成し、以下を記述します。

```toml
[OpenAIAPI]
openai_api_key = "your-openai-api-key"
```

**Streamlit Community Cloud にデプロイする場合：**

アプリの設定画面 > Secrets に以下を追加します。

```toml
[OpenAIAPI]
openai_api_key = "your-openai-api-key"
```

## 実行方法

```bash
streamlit run app.py
```

ブラウザで `http://localhost:8501` が自動的に開きます。

## ファイル構成

```
openai_api_bot_001/
├── app.py              # メインアプリケーション
├── requirements.txt    # 依存パッケージ
└── README.md           # このファイル
```

## 依存パッケージ

| パッケージ | バージョン |
|-----------|-----------|
| streamlit | 1.20.0    |
| openai    | 最新版     |

## ライセンス

[MIT License](LICENSE)
