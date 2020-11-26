# DjangoをHerokuにデプロイする最小限のサンプル
---

## usage

```sh
$ git clone [this repository url]
$ cd cloned-repository-path
$ heroku create
$ heroku config:set DISABLE_COLLECTSTATIC=1
```

- Django用の秘密鍵を用意
  - cf. https://miniwebtool.com/ja/django-secret-key-generator/

```sh
$ heroku config:set DJANGO_SECRET_KEY="your-secret-key"
$ git push heroku main
```

生成されたherokuapp.comのURLを開いて :rocket: が出たら成功
