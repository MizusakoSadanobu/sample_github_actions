# やること
- github actionsとpytestを組み合わせた自動テストのパイプラインを作る

# 手順
- 下準備
    - venvで仮想環境を作る
    - .gitignoreでgit管理対象からvenvを除外する
- ローカルでの開発作業
    - 必要なパッケージのインストール
    - テスト、実行ファイルの作成
- 自動テストのための準備
    - pip freezeでrequirements.txtを自動生成する
    - yamlファイルの作成
- 自動テスト実行
    - ローカルでの変更内容をPush

# 躓きポイント
- Actionsに書き込みの権限を与えないとエラーが出る
    - https://zenn.dev/tatsugon/articles/github-actions-permission-error
- pytest-covのインストールが必要