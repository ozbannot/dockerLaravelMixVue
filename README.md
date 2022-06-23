## 環境情報
```
・ Docker
・ Laravel6.x(LTS)
・ Vue2.x(LTS)
・ MySQL8.x(LTS)
・ Nginx(LTS)
```

## 構築手順(TIPS)
```
$ docker-compose -d
$ docker compose exec app bash
$ composer create-project --prefer-dist "laravel/laravel=6.*" .
$ composer require laravel/ui "1.x" --dev(version指定してあげないとコケる)
$ php artisan ui vue
$ npm install
$ npm install --save vue-router
$ npm run dev
$ npm run watch(毎回npm run devでビルドが怠い場合はwatchで監視してあげる)
```

## Vue導入確認
```
routes/web.php
で適当にroutingを用意(確認できればいいので、ひとまずは/でいい)
併せてbladeでVue確認用のファイルを作成
デフォルトで用意されているexample-componentで反映確認
確認できたらVue導入OK、example-componentはBootstrapも使われているのでその確認も兼ねている
```
