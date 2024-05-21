## 各種バージョン

- node: 20.10.0

## 環境構築

1. プロジェクトをチェックアウト後、api, front フォルダ直下で yarn add をする
2. docker compose up をして DB サーバーを起動
3. api フォルダ直下で下記を実行 (openAI の有料アカウントが必要です)
   ```
   yarn memo:insert ./data/JapaneseNLP.csv
   ```
4. api フォルダ直下で yarn start:dev でサーバー側を起動
5. front フォルダ直下で yarn dev でフロントを起動
6. http://localhost:3001/chat にアクセスする
