# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:


## usersテーブル
|column               | type  |options                  |
|---------------------|-------|-------------------------|
|email                |string |null: false, ユニーク制約  |
|encrypted_password   |string |null: false              |
|name                 |string |null: false              |
|profile              |text   |null: false              |
|occupation           |text   |null: false              |
|position             |text   |null: false              |

## prototypesテーブル
| column              | type  |options                              |
|---------------------|-------|-------------------------------------|
|title                |string     |null: false,                     |
|catch_copy           |string     |null: false                      |
|concept              |text       |null:false                       |
|user                 |references |null: false    foreign_key: true |


## commentsテーブル
| column        | type      |options                        |
|---------------|-----------|-------------------------------|
| content       |text       |null: false                    |
| prototype     |references |null: false ,foreign_key:true  |
| user          |references |null: false ,foreign_key:true  |

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
