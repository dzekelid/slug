swagger: "2.0"
x-collection-name: UserVoice
x-complete: 1
info:
  title: The Noun Project User API
  version: 1.0.0
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