# MakeLog

## 2024/2/14

1.  Readme作成

## 2024/2/13

1.  {% empty %}:空の時の場合を記述できる。
2.  完成

## 2024/2/12

1.  {{form.as_p}}でinputなど書かなくてもformが作成される。pはpタグ。
2.  Comment投稿エラー。models.pyでbody = models.TextField()を追記した後上書きしなかったのでbodyが無かった。
3.  Commentが投稿できないエラー。  
    〇　form action="" method="post"  
    ✕　form action="" ,method="post"
4.  テストアドレスとしてfoamにaaa@gmailとしたら「有効なメールアドレスを入力してください。」とでてきた。

## 2024/2/11

1.  Commentモデルを作成。
2.  マイグレーション：python manage.py makemigrations
3.  マイグレート：python manage.py migrate
4.  サーバー立ち上げ：python manage.py runserver
5.  {% csrf_token %}はCross Site Request Forgery（CSRF）攻撃を防ぐために使われる。

## 2024/2/10

1.  href="{%url 'post_detail' post.slug%}でリンクが追加された。
2.  models.CASCADEのCASCADEは関連付けられているものを全て削除できる
3.  タイプミス。全然わからなくて、ChatGPTになげてようやくわかった…。  
    〇　related_name  
    ✕　relatede_name

## 2024/2/9

1. post_detail.htmlを追加。

## 2024/2/8

1. ミス。まだ%の打ち間違いあり。  
   〇：{% endblock %}  
   ✕：{$ endblock %}

## 2024/2/7

1. base.html作成
2. BulmaCSSをあてる
3. {% extends "blog/base.html"}と書くとbase.htmlを継承することができる

## 2024/2/6

1. /adminとパスで管理画面にアクセスできる。
2. admin.pyにPostをimportすると管理画面にPostが表示される。

## 2024/2/5

1. 管理者を作成（python manage.py createsuperuser）

## 2024/2/4

1. migrationフォルダを作成（python manage.py makemigrations）

## 2024/2/3

1. Djangoの拡張機能追加
2. models.pyにブログ要素を追加

## 2024/2/2

1. 作成
