---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - shell
toc_footers:
  - <a href='https://github.com/lord/slate'>Koodos to Slate</a>

includes:
  - errors

search: true
---

# Introduction

Welcome to the op.io API! You can use our API to access op.io API endpoints, which can get information on various business data and reviews in our database.

We have language bindings in Shell coming soon: Ruby, Python, and JavaScript! You can view code examples in the dark area to the right, and you can switch the programming language of the examples with the tabs in the top right.

# Authentication

> To authorize, use this code:



```shell
# With shell, you can just pass the correct header with each request
curl "https://op.io/api/entities/entity_id"
  -H "Authorization: Bearer ACCESS_TOKEN"
```



> Make sure to replace `ACCESS_TOKEN` with your API key.

op.io uses API Access token to allow access to the API. You will need to request one from our team.

op.io expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: Bearer ACCESS_TOKEN`

<aside class="notice">
You must replace <code>ACCESS_TOKEN</code> with your business' Access Token.
</aside>

# op.io

## Get my op.io business data




```shell
curl "https://op.io/api/entities/entity_id"
  -H "Authorization: ACCESS_TOKEN"
```



> The above command returns JSON structured like this:

```json
[
    {
        "dateCreated": 1520541056825,
        "dateUpdated": 1554843258677,
        "name": "Ryans Plumbingers",
        "_id": "jeiyvwahsq7hayvcp",
        "description": "Great Plumbing services. Local prices.",
        "type": "business",
        "logo": {
            "imageId": "c9040f5d9ccb9b1a158f854647ee59f8",
            "dateCreated": 1520541056038,
            "_id": "jeiyvvomkpekr9yqd",
            "dateUpdated": 1520541056038
        },
        "coverImage": "https://rimages.n49.ca/r_images/640x640/390/389318.jpg",
        "address": {
            "country": "United States",
            "province": "MA",
            "city": "Boston",
            "address1": "459 Massachusetts Avenues",
            "postalCode": "02118"
        },
        "phone1": "4163852433",
        "phone2": "",
        "tags": [],
        "users": [
            {
                "user_id": "ju2qbdsq6mbfpm76s",
                "email": "dhiraj+52154@n49.com",
                "fullName": "Bazaar Rhinoceros",
                "firstName": "Bazaar",
                "lastName": "Rhinoceros",
                "username": "",
                "dateCreated": 1554387721370,
                "dateUpdated": 1554387721370,
                "relationships": [
                    "USER_CAN_GET_ENTITY",
                    "USER_CAN_UPDATE_ENTITY"
                ],
                "type": "user",
                "deleted": false
            },
            {
                "user_id": "jtytyy48b0xjjmvv4",
                "email": "dhiraj+54845@n49.com",
                "fullName": "second dhiraj",
                "firstName": "second",
                "lastName": "dhiraj",
                "username": "",
                "dateCreated": 1554151994936,
                "dateUpdated": 1554151994936,
                "relationships": [
                    "USER_CAN_GET_ENTITY",
                    "USER_CAN_UPDATE_ENTITY"
                ],
                "type": "user",
                "deleted": false
            },
            {
                "user_id": "jlwfd3gcux5mg9rew",
                "email": "dhiraj@n49.com",
                "fullName": "Dhiraj Timalsina",
                "firstName": "Dhiraj",
                "lastName": "Timalsina",
                "username": "",
                "userPic": {
                    "imageId": "cb87e0310c601934fc379676aeb26098",
                    "dateCreated": 1554151447948,
                    "_id": "jtytn824gd1lyzrhq",
                    "dateUpdated": 1554151447948
                },
                "dateCreated": 1536592269756,
                "dateUpdated": 1554151450308,
                "relationships": [
                    "USER_CAN_GET_ENTITY",
                    "USER_CAN_UPDATE_ENTITY"
                ],
                "type": "user",
                "deleted": false
            }
        ],
        "reviews": [
            {
                "_id": "jtywp6fyacugb91yy",
                "status": "published",
                "deleted": false,
                "propertyId": "5734f48a0b64d7382829fdf7",
                "entityId": "jeiyvwahsq7hayvcp",
                "entityInfo": {},
                "propertyInfo": {
                    "displayName": "OP.IO",
                    "dateCreated": 1512502852720,
                    "deleted": false,
                    "_id": "5734f48a0b64d7382829fdf7",
                    "dateModified": 1548186924774,
                    "description": "Main domain for review product",
                    "logo": {
                        "imageId": "d8eb1d2d92723461f28c5356112cb979",
                        "dateCreated": 1529944095296,
                        "_id": "jiuh7n7kqd8x62vux",
                        "dateUpdated": 1529944095296
                    },
                    "name": "OP.IO",
                    "primaryColor": "#209cd3",
                    "dateUpdated": 1548186924774,
                    "domain": "op.io",
                    "relationships": [
                        "REVIEW_BELONGS_TO_PROPERTY"
                    ]
                },
                "rating": 5,
                "labels": [
                    "Review"
                ],
                "dateCreated": 1554156578014,
                "dateUpdated": 1554156589473,
                "images": [],
                "videos": [],
                "tags": [],
                "comments": [],
                "user": {
                    "dateCreated": 1554156577874,
                    "dateUpdated": 1554156587036,
                    "user_id": "jtywp6c2fm4i579mm",
                    "fullName": "dddw dds",
                    "firstName": "dddw",
                    "lastName": "dds",
                    "username": "",
                    "userPic": "",
                    "deleted": false,
                    "status": "enabled"
                },
                "content": "this should make 12th review",
                "totalEntities": 1,
                "totalProperties": 1,
                "totalUsers": 1,
                "totalImages": 0,
                "totalVideos": 0,
                "totalTags": 0,
                "totalComments": 0,
                "fullyLoaded": true
            },
            {
                "_id": "jtug8osofk9xx7uc9",
                "status": "published",
                "deleted": false,
                "propertyId": "5734f48a0b64d7382829fdf7",
                "entityId": "jeiyvwahsq7hayvcp",
                "entityInfo": {},
                "propertyInfo": {
                    "displayName": "OP.IO",
                    "dateCreated": 1512502852720,
                    "deleted": false,
                    "_id": "5734f48a0b64d7382829fdf7",
                    "dateModified": 1548186924774,
                    "description": "Main domain for review product",
                    "logo": {
                        "imageId": "d8eb1d2d92723461f28c5356112cb979",
                        "dateCreated": 1529944095296,
                        "_id": "jiuh7n7kqd8x62vux",
                        "dateUpdated": 1529944095296
                    },
                    "name": "OP.IO",
                    "primaryColor": "#209cd3",
                    "dateUpdated": 1548186924774,
                    "domain": "op.io",
                    "relationships": [
                        "REVIEW_BELONGS_TO_PROPERTY"
                    ]
                },
                "rating": 5,
                "labels": [
                    "Review"
                ],
                "dateCreated": 1553887070088,
                "dateUpdated": 1553887085481,
                "images": [],
                "videos": [],
                "tags": [],
                "comments": [],
                "user": {
                    "dateCreated": 1553887069965,
                    "dateUpdated": 1553887085147,
                    "user_id": "jtug8op909906hmfo",
                    "fullName": "asdf asdf",
                    "firstName": "asdf",
                    "lastName": "asdf",
                    "username": "",
                    "userPic": "",
                    "deleted": false,
                    "status": "enabled"
                },
                "content": "11th review",
                "totalEntities": 1,
                "totalProperties": 1,
                "totalUsers": 1,
                "totalImages": 0,
                "totalVideos": 0,
                "totalTags": 0,
                "totalComments": 0,
                "fullyLoaded": true
            },
            {
                "_id": "jtuf5qfbn6cclz1wu",
                "status": "published",
                "deleted": false,
                "propertyId": "5734f48a0b64d7382829fdf7",
                "entityId": "jeiyvwahsq7hayvcp",
                "entityInfo": {},
                "propertyInfo": {
                    "displayName": "OP.IO",
                    "dateCreated": 1512502852720,
                    "deleted": false,
                    "_id": "5734f48a0b64d7382829fdf7",
                    "dateModified": 1548186924774,
                    "description": "Main domain for review product",
                    "logo": {
                        "imageId": "d8eb1d2d92723461f28c5356112cb979",
                        "dateCreated": 1529944095296,
                        "_id": "jiuh7n7kqd8x62vux",
                        "dateUpdated": 1529944095296
                    },
                    "name": "OP.IO",
                    "primaryColor": "#209cd3",
                    "dateUpdated": 1548186924774,
                    "domain": "op.io",
                    "relationships": [
                        "REVIEW_BELONGS_TO_PROPERTY"
                    ]
                },
                "rating": 5,
                "labels": [
                    "Review"
                ],
                "dateCreated": 1553885252615,
                "dateUpdated": 1553885268685,
                "images": [],
                "videos": [],
                "tags": [],
                "comments": [],
                "user": {
                    "dateCreated": 1553885252466,
                    "dateUpdated": 1553885259400,
                    "user_id": "jtuf5qb6kcwh24gdv",
                    "fullName": "10th review",
                    "firstName": "10th",
                    "lastName": "review",
                    "username": "",
                    "userPic": "",
                    "deleted": false,
                    "status": "enabled"
                },
                "content": "this is the 10th review",
                "totalEntities": 1,
                "totalProperties": 1,
                "totalUsers": 1,
                "totalImages": 0,
                "totalVideos": 0,
                "totalTags": 0,
                "totalComments": 0,
                "fullyLoaded": true
            },
            {
                "_id": "jthosdtqdgy6q9ooa",
                "status": "published",
                "deleted": false,
                "propertyId": "5734f48a0b64d7382829fdf7",
                "entityId": "jeiyvwahsq7hayvcp",
                "entityInfo": {},
                "propertyInfo": {
                    "displayName": "OP.IO",
                    "dateCreated": 1512502852720,
                    "deleted": false,
                    "_id": "5734f48a0b64d7382829fdf7",
                    "dateModified": 1548186924774,
                    "description": "Main domain for review product",
                    "logo": {
                        "imageId": "d8eb1d2d92723461f28c5356112cb979",
                        "dateCreated": 1529944095296,
                        "_id": "jiuh7n7kqd8x62vux",
                        "dateUpdated": 1529944095296
                    },
                    "name": "OP.IO",
                    "primaryColor": "#209cd3",
                    "dateUpdated": 1548186924774,
                    "domain": "op.io",
                    "relationships": [
                        "REVIEW_BELONGS_TO_PROPERTY"
                    ]
                },
                "rating": 5,
                "labels": [
                    "Review"
                ],
                "dateCreated": 1553115365630,
                "dateUpdated": 1553884681845,
                "images": [],
                "videos": [],
                "tags": [],
                "comments": [],
                "user": {
                    "dateCreated": 1536592269756,
                    "dateUpdated": 1554151450308,
                    "user_id": "jlwfd3gcux5mg9rew",
                    "fullName": "Dhiraj Timalsina",
                    "firstName": "Dhiraj",
                    "lastName": "Timalsina",
                    "username": "",
                    "userPic": {
                        "imageId": "cb87e0310c601934fc379676aeb26098",
                        "dateCreated": 1554151447948,
                        "_id": "jtytn824gd1lyzrhq",
                        "dateUpdated": 1554151447948
                    },
                    "deleted": false,
                    "status": "enabled"
                },
                "content": "make it 101",
                "totalEntities": 1,
                "totalProperties": 1,
                "totalUsers": 1,
                "totalImages": 0,
                "totalVideos": 0,
                "totalTags": 0,
                "totalComments": 0,
                "fullyLoaded": true
            },
            {
                "_id": "jtsq74r3aegup385j",
                "status": "published",
                "deleted": false,
                "propertyId": "5734f48a0b64d7382829fdf7",
                "entityId": "jeiyvwahsq7hayvcp",
                "entityInfo": {},
                "propertyInfo": {
                    "displayName": "OP.IO",
                    "dateCreated": 1512502852720,
                    "deleted": false,
                    "_id": "5734f48a0b64d7382829fdf7",
                    "dateModified": 1548186924774,
                    "description": "Main domain for review product",
                    "logo": {
                        "imageId": "d8eb1d2d92723461f28c5356112cb979",
                        "dateCreated": 1529944095296,
                        "_id": "jiuh7n7kqd8x62vux",
                        "dateUpdated": 1529944095296
                    },
                    "name": "OP.IO",
                    "primaryColor": "#209cd3",
                    "dateUpdated": 1548186924774,
                    "domain": "op.io",
                    "relationships": [
                        "REVIEW_BELONGS_TO_PROPERTY"
                    ]
                },
                "rating": 4,
                "labels": [
                    "Review"
                ],
                "dateCreated": 1553782861263,
                "dateUpdated": 1553782881116,
                "images": [
                    {
                        "_id": "jtsq6ga4u113gyd7p",
                        "dateCreated": 1553782829548,
                        "imageId": "9a4dfe7497ae2ad1f4a487937737e52a",
                        "dateUpdated": 1553782829548,
                        "relationships": [
                            "IMAGE_BELONGS_TO_REVIEW"
                        ]
                    }
                ],
                "videos": [
                    {
                        "_id": "jtsq6juuya7okom5o",
                        "dateCreated": 1553782834182,
                        "videoId": "ab14ef96c688dbf68082733f26a73efd",
                        "dateUpdated": 1553782834182,
                        "relationships": [
                            "VIDEO_BELONGS_TO_REVIEW"
                        ]
                    }
                ],
                "tags": [],
                "comments": [],
                "user": {
                    "dateCreated": 1553782861128,
                    "dateUpdated": 1553782880877,
                    "user_id": "jtsq74ncr0sxu8r0e",
                    "fullName": "Djdj Xnxn",
                    "firstName": "Djdj",
                    "lastName": "Xnxn",
                    "username": "",
                    "userPic": "",
                    "deleted": false,
                    "status": "enabled"
                },
                "content": "Landscape photo and Video",
                "totalEntities": 1,
                "totalProperties": 1,
                "totalUsers": 1,
                "totalImages": 1,
                "totalVideos": 1,
                "totalTags": 0,
                "totalComments": 0,
                "fullyLoaded": true
            },
            {
                "_id": "jtohfrgrmg8160urr",
                "status": "published",
                "deleted": false,
                "propertyId": "5734f48a0b64d7382829fdf7",
                "entityId": "jeiyvwahsq7hayvcp",
                "entityInfo": {},
                "propertyInfo": {
                    "displayName": "OP.IO",
                    "dateCreated": 1512502852720,
                    "deleted": false,
                    "_id": "5734f48a0b64d7382829fdf7",
                    "dateModified": 1548186924774,
                    "description": "Main domain for review product",
                    "logo": {
                        "imageId": "d8eb1d2d92723461f28c5356112cb979",
                        "dateCreated": 1529944095296,
                        "_id": "jiuh7n7kqd8x62vux",
                        "dateUpdated": 1529944095296
                    },
                    "name": "OP.IO",
                    "primaryColor": "#209cd3",
                    "dateUpdated": 1548186924774,
                    "domain": "op.io",
                    "relationships": [
                        "REVIEW_BELONGS_TO_PROPERTY"
                    ]
                },
                "rating": 4,
                "labels": [
                    "Review"
                ],
                "dateCreated": 1553526282699,
                "dateUpdated": 1553526290046,
                "images": [
                    {
                        "_id": "jtohfayphknysma4g",
                        "dateCreated": 1553526261313,
                        "imageId": "652e4509cd403c3eaaec10e03e66affc",
                        "dateUpdated": 1553526261313,
                        "relationships": [
                            "IMAGE_BELONGS_TO_REVIEW"
                        ]
                    }
                ],
                "videos": [],
                "tags": [],
                "comments": [],
                "user": {
                    "dateCreated": 1553526282478,
                    "dateUpdated": 1553526289730,
                    "user_id": "jtohframgj30r0amo",
                    "fullName": "Ff Xnxn",
                    "firstName": "Ff",
                    "lastName": "Xnxn",
                    "username": "",
                    "userPic": "",
                    "deleted": false,
                    "status": "enabled"
                },
                "content": "Landscape",
                "totalEntities": 1,
                "totalProperties": 1,
                "totalUsers": 1,
                "totalImages": 1,
                "totalVideos": 0,
                "totalTags": 0,
                "totalComments": 0,
                "fullyLoaded": true
            },
            {
                "_id": "jthotv5s5w5pb61lf",
                "status": "published",
                "deleted": false,
                "propertyId": "5734f48a0b64d7382829fdf7",
                "entityId": "jeiyvwahsq7hayvcp",
                "entityInfo": {},
                "propertyInfo": {
                    "displayName": "OP.IO",
                    "dateCreated": 1512502852720,
                    "deleted": false,
                    "_id": "5734f48a0b64d7382829fdf7",
                    "dateModified": 1548186924774,
                    "description": "Main domain for review product",
                    "logo": {
                        "imageId": "d8eb1d2d92723461f28c5356112cb979",
                        "dateCreated": 1529944095296,
                        "_id": "jiuh7n7kqd8x62vux",
                        "dateUpdated": 1529944095296
                    },
                    "name": "OP.IO",
                    "primaryColor": "#209cd3",
                    "dateUpdated": 1548186924774,
                    "domain": "op.io",
                    "relationships": [
                        "REVIEW_BELONGS_TO_PROPERTY"
                    ]
                },
                "rating": 5,
                "labels": [
                    "Review"
                ],
                "dateCreated": 1553115434752,
                "dateUpdated": 1553115443787,
                "images": [],
                "videos": [],
                "tags": [],
                "comments": [],
                "user": {
                    "dateCreated": 1553115434623,
                    "dateUpdated": 1553874004587,
                    "user_id": "jthotv276aibo8aes",
                    "fullName": "asdf asdf",
                    "firstName": "asdf",
                    "lastName": "asdf",
                    "username": "",
                    "userPic": "",
                    "deleted": false,
                    "status": "enabled"
                },
                "content": "make it 7 review",
                "totalEntities": 1,
                "totalProperties": 1,
                "totalUsers": 1,
                "totalImages": 0,
                "totalVideos": 0,
                "totalTags": 0,
                "totalComments": 0,
                "fullyLoaded": true
            },
            {
                "_id": "jthon4cuo4l77xnz4",
                "status": "published",
                "deleted": false,
                "propertyId": "5734f48a0b64d7382829fdf7",
                "entityId": "jeiyvwahsq7hayvcp",
                "entityInfo": {},
                "propertyInfo": {
                    "displayName": "OP.IO",
                    "dateCreated": 1512502852720,
                    "deleted": false,
                    "_id": "5734f48a0b64d7382829fdf7",
                    "dateModified": 1548186924774,
                    "description": "Main domain for review product",
                    "logo": {
                        "imageId": "d8eb1d2d92723461f28c5356112cb979",
                        "dateCreated": 1529944095296,
                        "_id": "jiuh7n7kqd8x62vux",
                        "dateUpdated": 1529944095296
                    },
                    "name": "OP.IO",
                    "primaryColor": "#209cd3",
                    "dateUpdated": 1548186924774,
                    "domain": "op.io",
                    "relationships": [
                        "REVIEW_BELONGS_TO_PROPERTY"
                    ]
                },
                "rating": 5,
                "labels": [
                    "Review"
                ],
                "dateCreated": 1553115120078,
                "dateUpdated": 1553115138693,
                "images": [],
                "videos": [],
                "tags": [],
                "comments": [],
                "user": {
                    "dateCreated": 1545166776824,
                    "dateUpdated": 1553115137998,
                    "user_id": "jpu8ejg89p0sn7jhp",
                    "fullName": "asdf asdf",
                    "firstName": "asdf",
                    "lastName": "asdf",
                    "username": "",
                    "userPic": "",
                    "deleted": false,
                    "status": "enabled"
                },
                "content": "sdfds",
                "totalEntities": 1,
                "totalProperties": 1,
                "totalUsers": 1,
                "totalImages": 0,
                "totalVideos": 0,
                "totalTags": 0,
                "totalComments": 0,
                "fullyLoaded": true
            },
            {
                "_id": "jthoklg6535ljnbvn",
                "status": "published",
                "deleted": false,
                "propertyId": "5734f48a0b64d7382829fdf7",
                "entityId": "jeiyvwahsq7hayvcp",
                "entityInfo": {},
                "propertyInfo": {
                    "displayName": "OP.IO",
                    "dateCreated": 1512502852720,
                    "deleted": false,
                    "_id": "5734f48a0b64d7382829fdf7",
                    "dateModified": 1548186924774,
                    "description": "Main domain for review product",
                    "logo": {
                        "imageId": "d8eb1d2d92723461f28c5356112cb979",
                        "dateCreated": 1529944095296,
                        "_id": "jiuh7n7kqd8x62vux",
                        "dateUpdated": 1529944095296
                    },
                    "name": "OP.IO",
                    "primaryColor": "#209cd3",
                    "dateUpdated": 1548186924774,
                    "domain": "op.io",
                    "relationships": [
                        "REVIEW_BELONGS_TO_PROPERTY"
                    ]
                },
                "rating": 4.5,
                "labels": [
                    "Review"
                ],
                "dateCreated": 1553115002262,
                "dateUpdated": 1553115010628,
                "images": [],
                "videos": [],
                "tags": [],
                "comments": [],
                "user": {
                    "dateCreated": 1553115002115,
                    "dateUpdated": 1553115010364,
                    "user_id": "jthoklc3igqifv7h1",
                    "fullName": "asdfkj alsdfk",
                    "firstName": "asdfkj",
                    "lastName": "alsdfk",
                    "username": "",
                    "userPic": "",
                    "deleted": false,
                    "status": "enabled"
                },
                "content": "increase count to 4 reviews",
                "totalEntities": 1,
                "totalProperties": 1,
                "totalUsers": 1,
                "totalImages": 0,
                "totalVideos": 0,
                "totalTags": 0,
                "totalComments": 0,
                "fullyLoaded": true
            },
            {
                "_id": "jtehuzlhsrscmnjxu",
                "status": "published",
                "deleted": false,
                "propertyId": "5734f48a0b64d7382829fdf7",
                "entityId": "jeiyvwahsq7hayvcp",
                "entityInfo": {},
                "propertyInfo": {
                    "displayName": "OP.IO",
                    "dateCreated": 1512502852720,
                    "deleted": false,
                    "_id": "5734f48a0b64d7382829fdf7",
                    "dateModified": 1548186924774,
                    "description": "Main domain for review product",
                    "logo": {
                        "imageId": "d8eb1d2d92723461f28c5356112cb979",
                        "dateCreated": 1529944095296,
                        "_id": "jiuh7n7kqd8x62vux",
                        "dateUpdated": 1529944095296
                    },
                    "name": "OP.IO",
                    "primaryColor": "#209cd3",
                    "dateUpdated": 1548186924774,
                    "domain": "op.io",
                    "relationships": [
                        "REVIEW_BELONGS_TO_PROPERTY"
                    ]
                },
                "rating": 4,
                "labels": [
                    "Review"
                ],
                "dateCreated": 1552922331317,
                "dateUpdated": 1552922343116,
                "images": [],
                "videos": [
                    {
                        "_id": "jtehu67yr95vrhy2s",
                        "dateCreated": 1552922293246,
                        "videoId": "301a5f02f5ce6ecca58713ae6c3906b9",
                        "dateUpdated": 1552922293246,
                        "relationships": [
                            "VIDEO_BELONGS_TO_REVIEW"
                        ]
                    }
                ],
                "tags": [],
                "comments": [],
                "user": {
                    "dateCreated": 1552922331177,
                    "dateUpdated": 1552922342763,
                    "user_id": "jtehuzhls3a8ieo2o",
                    "fullName": "Shd Shs",
                    "firstName": "Shd",
                    "lastName": "Shs",
                    "username": "",
                    "userPic": "",
                    "deleted": false,
                    "status": "enabled"
                },
                "content": "35 second video ",
                "totalEntities": 1,
                "totalProperties": 1,
                "totalUsers": 1,
                "totalImages": 0,
                "totalVideos": 1,
                "totalTags": 0,
                "totalComments": 0,
                "fullyLoaded": true
            },
            {
                "_id": "jt9kqm2tu5suhk5og",
                "status": "published",
                "deleted": false,
                "propertyId": "5734f48a0b64d7382829fdf7",
                "entityId": "jeiyvwahsq7hayvcp",
                "entityInfo": {},
                "propertyInfo": {
                    "displayName": "OP.IO",
                    "dateCreated": 1512502852720,
                    "deleted": false,
                    "_id": "5734f48a0b64d7382829fdf7",
                    "dateModified": 1548186924774,
                    "description": "Main domain for review product",
                    "logo": {
                        "imageId": "d8eb1d2d92723461f28c5356112cb979",
                        "dateCreated": 1529944095296,
                        "_id": "jiuh7n7kqd8x62vux",
                        "dateUpdated": 1529944095296
                    },
                    "name": "OP.IO",
                    "primaryColor": "#209cd3",
                    "dateUpdated": 1548186924774,
                    "domain": "op.io",
                    "relationships": [
                        "REVIEW_BELONGS_TO_PROPERTY"
                    ]
                },
                "rating": 4.5,
                "labels": [
                    "Review"
                ],
                "dateCreated": 1552624835141,
                "dateUpdated": 1552624854575,
                "images": [
                    {
                        "_id": "jt9kom3vo7cw486e5",
                        "dateCreated": 1552624741867,
                        "imageId": "5948ca1c1d69e6233200eada0898ffe6",
                        "dateUpdated": 1552624741867,
                        "relationships": [
                            "IMAGE_BELONGS_TO_REVIEW"
                        ]
                    },
                    {
                        "_id": "jt9kq4snko6mdpnl1",
                        "dateCreated": 1552624812743,
                        "imageId": "26c3584390d61472f8bd6525734335cf",
                        "dateUpdated": 1552624812743,
                        "relationships": [
                            "IMAGE_BELONGS_TO_REVIEW"
                        ]
                    }
                ],
                "videos": [],
                "tags": [],
                "comments": [],
                "user": {
                    "dateCreated": 1552624835003,
                    "dateUpdated": 1552624853363,
                    "user_id": "jt9kqlyzbbn32zdls",
                    "fullName": "Xgd Dbsb",
                    "firstName": "Xgd",
                    "lastName": "Dbsb",
                    "username": "",
                    "userPic": "",
                    "deleted": false,
                    "status": "enabled"
                },
                "content": "Ryabs",
                "totalEntities": 1,
                "totalProperties": 1,
                "totalUsers": 1,
                "totalImages": 2,
                "totalVideos": 0,
                "totalTags": 0,
                "totalComments": 0,
                "fullyLoaded": true
            },
            {
                "_id": "jt93h0yz5ycdg1nsf",
                "status": "published",
                "deleted": false,
                "propertyId": "5734f48a0b64d7382829fdf7",
                "entityId": "jeiyvwahsq7hayvcp",
                "entityInfo": {},
                "propertyInfo": {
                    "displayName": "OP.IO",
                    "dateCreated": 1512502852720,
                    "deleted": false,
                    "_id": "5734f48a0b64d7382829fdf7",
                    "dateModified": 1548186924774,
                    "description": "Main domain for review product",
                    "logo": {
                        "imageId": "d8eb1d2d92723461f28c5356112cb979",
                        "dateCreated": 1529944095296,
                        "_id": "jiuh7n7kqd8x62vux",
                        "dateUpdated": 1529944095296
                    },
                    "name": "OP.IO",
                    "primaryColor": "#209cd3",
                    "dateUpdated": 1548186924774,
                    "domain": "op.io",
                    "relationships": [
                        "REVIEW_BELONGS_TO_PROPERTY"
                    ]
                },
                "rating": 5,
                "labels": [
                    "Review"
                ],
                "dateCreated": 1552595834410,
                "dateUpdated": 1552595863466,
                "images": [
                    {
                        "_id": "jt93gftncmd22v9di",
                        "dateCreated": 1552595807003,
                        "imageId": "976e47fcaa67c40495d402bcf60b095b",
                        "dateUpdated": 1552595807003,
                        "relationships": [
                            "IMAGE_BELONGS_TO_REVIEW"
                        ]
                    }
                ],
                "videos": [],
                "tags": [],
                "comments": [],
                "user": {
                    "dateCreated": 1552595834233,
                    "dateUpdated": 1552595863148,
                    "user_id": "jt93h0u1l7n455cdi",
                    "fullName": "D D",
                    "firstName": "D",
                    "lastName": "D",
                    "username": "",
                    "userPic": "",
                    "deleted": false,
                    "status": "enabled"
                },
                "content": "Testing ",
                "totalEntities": 1,
                "totalProperties": 1,
                "totalUsers": 1,
                "totalImages": 1,
                "totalVideos": 0,
                "totalTags": 0,
                "totalComments": 0,
                "fullyLoaded": true
            }
        ],
        "reviewsDisabled": false,
        "apiKeys": [],
        "reviewFeedSettings": {
            "hours": false,
            "address": true,
            "providedByReseller": false,
            "feedStarColor": "rgba(236, 57, 19, 1)",
            "feedButtonTextColor": "#ffffff",
            "description": true,
            "customButton": false,
            "feedBgColor": "#ffffff",
            "writeReview": true,
            "aggregateWidget": true,
            "poweredByOpioLogo": true,
            "feedButtonColor": "#0078ca",
            "activeFontFamily": {
                "name": "Roboto",
                "value": "default"
            },
            "phone": true,
            "contact": "Book a consultation",
            "name": false,
            "logo": true,
            "on": true
        },
        "reviewFeedUrls": {
            "5734f48a0b64d7382829fdf7": "http://deveric.dev.pop.ca/ryan/reviews/"
        },
        "reviewFeedSEO": {
            "5734f48a0b64d7382829fdf7": "json-ld"
        },
        "reviewFeedTestDate": 1553122029154,
        "properties": [
            {
                "dateCreated": 1512502852720,
                "dateUpdated": 1548186924774,
                "name": "OP.IO",
                "domain": "op.io",
                "displayName": "OP.IO",
                "description": "Main domain for review product",
                "logo": {
                    "imageId": "d8eb1d2d92723461f28c5356112cb979",
                    "dateCreated": 1529944095296,
                    "_id": "jiuh7n7kqd8x62vux",
                    "dateUpdated": 1529944095296
                },
                "primaryColor": "#209cd3",
                "_id": "5734f48a0b64d7382829fdf7",
                "deleted": false,
                "reviews": [],
                "entities": [],
                "organizations": [],
                "relationships": [
                    "ENTITY_CAN_BE_REVIEWED_ON_PROPERTY"
                ],
                "totalReviews": 0,
                "totalEntities": 0,
                "totalOrganizations": 0,
                "total": 0
            }
        ],
        "aggregateRating": {
            "average": 4.7,
            "total": 12,
            "5734f48a0b64d7382829fdf7": {
                "average": 4.7,
                "total": 12,
                "star1": 0,
                "star4": 3,
                "star5": 9,
                "star2": 0,
                "star3": 0
            },
            "star1": 0,
            "star4": 3,
            "star5": 9,
            "star2": 0,
            "star3": 0
        },
        "hours": [],
        "organizations": [
            {
                "coverImage": {
                    "imageId": "b65f6b91118d14e6dd4031aa16ac0988",
                    "dateCreated": 1525191259896,
                    "_id": "jgnvhvy09shqj2le5",
                    "dateUpdated": 1525191259896
                },
                "dateCreated": 1525191269453,
                "permissions": [
                    "user can get entities",
                    "user can get reviews",
                    "user can get users",
                    "user can update entities",
                    "user can update reviews",
                    "user can update users",
                    "user can get deleted",
                    "user can get removefilters",
                    "user can create entities",
                    "user can create reviews",
                    "user can create users",
                    "user can delete entities",
                    "user can delete reviews",
                    "user can delete users",
                    "user can disable reviews for entities",
                    "user can disable users",
                    "user can import businesses",
                    "user can import reviews",
                    "user can get properties",
                    "user can create comments",
                    "user can update properties",
                    "user can get comments",
                    "user can update comments",
                    "user can delete comments",
                    "user can create as entities",
                    "user can create as reviews",
                    "user can get draft reviews",
                    "user can sync algolia with organizations",
                    "user can operate as",
                    "user can delete as comments",
                    "user can delete as reviews",
                    "user can create as comments",
                    "user can update permissions for organizations",
                    "user can get userstatus",
                    "user can sync relations with reviews",
                    "user can sync algolia with users",
                    "user can sync algolia with entities",
                    "user can assign properties to entities",
                    "user can assign properties to organizations",
                    "user can assign entities to organizations",
                    "user can assign users to organizations",
                    "user can delete as apps",
                    "user can delete as organizations",
                    "user can delete as tags",
                    "user can delete as properties",
                    "user can delete as entities",
                    "user can update as apps",
                    "user can update as comments",
                    "user can update as organizations",
                    "user can update as reviews",
                    "user can update as tags",
                    "user can update as properties",
                    "user can update as entities",
                    "user can get as apps",
                    "user can get as comments",
                    "user can get as organizations",
                    "user can get as reviews",
                    "user can get as tags",
                    "user can get as properties",
                    "user can get as entities",
                    "user can create as apps",
                    "user can create as organizations",
                    "user can create as tags",
                    "user can create as properties",
                    "user can delete apps",
                    "user can delete organizations",
                    "user can delete tags",
                    "user can delete properties",
                    "user can update apps",
                    "user can update organizations",
                    "user can update tags",
                    "user can get apps",
                    "user can get organizations",
                    "user can get tags",
                    "user can create apps",
                    "user can create organizations",
                    "user can create tags",
                    "user can create properties",
                    "user can create anonymous users",
                    "user can update timestamps for reviews",
                    "user can update timestamps for entities",
                    "user can update timestamps for users",
                    "user can update timestamps for organizations",
                    "user can update timestamps for comments",
                    "user can update timestamps for properties",
                    "user can update seo for entity",
                    "user can get stats",
                    "user can sync algolia with properties",
                    "user can get reviewstatus",
                    "user can update email for users"
                ],
                "_id": "jgnvi3bh5c3fak2xy",
                "address": {
                    "country": "Canada",
                    "province": "ON",
                    "city": "Toronto",
                    "address1": "505 Eglinton Avenue West",
                    "postalCode": "M5N 1B1"
                },
                "hours": [],
                "logo": {
                    "_id": "jr86iktncn2ha1ng8",
                    "dateCreated": 1548186914795,
                    "imageId": "d4f5a5ef229b1818ec553f72e81517d6",
                    "dateUpdated": 1548186914795
                },
                "name": "OPIO",
                "dateUpdated": 1548186919337,
                "type": "business",
                "relationships": [
                    "USER_CAN_GET_ENTITY",
                    "USER_CAN_UPDATE_ENTITY"
                ]
            },
            {
                "dateCreated": 1522097215137,
                "_id": "jf8pdrq9bf4ilckoo",
                "address": {
                    "country": "United States",
                    "province": "NY",
                    "city": "New York",
                    "address1": "60 Lexington Avenue",
                    "postalCode": "10010"
                },
                "hours": [],
                "name": "drmg",
                "dateUpdated": 1526676696759,
                "type": "business",
                "relationships": [
                    "USER_CAN_GET_ENTITY",
                    "USER_CAN_UPDATE_ENTITY"
                ]
            },
            {
                "displayName": "Super Admins",
                "dateCreated": 1512502853126,
                "deleted": false,
                "__v": 11,
                "permissions": [
                    "user can sync algolia with properties",
                    "user can create entities",
                    "user can create properties",
                    "user can create tags",
                    "user can create reviews",
                    "user can create organizations",
                    "user can create comments",
                    "user can create apps",
                    "user can get entities",
                    "user can get properties",
                    "user can get tags",
                    "user can get reviews",
                    "user can get organizations",
                    "user can get apps",
                    "user can get users",
                    "user can get comments",
                    "user can update entities",
                    "user can update properties",
                    "user can update tags",
                    "user can update reviews",
                    "user can update organizations",
                    "user can update apps",
                    "user can update comments",
                    "user can delete entities",
                    "user can delete properties",
                    "user can delete tags",
                    "user can delete reviews",
                    "user can delete organizations",
                    "user can delete comments",
                    "user can delete apps",
                    "user can create as comments",
                    "user can create as entities",
                    "user can create as properties",
                    "user can create as tags",
                    "user can create as reviews",
                    "user can create as organizations",
                    "user can create as comments",
                    "user can create as apps",
                    "user can get as comments",
                    "user can get as entities",
                    "user can get as properties",
                    "user can get as tags",
                    "user can get as reviews",
                    "user can get as organizations",
                    "user can get as comments",
                    "user can get as apps",
                    "user can update as entities",
                    "user can update as comments",
                    "user can update as properties",
                    "user can update as tags",
                    "user can update as reviews",
                    "user can update as organizations",
                    "user can update as comments",
                    "user can update as apps",
                    "user can delete as entities",
                    "user can delete as properties",
                    "user can delete as tags",
                    "user can delete as reviews",
                    "user can delete as organizations",
                    "user can delete as comments",
                    "user can delete as apps",
                    "user can operate as",
                    "user can assign users to organizations",
                    "user can assign entities to organizations",
                    "user can assign properties to organizations",
                    "user can create users",
                    "user can update users",
                    "user can delete users",
                    "user can assign properties to entities",
                    "user can sync algolia with entities",
                    "user can sync algolia with users",
                    "user can sync algolia with organizations",
                    "user can sync relations with reviews",
                    "user can get deleted",
                    "user can get userstatus",
                    "user can get reviewstatus",
                    "user can get removefilters",
                    "user can get draft reviews",
                    "user can import reviews",
                    "user can import businesses",
                    "user can disable users",
                    "user can disable reviews for entities",
                    "user can update permissions for organizations",
                    "user can create anonymous users",
                    "user can update timestamps for reviews",
                    "user can update timestamps for entities",
                    "user can update timestamps for users",
                    "user can update timestamps for organizations",
                    "user can update timestamps for comments",
                    "user can update timestamps for properties",
                    "user can get stats",
                    "user can update email for users",
                    "user can update seo for entity"
                ],
                "_id": "572a442747ab89c93c1435e5",
                "scopes": {
                    "image": [
                        "_id",
                        "imageId"
                    ],
                    "review": [
                        "title",
                        "_id",
                        "propertyId",
                        "entityId",
                        "rating",
                        "createdAt",
                        "images",
                        "videos",
                        "tags",
                        "user",
                        "content",
                        "deleted",
                        "relationships"
                    ],
                    "organization": [
                        "name",
                        "_id",
                        "description",
                        "permissions",
                        "deleted",
                        "users",
                        "entities",
                        "properties",
                        "relationships"
                    ],
                    "property": [
                        "name",
                        "displayName",
                        "description",
                        "_id",
                        "reviews",
                        "entities",
                        "relationships"
                    ],
                    "tag": [
                        "name",
                        "_id",
                        "relationships"
                    ],
                    "video": [
                        "_id",
                        "videoId"
                    ],
                    "user": [
                        "email",
                        "username",
                        "fullName",
                        "lastName",
                        "userName",
                        "givenName",
                        "surname",
                        "userPic",
                        "customData",
                        "entities",
                        "reviews",
                        "organizations",
                        "tags",
                        "properties",
                        "images",
                        "videos",
                        "users",
                        "save"
                    ],
                    "entity": [
                        "name",
                        "_id",
                        "description",
                        "type",
                        "tags",
                        "users",
                        "reviews",
                        "deleted",
                        "relationships"
                    ]
                },
                "description": "All global permissions are assigned to the Super Admins. Should only be used by n49 employees.",
                "logo": {
                    "imageId": "442cbe75f6c796f715ff80ea28fcb46e",
                    "_id": "57a9079166f021552d63a734",
                    "deleted": false,
                    "__v": 0
                },
                "name": "Super Admins",
                "dateUpdated": 1512504540396,
                "relationships": [
                    "USER_CAN_GET_ENTITY",
                    "USER_CAN_UPDATE_ENTITY",
                    "USER_CAN_DEFINE_TAGS_FOR_ENTITY",
                    "USER_CAN_PUBLISH_REVIEWS_OF_ENTITY",
                    "USER_CAN_ASSIGN_USERS_TO_ENTITY",
                    "USER_CAN_GET_TAGS_FOR_ENTITY",
                    "USER_CAN_ASSIGN_PROPERTIES_TO_ENTITY"
                ]
            }
        ],
        "reviewUs": {},
        "reviewUsUrl": "",
        "totalReviews": 12,
        "totalUsers": 3,
        "totalTags": 0,
        "totalProperties": 1,
        "totalOrganizations": 3,
        "algolia": false,
        "fullyLoaded": true,
        "stripeCustomerId": "",
        "stripe": null,
        "freshbooksClientId": "",
        "billingEmail": "",
        "reviewFeedSubscriptionEnabled": false,
        "reviewFeedSubscriptionDateEnd": "",
        "failedCharges": 0,
        "writeReviewUrlHandler": "ryanplumbing",
        "nativeFeedEnabled": "php",
        "rating": 4.7
    }
]
```

This endpoint retrieves your op.io business data based on entity id. It will also retrieve your latest 25 reviews if you do not set subSkip or subLimit. If you want to paginate lets say after 25 reviews and get the next 25 reviews, set <em>scopes</em> to <b>Review</b> <em>subSkip</em> to <b>25</b> and <em>subLimit</em> to <b>25</b>

### HTTP Request

`GET https://op.io/api/entities/entity_id`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
scopes | all | If set to Review, the result will only output review data, use when paginating.
subSkip | 0 | If set to 25, it will skip the first latest 25 reviews and fetch until the set subLimit use for paginating.
subLimit | 25 | If set to 100, it will bring 100 reviews after the set subSkip.

<aside class="success">
Remember — all opio request must have an authenticated token!
</aside>
