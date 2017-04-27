# サーバー実装手順
## 実装者の事前準備
1. kensyu2017リポジトリで「http」ブランチにチェックアウトする
    - (https://github.com/bizreach/kensyu2017)
2. 「http」ブランチから「{自分の名前}_http」ブランチをチェックアウトする
    - 例: yamamoto_http
    - ※ 基本的に実装者が触ることになるブランチは「{自分の名前}_http」ブランチのみ
## 各STEPの実装手順
1. 「{自分の名前}_http」ブランチから各ステップのブランチ「{自分の名前}_http{STEP番号}」をチェックアウトする
    - 例: yamamoto_http1
2. 「{自分の名前}_http{STEP番号}」で実装を行う
3. 実装完了後、実装者はissueに紐付けるかたちでプルリクを作成する
    - Reviewers: 各STEPのレビュワー
    - Assignees: 実装者
    - Comment: 各ステップのissue番号を記載(STEP1 なら #1)
4. Slackで実装者がレビュワーにプルリク作成の旨を通知
    - チャネル: #zzz_17training_http
    - 形式: メンション付きでレビュー依頼を出す
      - 例: @ryohei.yamamoto STEP8のレビューをお願いします。
5. レビュワーはレビューを行い、コメントを残す
6. Slackでレビュワーが実装者にレビュー完了の旨を通知
7. 実装者はレビュー内容に応じて、修正を行い、再度レビュー依頼を投げる
8. レビュワーはレビューOKであれば、プルリクをマージする

上記の手順で各STEPの実装を進めていく

# その他諸々
## 起動方法
`SimpleJavaHTTPServer.java` をrunする

## レビュー観点について
各STEPに、必要に応じて「レビュー項目」を記載済み

他に必要だと感じる観点があれば、レビュワーが随時アップデートを行う

## HTTPサーバー実装のルール
4期エンジニア向けには以下のように共有している
https://github.com/RyoheiYamamoto/SimpleHttpServer/wiki

## 参考資料
### HTTP1.1について
https://triple-underscore.github.io/RFC723X-ja.html

## その他
詳細は別途共有している資料を参照
