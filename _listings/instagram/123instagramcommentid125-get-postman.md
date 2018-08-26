{
  "info": {
    "name": "Instagram Instagram Comment",
    "_postman_id": "3f70dbba-43df-4df7-acf7-c403a7f83549",
    "description": "Instagram Comment",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Instagram",
      "item": [
        {
          "id": "a2dcca55-5ad4-4905-88d5-bab77ac365ed",
          "name": "getInstagramMediaComments",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;instagram-media-id&#125;/comments?100=100",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Instagram Media Comments"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f31ec97-9c35-45ff-9579-550543e61db1"
            }
          ]
        },
        {
          "id": "eff0fa03-8be5-451e-86f5-21f7d8c0c051",
          "name": "getInstagramUser",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;instagram-user-id&#125;?followed_by_countint32=followed_by_countint32&follow_countint32=follow_countint32&has_profile_picturebool=has_profile_picturebool&idnumeric string=idnumeric%20string&is_privatebool=is_privatebool&is_publishedbool=is_publishedbool&media_countint32=media_countint32&profile_picstring=profile_picstring&usernamestring=usernamestring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Instagram User"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46e301b9-a7fc-4d99-a214-2e6f4f8ccf53"
            }
          ]
        },
        {
          "id": "689f470a-70ad-494c-bcdb-0efa35040b8d",
          "name": "getInstagramUserAgencies",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;instagram-user-id&#125;/agencies?294=294",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Instagram User Agencies"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6979130-1571-4600-8951-83e7904d6866"
            }
          ]
        },
        {
          "id": "3c4987e7-d876-4700-8d92-62e8b627d673",
          "name": "getInstagramUserAuthorizedAdaccounts",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;instagram-user-id&#125;/authorized_adaccounts?100=100",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Instagram User Authorized Adaccounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79487daf-6b89-44c4-93a2-34e563912824"
            }
          ]
        },
        {
          "id": "26701d56-75fb-4ac1-8276-bd2877681c0f",
          "name": "getInstagramMedia",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;instagram-media-id&#125;?caption_textstring=caption_textstring&comment_countint32=comment_countint32&content_typeint32=content_typeint32&display_urlstring=display_urlstring&filter_namestring=filter_namestring&idnumeric string=idnumeric%20string&latitudefloat=latitudefloat&like_countint32=like_countint32&locationLocation=locationLocation&location_namestring=location_namestring&longitudefloat=longitudefloat&owner_instagram_userInstagramUser=owner_instagram_userInstagramUser&permalinkstring=permalinkstring&taken_atdatetime=taken_atdatetime&video_urlstring=video_urlstring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Instagram Media"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42123144-03ca-4832-9dc8-cce0291cc501"
            }
          ]
        },
        {
          "id": "a5b0dd78-f4d9-44b7-bc35-7c28bc08b91d",
          "name": "getInstagramComment",
          "request": {
            "url": "http://graph.facebook.com/v3.0/&#123;instagram-comment-id&#125;?comment_typeenum=comment_typeenum&created_atdatetime=created_atdatetime&idstring=idstring&instagram_comment_idnumeric string=instagram_comment_idnumeric%20string&instagram_userInstagramUser=instagram_userInstagramUser&mentioned_instagram_userslistInstagramUser=mentioned_instagram_userslistInstagramUser&messagestring=messagestring",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Instagram Comment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2fe88371-d742-47a5-8005-11037606b9f8"
            }
          ]
        }
      ]
    }
  ]
}