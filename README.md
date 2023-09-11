## アプリケーション名
Investment Beginner

## アプリケーション概要
実際の米国銘柄を用いて意見を交換したり、自身のお気に入り銘柄の損益を確認したりできる投資初心者向けのアプリです。

## URL
https://investment-beginner-zsdc.onrender.com

## テスト用アカウント
* Basic認証パスワード：2222
* Basic認証ID：admin
* メールアドレス1：aaa@a
* パスワード1：a11111
* メールアドレス2：bbb@b
* パスワード2：b22222


## 利用方法
#### 意見交換
1.　トップページからのヘッダーからユーザー新規登録を行います。  
2.　投稿フォームに必要事項（銘柄、公開の是非、自由記述）を入力して投稿します。  
3.　詳細ページにあるコメントフォームから投稿を行い、他のユーザーと交流を図ります。  
#### お気に入り銘柄の損益の確認
1.　マイページにあるフォームから登録を行います。  
2.　登録日前日の終値と閲覧日前日の終値をもとに損益が表示されます。  

## アプリケーションを作成した背景
2024年より新NISAが始まります。しかし日本では現在約6割の人が投資未経験だと言われています。  
投資を行わない主な理由としては「投資は怖いものである」というイメージが先行していることと、  
誰に相談したらいいかわからないというこの2点が挙げられることが多いです。  
そのため実際の米国株を用いて損益を体験でき、また匿名で意見交換をする場を作りたいと考えてこのアプリを開発しました。

## 洗い出した要件
https://docs.google.com/spreadsheets/d/1LrMc9M8SaW0UH-OBIKf0yl92f7NsPhGk0Yp8lzTX5C8/edit#gid=982722306

## 実装した機能についての画像やGIFおよびその説明
* 意見投稿機能  
  銘柄コードを検索すると同じ銘柄に対する他のユーザーの声が見れます。  
  [![Image from Gyazo](https://i.gyazo.com/462447088a2f10c590a9d9c4a2281165.gif)](https://gyazo.com/462447088a2f10c590a9d9c4a2281165)  
* お気に入り銘柄の登録
  登録日からの損益を確認できます。
  [![Image from Gyazo](https://i.gyazo.com/225d8ab0a6de83cb4a6f81bdb70834ce.gif)](https://gyazo.com/225d8ab0a6de83cb4a6f81bdb70834ce)

## 実装予定の機能
過去20年の終値をもとにした株価チャートの表示機能

## データベース設計
[![Image from Gyazo](https://i.gyazo.com/7c6642beffa93357625c85ab1c97302d.png)](https://gyazo.com/7c6642beffa93357625c85ab1c97302d)

## 画面遷移図
[![Image from Gyazo](https://i.gyazo.com/397a69c89a302ed12a24bf3abd65ef0b.png)](https://gyazo.com/397a69c89a302ed12a24bf3abd65ef0b)

## 開発環境
* フロントエンド
* バックエンド
* インフラ
* テスト
* テキストエディタ
* タスク管理

## ローカルでの操作方法
以下のコマンドを順に実行してください。  
% git clone https://github.com/yuri-lily/Investment_Beginner.git  
% cd investment_beginner  
% bundle install  
% yarn install  

## 工夫したポイント
alphavantageという初めて使用するジェムに挑戦したことです。  
使用方法がわからず苦戦しましたが、先人のgithubの記述とChatGPTを駆使し完成することができました。  
特に株価の検索結果を投稿フォームと同じページに表示することが困難だったため、  
search_stock_dataという8つ目のアクションを作成することで可能になった際は達成感を感じました。  
今後も学び続け、技術の向上に努めたいと考えています。