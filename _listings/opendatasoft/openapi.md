---
swagger: "2.0"
x-collection-name: OpenDataSoft
x-complete: 1
info:
  title: OpenDataSoft
  description: opendatasoft-is-a-cloudbased-turnkey-platform-for-data-publishing-and-api-management--its-interface-is-intuitively-designed-to-empower-anyone-regardless-of-technical-skills-to-upload-easytounderstand-open-data-or-to-even-share-data-within-an-admi---
  version: 2.1.0
host: public.opendatasoft.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /pages/{slug}:
    get:
      summary: Get Pages Slug
      description: A single page's metadata from this portal
      operationId: getPage
      x-api-path-slug: pagesslug-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Pages
      - Slug
---