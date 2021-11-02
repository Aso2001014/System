# DB定義書
## ER図
[ER図はこちら](https://github.com/Aso2001026/2021sys-design/blob/main/md/sample/DB/ER%E5%9B%B3.md)

# DBテーブルカラム一覧

# データベース設計図

## ログイン(d_purchase)

|和名|属性名(カラム名)|型|PK|NN|FK|
|---|-----|--|--|--|--|
|氏名|user_name|varchar(20)|○|○||
|メール|mail|varchar(100)|○|○||
|パスワード|password|varchar(50)||○|○|

## 新規会員登録(d_purchase_detail)

|和名|属性名(カラム名)|型|PK|NN|FK|
|---|-----|--|--|--|--|
|氏名|user_name|varchar(20)|○|○||
|メール|mail|varchar(100)|○|○||
|パスワード|password|varchar(50)||○|○|


## 会員情報(m_customers)

|和名|属性名(カラム名)|型|PK|NN|FK|
|---|-----|--|--|--|--|
|購入履歴|Purchase history|varchar(50)|○|○||
|お気に入り|favorite|varchar(50)||○||
|会員情報変更|Member information change|varchar(20)||○||
|パスワード変更|Change Password|varchar(50)||○||
|決済情報変更|Change payment information|varchar(20)||○||
|アドレス変更|Address change|varchar(100)||○||

## お気に入り(m_category)

|和名|属性名(カラム名)|型|PK|NN|FK|
|---|-----|--|--|--|--|
|カテゴリID|category_id|int(11)|○|○||
|氏名|user_name|varchar(20)||○||
|登録日|reg_date|date||○||

## 検索ページ(m_items)

|和名|属性名(カラム名)|型|PK|NN|FK|
|---|-----|--|--|--|--|
|検索ワード|search|int(11)|○|○||


## カート(m_category)

|和名|属性名(カラム名)|型|PK|NN|FK|
|---|-----|--|--|--|--|
|価格|price|int(11)|○|○||
|数量|num|varchar(20)||○||
|削除フラグ|del_flag|date||○||

## 住所(m_category)

|和名|属性名(カラム名)|型|PK|NN|FK|
|---|-----|--|--|--|--|
|氏名|user_name|varchar(20)|○|○||
|住所|address|varchar(20)||○||
|電話番号|tel|varchar(20)||○||






