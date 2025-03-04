# 模擬案件　フリマアプリ  
  
## 環境構築
Dockerビルド  
1.git clone git@github.com:Daisuke70/Flea-Market-App.git  
2.docker-compose up -d --build  

Laravel環境構築  
1.docker-compose exec php bash  
2.composer install  
3.「.env.example」ファイルから新しく「.env」ファイルを作成し  
4..envに以下の環境変数を追加  
DB_CONNECTION=mysql  
DB_HOST=mysql  
DB_PORT=3306  
DB_DATABASE=laravel_db  
DB_USERNAME=laravel_user  
DB_PASSWORD=laravel_pass  
5.アプリケーションキーの作成  
php artisan key:generate  
6.マイグレーションの実行  
php artisan migrate  
7.シーディングの実行  
php artisan db:seed  
8.テストユーザーのメールアドレス、パスワード  
メールアドレス：test@example.com  
パスワード：password123  

## 使用技術(実行環境)  
・PHP 7.4.9  
・Laravel 8.83.8  
・MySQL 15.1  


## ER図  
 
<img width="477" alt="模擬案件　フリマアプリ　ER図" src="https://github.com/user-attachments/assets/8fff09e3-a92f-4268-8ef4-101e8ee91e0d" />

## URL
・開発環境：http://localhost/  
・phpMyAdmin：http://localhost:8080/
