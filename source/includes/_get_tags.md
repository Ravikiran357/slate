
# getSoftwareTags

To get a list of item/posts with software tags.

```http
GET /getSoftwareTags?type=Post HTTP/1.1

HTTP/1.1 200 OK
Content-Type: application/json

{
  "type": "getSoftwareTags",
  "message": "SUCCESS",
  "results": [
    {
      "autoTranslated": false,
      "recorded_Time": "12:53:52",
      "softwareTags": {
        "скайпу": "Skype"
      },
      "postedDate": "2017-05-30",
      "uid": 115157,
      "boardsName": "Защита информации",
      "forumsId": 38,
      "topicsName": "Интеллектуальная собственность",
      "postContent": "многие не понимают и ведут бизнес переговоры по скайпу. на сегодняшний день есть только один распределённый шифрованный мессенджер поддерживающий звук и видео: tox. есть ещё ring, но он похоже ещё не очень стабилен. только распределённые (бессерверные) мессенджеры с открытым кодом могут считаться защищёнными от прослушивания так как централизованные системы привязаны к компаниям.",
      "postsId": 32999860,
      "postedTime": "12:53:52",
      "language": "Russian",
      "topicId": 148653,
      "scrapedDate": "2017-05-30",
      "postMs": null,
      "postCve": null,
      "recordedDate": "2017-05-30",
      "recordedTime": "12:53:52",
      "financialTags": null,
      "entity": null,
      "tags": null
    }
  ]
}
```

```http
GET /getSoftwareTags?type=Item HTTP/1.1

HTTP/1.1 200 OK
Content-Type: application/json

{
  "type": "getSoftwareTags",
  "message": "SUCCESS",
  "results": [
    {
      "autoTranslated ": false,
      "itemId": 797314,
      "itemName": "paypal accounts usd451.05",
      "itemDescription": null,
      "language": "English",
      "uid": "1",
      "marketplaceId": "32",
      "recordedTime": "12:00:00",
      "scrapedDate": "2017-05-25",
      "postedDate": "None",
      "recordedDate": "2017-05-25",
      "itemCve": null,
      "itemMs": null,
      "itemCategory": "paypal accounts ",
      "itemEscrowinfo": null,
      "itemViews": null,
      "itemLastViewDate": "None",
      "itemQuantitySold": null,
      "itemQuantityLeft": null,
      "itemShippedFrom": null,
      "itemShippedTo": null,
      "itemVendorRating": "0.00",
      "itemSuccessfulTrans": null,
      "softwareTags": {
        "paypal": "Paypal"
      },
      "financialTags": {
        "paypal": "Paypal"
      },
      "entity": null,
      "sellingPrice": [
        {
          "sellingPriceUsd": "451.050000"
        }
      ],
      "tags": null
    }
  ]
}
```
**URL:** *http://apigargoyle.com/GargoyleApi/beta/getSoftwareTags*
### Request Format
The getSoftwareTags API call uses the following as the required parameter

Parameter | Description
--------- | -----------
type* | type should be of value Item or Post. It is case-sensitive.
start | start record of the results that is to be retrieved. Default is 0 when start is not set. Allows “=” behavior
limit | Number of records to be retrieved. Default is 10 when limit not set. Maximum limit is 10000. When more data having index > 10000 is to be retrieved set start=10000 and limit = "some amount of results you want"
tagContent | Search for item/post with a specific tag
pastDay |
getCount | if set to true, it will return the total number of results with the filters in place.
from | Date (YYYY-MM-DD) from which information was scraped; if “to” is not specified, then information through the present is returned
to | Date (YYYY-MM-DD) to which information was scraped; if “from” is not specified, then information starting from the earliest available in the dB is returned

<aside class="notice">
* mandatory parameter that needs to be included with the request
</aside>

* URL with single request parameter: To give a single parameter to a request, specify a parameter with its value like examples given below:

1. *http://apigargoyle.com/GargoyleApi/beta/getSoftwareTags?type=Post*

2. *http://apigargoyle.com/GargoyleApi/beta/getSoftwareTags?type=Item*

* URL with multiple request parameters: To give multiple parameters to a request, separate each parameter with ‘&’ like the example given below:

1. *http://apigargoyle.com/GargoyleApi/beta/getSoftwareTags?type=Post&limit=2*

2. *http://apigargoyle.com/GargoyleApi/beta/getSoftwareTags?type=Item&getCount=true*

### Response Format

Parameter | Description
--------- | -----------
type | Name of API call
results | List of hacking items
message | status of the API call
count | If true, displays the total count of the results with the filters in place. Otherwise, not displayed in the response body

**Example Response:**

Sample responses are shown on the right side.


# getFinancialTags

To get a list of items/posts with Financial tags

```http
GET /getFinancialTags?type=Post HTTP/1.1

HTTP/1.1 200 OK
Content-Type: application/json

{
  "type": "getFinancialTags",
  "message": "SUCCESS",
  "results": [
    {
      "autoTranslated": false,
      "recorded_Time": "12:16:59",
      "softwareTags": null,
      "postedDate": "2017-06-01",
      "uid": 90778,
      "boardsName": "Финансы и Право",
      "forumsId": 38,
      "topicsName": "[Статья] Развод на деньги в торговой площадке на Ebay",
      "postContent": "майор полиции бутылкин пишет:увидит ли немамонт что карта не просто visa / mastercard, но еще и русс. виртуальнаяесли захочет то увидит. есть сервисы пробива карт. например вот этот https://www.bindb.com/bin-database.html",
      "postsId": 33925534,
      "postedTime": "12:16:59",
      "language": "Russian",
      "topicId": 148496,
      "scrapedDate": "2017-06-03",
      "postMs": null,
      "postCve": null,
      "recordedDate": "2017-06-01",
      "recordedTime": "12:16:59",
      "financialTags": {
        "mastercard": "Mastercard"
      },
      "entity": [
        {
          "entityId": "https://www.bindb.com/bin-database.html",
          "freebaseTypes": null,
          "type": [
            "URL"
          ],
          "matchedText": "https://www.bindb.com/bin-database.html",
          "entityEnglishId": ""
        }
      ],
      "tags": null,
      "originalContent": null
    }
  ]
}
```

```http
GET /getFinancialTags?type=Item HTTP/1.1

HTTP/1.1 200 OK
Content-Type: application/json

{
  "type": "getFinancialTags",
  "message": "SUCCESS",
  "results": [
    {
     "autoTranslated": false,
      "itemId": 941641,
      "itemName": "paypal accounts usd457.26",
      "itemDescription": null,
      "language": "English",
      "uid": "1",
      "marketplaceId": "32",
      "recordedTime": "12:00:00",
      "scrapedDate": "2017-06-03",
      "postedDate": "None",
      "recordedDate": "2017-06-03",
      "itemCve": null,
      "itemMs": null,
      "itemCategory": "paypal accounts ",
      "itemEscrowinfo": null,
      "itemViews": null,
      "itemLastViewDate": "None",
      "itemQuantitySold": null,
      "itemQuantityLeft": null,
      "itemShippedFrom": null,
      "itemShippedTo": null,
      "itemVendorRating": "0.00",
      "itemSuccessfulTrans": null,
      "softwareTags": null,
      "financialTags": {
        "paypal": "Paypal"
      },
      "entity": null,
      "sellingPrice": [
        {
          "sellingPriceUsd": "457.260000"
        }
      ],
      "tags": null
    }
  ]
}
```
**URL:** *http://apigargoyle.com/GargoyleApi/beta/getFinancialTags*
### Request Format
The getFinancialTags API call can be refined by adding one or more of the following parameters.

Parameter | Description
--------- | -----------
type* | type should be of value Item or Post. It is case-sensitive.
start | start record of the results that is to be retrieved. Default is 0 when start is not set. Allows “=” behavior
limit | Number of records to be retrieved. Default is 10 when limit not set. Maximum limit is 10000. When more data having index > 10000 is to be retrieved set start=10000 and limit = "some amount of results you want"
tagContent | Search for item/post with a specific tag
pastDay |
getCount | if set to true, it will return the total number of results with the filters in place.
from | Date (YYYY-MM-DD) from which information was scraped; if “to” is not specified, then information through the present is returned
to | Date (YYYY-MM-DD) to which information was scraped; if “from” is not specified, then information starting from the earliest available in the dB is returned

<aside class="notice">
* refers to a mandatory parameter that needs to be included with the request
</aside>

* URL with single request parameter: To give a single parameter to a request, specify a parameter with its value like examples given below:

1. *http://apigargoyle.com/GargoyleApi/beta/getFinancialTags?type=Post*

2, *http://apigargoyle.com/GargoyleApi/beta/getFinancialTags?type=Item*

* URL with multiple request parameters: To give multiple parameters to a request, separate each parameter with ‘&’ like the example given below:

1. *http://apigargoyle.com/GargoyleApi/beta/getFinancialTags?type=Post&limit=2*

2. *http://apigargoyle.com/GargoyleApi/beta/getFinancialTags?type=Item&getCount=true*

### Response Format

Parameter | Description
--------- | -----------
type | Name of API call
results | List of hacking items
message | status of the API call
count | If true, displays the total count of the results with the filters in place. Otherwise, not displayed in the response body

**Example Response:**

Sample responses are shown on the right side.

