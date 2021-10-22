# DB定義書
## ER図
[ER図はこちら](https://github.com/Aso2001026/2021sys-design/blob/main/md/sample/DB/ER%E5%9B%B3.md)

# DBテーブルカラム一覧

# データベース設計図

## ログイン(d_purchase)

|和名|属性名(カラム名)|型|PK|NN|FK|
|---|-----|--|--|--|--|
|Email|order_id|bigint(20)|○|○||
|password|customer_code|varchar(50)||○|○|

## 新規会員登録(d_purchase_detail)

|和名|属性名(カラム名)|型|PK|NN|FK|
|---|-----|--|--|--|--|
|Email|order_id|bigint(20)|○|○||
|password|customer_cod|bigint(20) |○|○|○|


## 会員情報(m_customers)

|和名|属性名(カラム名)|型|PK|NN|FK|
|---|-----|--|--|--|--|
|購入履歴|Purchase history|varchar(50)|○|○||
|お気に入り|favorite|varchar(50)||○||
|会員情報変更|Member information change|varchar(20)||○||
|パスワード変更|Change Password|varchar(100)||○||
|決済情報変更|Change payment information|varchar(20)||○||
|アドレス変更|Address change|varchar(100)||○||

## お気に入り(m_category)

|和名|属性名(カラム名)|型|PK|NN|FK|
|---|-----|--|--|--|--|
|カテゴリID|category_id|int(11)|○|○||
|氏名|name|varchar(20)||○||
|登録日|reg_date|date||○||

## 検索ページ(m_items)

|和名|属性名(カラム名)|型|PK|NN|FK|
|---|-----|--|--|--|--|
|商品コード|item_code|int(11)|○|○||
|商品名|item_name|varchar(50)||○||
|価格|price|int(11)||○||
|カテゴリID|category_id|int(11)||○|○|
|画像ファイル名|image|varchar(200)||○||
|商品詳細証明|detail|varchar(500)||||
|削除フラグ|del_flag|int(11)||||
|登録日|reg_date|date||○||

## カート(m_category)

|和名|属性名(カラム名)|型|PK|NN|FK|
|---|-----|--|--|--|--|
|カテゴリID|category_id|int(11)|○|○||
|氏名|name|varchar(20)||○||
|登録日|reg_date|date||○||

## 住所(m_category)

|和名|属性名(カラム名)|型|PK|NN|FK|
|---|-----|--|--|--|--|
|氏名|name|int(11)|○|○||
|住所|address|varchar(20)||○||
|電話番号|number|date||○||






