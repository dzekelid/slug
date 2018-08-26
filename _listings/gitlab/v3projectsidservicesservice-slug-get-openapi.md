---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Get Projects Services Service Slug
  version: 1.0.0
  description: Get the service settings for project
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/services/{service_slug}:
    delete:
      summary: Delete Projects Services Service Slug
      description: Delete projects services service slug.
      operationId: deleteV3ProjectsIdServicesServiceSlug
      x-api-path-slug: v3projectsidservicesservice-slug-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: service_slug
        description: The name of the service
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Service
      - Slug
    get:
      summary: Get Projects Services Service Slug
      description: Get the service settings for project
      operationId: getV3ProjectsIdServicesServiceSlug
      x-api-path-slug: v3projectsidservicesservice-slug-get
      parameters:
      - in: path
        name: id
      - in: path
        name: service_slug
        description: The name of the service
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Services
      - Service
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