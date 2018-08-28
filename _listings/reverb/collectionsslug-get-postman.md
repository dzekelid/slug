{
  "info": {
    "name": "reverb Get Collections Slug",
    "_postman_id": "8e81a4d8-d2a8-47b5-bec8-f5b613f2f5af",
    "description": "Get collections slug.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "My",
      "item": [
        {
          "id": "4b3e98b9-b79e-46b8-aa1c-ebace8cf0321",
          "name": "getMyFollowsCollectionsSlug",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reverb.com",
              "path": [
                "api",
                "my/follows/collections/:slug"
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
            "description": "Get my follows collections slug."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f864697-96d0-45db-828f-beafd9378b40"
            }
          ]
        },
        {
          "id": "c6700483-4f78-4cbb-97bb-abaadb9a28c5",
          "name": "postMyFollowsCollectionsSlug",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reverb.com",
              "path": [
                "api",
                "my/follows/collections/:slug"
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
            "description": "Post my follows collections slug."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "299a9c68-57c5-4a49-a590-9058e498ddb8"
            }
          ]
        },
        {
          "id": "fbd525d2-1771-4228-bdbb-cdd5cff1833e",
          "name": "deleteMyFollowsCollectionsSlug",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reverb.com",
              "path": [
                "api",
                "my/follows/collections/:slug"
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
            "description": "Delete my follows collections slug."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fd229550-1df5-430f-a0eb-cc70abbc6cdb"
            }
          ]
        }
      ]
    },
    {
      "name": "Collections",
      "item": [
        {
          "id": "98549a10-6431-49e9-ae99-52438c18b10f",
          "name": "getCollections",
          "request": {
            "url": "http://api.reverb.com/api/collections",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of curated collections"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e194cd2a-b605-4c2d-a016-b3a7b8a71f98"
            }
          ]
        },
        {
          "id": "d9bfd874-7eb5-484d-a11a-e05248de8238",
          "name": "getCollectionsSlug",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reverb.com",
              "path": [
                "api",
                "collections/:slug"
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
            "description": "Get collections slug."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e85fd022-8a33-42b1-803f-9571e0182fed"
            }
          ]
        }
      ]
    }
  ]
}