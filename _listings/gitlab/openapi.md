---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
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
---