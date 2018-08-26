{
  "info": {
    "name": "reverb Get Shops Slug",
    "_postman_id": "c64e7b55-3358-4b75-812b-90b960ff2f5d",
    "description": "Get details on a shop.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "My",
      "item": [
        {
          "id": "e713f43a-a001-4fc4-a929-eb37cade4d6c",
          "name": "getMyFollowsShopsSlug",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reverb.com",
              "path": [
                "api",
                "my/follows/shops/:slug"
              ],
              "variable": [
                {
                  "id": "slug",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get my follows shops slug."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ac2fa74-af90-4658-870e-32216fcf2129"
            }
          ]
        },
        {
          "id": "52c5d093-9d5a-4885-a5ae-7a3b32614b75",
          "name": "postMyFollowsShopsSlug",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reverb.com",
              "path": [
                "api",
                "my/follows/shops/:slug"
              ],
              "variable": [
                {
                  "id": "slug",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post my follows shops slug."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae06e3ea-692a-46c3-b902-bf26899b50cd"
            }
          ]
        },
        {
          "id": "e6ec4eb8-7202-41e1-8887-c069a64d43c9",
          "name": "deleteMyFollowsShopsSlug",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reverb.com",
              "path": [
                "api",
                "my/follows/shops/:slug"
              ],
              "variable": [
                {
                  "id": "slug",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete my follows shops slug."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0662aee-a7ff-42b3-a80c-bc0d9fb266e1"
            }
          ]
        }
      ]
    },
    {
      "name": "Shops",
      "item": [
        {
          "id": "1c5d55f2-f884-4390-8120-f761f053d6e4",
          "name": "getShopsStorefronts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reverb.com",
              "path": [
                "api",
                "shops/:id/storefronts"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get storefront details on a shop."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32c661a0-a641-4cf3-9eb3-89300c32c343"
            }
          ]
        },
        {
          "id": "cc99b633-159d-48e8-8a6e-40a939ba6e6f",
          "name": "getShopsShopShippingProfiles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reverb.com",
              "path": [
                "api",
                "shops/:shop_id/shipping_profiles"
              ],
              "variable": [
                {
                  "id": "shop_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of shipping profiles for your shop"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04f974fd-b69d-416b-b4bf-7660baf81b5a"
            }
          ]
        },
        {
          "id": "1a95a629-32a5-4819-8c06-a783d6c51fcf",
          "name": "getShopsSlug",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reverb.com",
              "path": [
                "api",
                "shops/:slug"
              ],
              "query": [
                {
                  "key": "include_listing_count",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "slug",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get details on a shop."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64172d5f-b3c0-484f-9ffb-f9e27ca26b2f"
            }
          ]
        }
      ]
    }
  ]
}