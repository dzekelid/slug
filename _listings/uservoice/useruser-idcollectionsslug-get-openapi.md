---
swagger: "2.0"
x-collection-name: UserVoice
x-complete: 0
info:
  title: The Noun Project User API Get user collection
  version: 1.0.0
  description: Returns a single collection associated with a user
host: /user
basePath: http://api.thenounproject.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/{user_id}/collections/{slug}:
    get:
      summary: Get user collection
      description: Returns a single collection associated with a user
      operationId: getUserCollection
      x-api-path-slug: useruser-idcollectionsslug-get
      parameters:
      - in: path
        name: slug
        description: Collection slug
      - in: path
        name: user_id
        description: User id
      responses:
        200:
          description: OK
      tags:
      - User
      - User
      - Id
      - Collections
      - Slug
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---