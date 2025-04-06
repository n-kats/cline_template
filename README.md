# 使い方
``` bash
pipx run cookiecutter git@github.com:n-kats/cline_template.git
```

## cookiecutter のtips
### デフォルトの設定値を変更したい。
`~/.cookiecutterrc` に以下を追加してください。

``` yaml
default_context:
  project_name: "project_name"
  author_name: "author_name"
  author_email: "author_email"
  github_username: "github_username"
```

### 会社用と個人用で .cookiecutterrc を分けたい。
`cookiecutter` コマンドを実行する際に `--config-file` オプションを指定してください。

``` bash
pipx run cookiecutter git@github.com:n-kats/cline_template.git --config-file ~/.cookiecutterrc_work
```


# gitignore

Python用のignore に以下を追加しています。

|項目|用途|
|---|---|
|/_data|データ|
|/_model|モデル|
|/_models|モデル（推奨）|
|/_output|出力|
|/_outputs|出力（推奨）|
|/_cache|キャッシュ|
|/_tmp|一時（推奨）|
|/_temp|一時|
|/_log|ログ|
|/_logs|ログ（推奨）|
