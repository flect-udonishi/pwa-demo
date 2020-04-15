# pwa-demo

# 実行環境
* Ruby2.6.2
* Ruby on Rails 5.2.4.2
* PostgreSQL 11.5以上

# 環境構築
1. rbenvをインストール

2. Rubyをインストール
```
$ rbenv install 2.6.2
```
インストールが終わったら次のコマンドでシステム全体で使用するRubyのバージョンをrbenvに設定する。
```
$ rbenv global 2.6.2
```
Rubyのバージョンを確認する。
```
$ ruby -v
```

3. Bundlerのインストール
```
$ gem install bundler
```

4. Railsのインストール
```
$ gem install rails -v 5.2.4.2
```
Railsのバージョンを確認する。
```
$ rails -v
```

5. PostgreSQLのインストール

# 使い方
このアプリケーションを動かす場合は、まずはリポジトリを手元にクローンしてください。
その後、次のコマンドで必要になる RubyGems をインストールします。

```
$ bundle install
```  

※ bundle installに失敗する場合、Gemfile.lockを削除した後に、再度上記のコマンドを実行します。

その後、データベースへのマイグレーションを実行します。

```
$ rails db:migrate
```

サーバ起動を起動します。  
```
$ rails s
```
