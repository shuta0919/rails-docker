## アプリ起動方法
1. ターミナルにて rails-dockerリポジトリをcloneする
   `$ git clone ( リポジトリURL)`
   `$ cd rails-docker`
2. rails-docker/ でコンテナを作成し起動する
   `$ docker-compose up`
3. データベースの作成
   コンテナの中に入る
   `$ docker-compose exec web bash`
   Railsのデータベースを作成
   `$ rails db:create`
   `$ rails db:migrate`
   `$ exit`
4. ブラウザから localhost:3000 にアクセスする
   `$ docker-compose up`
5. 起動終了する 
   `ctrl + c`