#テーブル設計

##userテーブル

| column             | Type   | Options     |
| ------------------ | ------ | ------------|
| email              | string | null: false, unique: true |
| encrypted_password | string | null: false |
| name               | string | null: false |
| profile            | text   | null: false |
| occupation         | text   | null: false |
| position           | text   | null: false |


##prototypesテーブル

| column     | Type       | Options     |
| ---------- | ---------- | ------------|
| title      | string     | null: false |
| catch_copy | text       | null: false |
| concept    | text       | null: false |
| user       | references | null: false |

##commentsテーブル

| column    | Type       | Options     |
| --------- | ---------- | ------------|
| content   | text       | null: false |
| prototype | references | null: false |
| user      | references | null: false |
