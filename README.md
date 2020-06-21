# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

```README.md
<<<<<<< Updated upstream
=======

>>>>>>> Stashed changes
## usersテーブル

|Column|Type|Options|
|------|----|-------|
|name|string|null: false, add_index: true|
|email|string|null: false, unique: true|

### Association
- has_many :messages
- has_many :group_users
<<<<<<< Updated upstream
- has_many :groups, through: :group_users
=======
- has_many :groups, through: groups_users
>>>>>>> Stashed changes

## messagesテーブル

|Column|Type|Options|
|------|----|-------|
|body|text||
|image|string||
|user_id|integer|null: false, foreign_key: true|
|group_id|integer|null: false, foreign_key: true|

### Association
- belongs_to :group
- belongs_to :user

## groupsテーブル

|Column|Type|Options|
|------|----|-------|
<<<<<<< Updated upstream
|name|string|null: false, unique: true|
=======
|group_name|string|null: false, unique: true|
>>>>>>> Stashed changes

### Association
- has_many :messages
- has_many :groups_users
<<<<<<< Updated upstream
- has_many :users, through: :groups-user
=======
- has_many :users, through: groups_users
>>>>>>> Stashed changes

## groups-userテーブル

|Column|Type|Options|
|------|----|-------|
|user_id|string|null: false, foreign_key: true|
|group_id|string|null: false, foreign_key: true|

### Association
- belongs_to :user
- belongs_to :group

```
