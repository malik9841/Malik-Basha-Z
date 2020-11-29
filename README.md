# Malik-Basha-Z
For Technical Publication Practise

# Introduction
These APIs help you avail two kinds of data - data regarding the gods and poets, their categories, and poem meters used in all of the Rig Veda verses, and data regarding the descriptions of all the nouns (except proper nouns) mentioned in Vedic literature.
# URL 
[Base URL](https://aninditabasu.github.io/indica/index.html)
# Throttle Limit
The APIs are hosted on Sheetlabs, which limits the monthly API calls to 10,000.
# Status Code
| Status Code | Description |
|--- | ---|
200 | The request was successfully completed.
404 | Web service not found.
# API Reference
All the poets and gods in the Rig Veda, presented with the mandal and sukta numbers, and the meters the verses are composed.
The Rig Veda API. Returns the gods and poets, their categories, and the meters from all the Rig Veda verses, together with the mandal and sukta number.
## How it helps Developer
You can specify a range for the integers, or partial text for the strings. You can supply more than one parameter in a single call by separating them w ith an ampersand (&), for example, https://sheetlabs.com/IND/rv?mandal=10&meter=gayatri&sungby=*dra.
## URL - Rig Veda
End point URL – https://sheetlabs.com/IND/rv
## Method
You can make only **GET** calls to the API. 
## Headers
| API | Details |
| --- | --- |
Authorization or Authentication | No authentication or authorization is required
Application type | Application/JSON
## Table of Parameters
| Parameters | Data Type | Values (if any) | Description
| --- | --- | --- | ---
mandal | Integer | 1 -10
sukta | Integer |
sungby | String | | The composer of the verse.
sungbycategory | String | | The category that composer of the verse belongs to. For example, human male. The following categories are available: 
## Sample Request
Make sure below points while calling the End Point:
* Call the service with **Get** method.
* Header
    * Authorization or Authentication – **No Auth**
## Sample Response
```
[
    {
        "mandal": 7,
        "sukta": 43,
        "sungby": "Vasishth Maitravaruni",
        "sungbycategory": "human male",
        "sungfor": "Vishwadeva",
        "sungforcategory": "divine male",
        "meter": "Trishtup"
    },
    {
        "mandal": 7,
        "sukta": 43,
        "sungby": "Vasishth Maitravaruni",
        "sungbycategory": "human male",
        "sungfor": "Agni",
        "sungforcategory": "divine male",
        "meter": "Trishtup"
    },
    {
        "mandal": 7,
        "sukta": 44,
        "sungby": "Vasishth Maitravaruni",
        "sungbycategory": "human male",
        "sungfor": "Dadhikra",
        "sungforcategory": "animal",
        "meter": "Jagati"
    }
]
```
