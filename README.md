# ときのそら非公式ファンサイト

## ディレクトリ構成

```
.
├── infra
│   ├── mysql
│   │   └── initdb.d
│   └── wordpress 
└── src
    └── wp-content        
        └── themes        
            └── tokinosora // 独自テーマに関するファイルはここ
```

## 環境構築方法

1. .env.templateをコピーして.envファイルを作成
2. イメージのビルド
3. コンテナ起動

```
$ cp .env.template .env

$ docker compose build

$ docker compose up -d
```

### .envファイル記述例

```.env
WP_USER=db-user
WP_PASSWORD=db-password
ROOT_PASSWORD=root
MYSQL_DATABASE=tokinosora
MYSQL_USER=db-user
MYSQL_PASSWORD=db-password
```
