# Ruby on Rails Tutorial Sample App

Ruby on Rails チュートリアルの[Rails 5.1対応 (第4版)](https://railstutorial.jp/?version=5.1)をRails 5.2を使って実装

## 変更点

- [Bootstrap 4](https://rubygems.org/gems/bootstrap)を使用
- `form_for`の替わりに[`form_with`](http://api.rubyonrails.org/classes/ActionView/Helpers/FormHelper.html#method-i-form_with)を使用
- [`will_paginate`](https://github.com/mislav/will_paginate)の替わりに[`kaminari`](https://github.com/kaminari/kaminari)を使用
- [`carrierwave`](https://github.com/carrierwaveuploader/carrierwave)の替わりに[Active Storage](http://guides.rubyonrails.org/active_storage_overview.html)を使用

## セットアップ

```
$ heroku create
$ heroku config:set APP_HOST=your-app-name.herokuapp.com
$ heroku addons:create sendgrid:starter
$ git push heroku master
$ heroku run bin/rails db:migrate db:seed
$ heroku restart
$ heroku open
```
