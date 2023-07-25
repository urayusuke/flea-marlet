# 学習内容
NestJS入門 TypeScriptではじめるサーバーサイド開発

https://www.udemy.com/course/nestjs-t/

# NestJSとは
NestJSは、効率的で信頼性の高いサーバーサイドアプリケーションを構築するためのフレームワークです。TypeScriptにより実装されており、オブジェクト指向プログラミング、関数型プログラミング、および関数反応型プログラミングの要素を含んでいます。NestJSはExpress（またはFastify）と統合され、Node.jsのエコシステム内で直接使用できます。

# 環境構築

docker立ち上げ
まずは、Dockerを用いて環境を立ち上げます。このステップでは、以下のコマンドを使用します。
```
docker-compose up -d  
```
このコマンドを使用すると、docker-compose.ymlファイルに基づいてDockerコンテナが作成・起動されます。 -dフラグは"detached mode"（バックグラウンドモード）でコンテナを起動することを意味します。


API起動
```
npm run start:dev 
```
このコマンドは、開発モードでNestJSアプリケーションを起動します。


マイグレーション実行
```
npx typeorm migration:run
```
このコマンドは、まだ実行されていないすべてのTypeORMマイグレーションを順に実行します。

Jestのテスト実行
```
npm run test:watch
```
このコマンドは、ファイル変更を監視し、変更があるたびにテストを自動的に再実行します。


lint（静的コード解析）実行
```
npm run lint
```
このコマンドは、ESLintを使用してコードを解析し、潜在的な問題を特定します。