---
nav_title: 5月
page_order: 8
noindex: true
page_type: update
description: "この記事には2020年5月のリリースノートが含まれている。"
---
# 2020年5月

## Google Tag Manager

Googleタグマネージャーを使用したBrazeのAndroid SDKのデプロイと管理方法のドキュメントと例を追加。

## 新しいブラックリストメールAPIエンドポイント

Braze API経由でメールアドレスを[ブラックリストに登録]({{site.baseurl}}/api/endpoints/email/post_blacklist/)できるようになった。メールアドレスをブラックリストに登録すると、ユーザーはメールの配信を停止され、ハードバウンスとしてマークされる。

## Braze APIエンドポイントのAPIキー変更

2020年5月より、BrazeはAPIキーの読み取り方法をより安全なものに変更した。APIキーはリクエストヘッダーとして渡されなければならない。例は、**API Key Explanationと**同様に、**Example Requestの**下にある個々のエンドポイントのページで見ることができる。

Brazeは、リクエストボディやURLパラメータを通して渡される`api_key` をサポートし続けるが、最終的にはSunsetting配信停止となる（未定）。**それに応じてAPIコールを更新する。**これらの変更は[Postman](https://documenter.getpostman.com/view/4689407/SVYrsdsG?version=latest#intro)内で更新された。
{% details APIキーの説明 %}
{% tabs %}
{% tab GET Request %}
この例では、`/email/hard_bounces` エンドポイントを使用している。

**その前だ：リクエスト・ボディにAPIキーを入力する**
```
curl --location --request GET 'https://rest.iad-01.braze.com/email/hard_bounces?api_key={YOUR_REST_API_KEY}&start_date=2019-01-01&end_date=2019-02-01&limit=100&offset=1&email=foo@braze.com' \
```
**今すぐだ：ヘッダー内のAPIキー**
```
curl --location --request GET 'https://rest.iad-01.braze.com/email/hard_bounces?start_date=2019-01-01&end_date=2019-02-01&limit=100&offset=1&email=foo@braze.com' \
--header 'Authorization: Bearer YOUR-REST-API-KEY'
```
{% endtab %}
{% tab POST Request %}
この例では、`/user/track` エンドポイントを使用している。

**その前だ：リクエスト・ボディにAPIキーを入力する**
```
curl --location --request POST 'https://rest.iad-01.braze.com/users/track' \
--header 'Content-Type: application/json' \
--data-raw '{
	"api_key": YOUR-API-KEY-HERE ,
	"attributes": [ 
 	{
 	  "external_id":"user_id",
      "string_attribute": "sherman",
      "boolean_attribute_1": true,
      "integer_attribute": 25,
      "array_attribute": ["banana", "apple"]
    }
    ]
}'
```
**今すぐだ：ヘッダー内のAPIキー**
```
curl --location --request POST 'https://rest.iad-01.braze.com/users/track' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer YOUR-REST-API-KEY' \
--data-raw '{
	"attributes": [ 
 	{
	  "external_id":"user_id",
      "string_attribute": "sherman",
      "boolean_attribute_1": true,
      "integer_attribute": 25,
      "array_attribute": ["banana", "apple"]
    }
    ]
}'
```
{% endtab %}
{% endtabs %}
{% enddetails %}


