---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Delete Repositories Username Repo Slug Branch Restrictions
  description: Delete repositories username repo slug branch restrictions
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repositories/{username}/{repo_slug}:
    delete:
      summary: Delete Repositories Username Repo Slug
      description: |-
        Deletes the repository. This is an irreversible operation.

        This does not affect its forks.
      operationId: deleteRepositoriesUsernameRepoSlug
      x-api-path-slug: repositoriesusernamerepo-slug-delete
      parameters:
      - in: path
        name: repo_slug
        description: 'This can either be the repository slug or the UUID of the repository,surrounded
          by curly-braces, for example: `{repository UUID}`'
      - in: path
        name: username
        description: 'This can either be the username or the UUID of the user,surrounded
          by curly-braces, for example: `{user UUID}`'
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
    get:
      summary: Get Repositories Username Repo Slug
      description: Returns the object describing this repository.
      operationId: getRepositoriesUsernameRepoSlug
      x-api-path-slug: repositoriesusernamerepo-slug-get
      parameters:
      - in: path
        name: repo_slug
        description: 'This can either be the repository slug or the UUID of the repository,surrounded
          by curly-braces, for example: `{repository UUID}`'
      - in: path
        name: username
        description: 'This can either be the username or the UUID of the user,surrounded
          by curly-braces, for example: `{user UUID}`'
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
    parameters:
      summary: Parameters Repositories Username Repo Slug
      description: Parameters repositories username repo slug
      operationId: parametersRepositoriesUsernameRepoSlug
      x-api-path-slug: repositoriesusernamerepo-slug-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
    post:
      summary: Add Repositories Username Repo Slug
      description: |-
        Creates a new repository.

        Note: In order to set the project for the newly created repository,
        pass in either the project key or the project UUID as part of the
        request body as shown in the examples below:

        ```
        $ curl -X POST -H "Content-Type: application/json" -d '{
            "scm": "git",
            "project": {
                "key": "MARS"
            }
        }' https://api.bitbucket.org/2.0/repositories/teamsinspace/hablanding
        ```

        or

        ```
        $ curl -X POST -H "Content-Type: application/json" -d '{
            "scm": "git",
            "project": {
                "key": "{ba516952-992a-4c2d-acbd-17d502922f96}"
            }
        }' https://api.bitbucket.org/2.0/repositories/teamsinspace/hablanding
        ```

        The project must only be assigned for repositories belonging to a team.
        If the repository owner is a team and the project is not provided, the
        repository is automatically assigned to the oldest project in the team.

        Note: In the examples above, the username `teamsinspace`,
        and/or the repository name `hablanding` can be replaced by UUIDs.
      operationId: postRepositoriesUsernameRepoSlug
      x-api-path-slug: repositoriesusernamerepo-slug-post
      parameters:
      - in: path
        name: repo_slug
        description: 'This can either be the repository slug or the UUID of the repository,surrounded
          by curly-braces, for example: `{repository UUID}`'
      - in: path
        name: username
        description: 'This can either be the username or the UUID of the user,surrounded
          by curly-braces, for example: `{user UUID}`'
      - in: body
        name: _body
        description: The repository that is to be created
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
    put:
      summary: Update Repositories Username Repo Slug
      description: |-
        Since this endpoint can be used to both update and to create a
        repository, the request body depends on the intent.

        ### Creation

        See the POST documentation for the repository endpoint for an example
        of the request body.

        ### Update

        Note: Changing the `name` of the repository will cause the location to
        be changed. This is because the URL of the repo is derived from the
        name (a process called slugification). In such a scenario, it is
        possible for the request to fail if the newly created slug conflicts
        with an existing repository's slug. But if there is no conflict,
        the new location will be returned in the `Location` header of the
        response.
      operationId: putRepositoriesUsernameRepoSlug
      x-api-path-slug: repositoriesusernamerepo-slug-put
      parameters:
      - in: path
        name: repo_slug
        description: 'This can either be the repository slug or the UUID of the repository,surrounded
          by curly-braces, for example: `{repository UUID}`'
      - in: path
        name: username
        description: 'This can either be the username or the UUID of the user,surrounded
          by curly-braces, for example: `{user UUID}`'
      - in: body
        name: _body
        description: The repository that is to be updated
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
  /repositories/{username}/{repo_slug}/branch-restrictions:
    get:
      summary: Get Repositories Username Repo Slug Branch Restrictions
      description: |-
        Returns a paginated list of all branch restrictions on the
        repository.
      operationId: getRepositoriesUsernameRepoSlugBranchRestrictions
      x-api-path-slug: repositoriesusernamerepo-slugbranchrestrictions-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Branch
      - Restrictions
    parameters:
      summary: Parameters Repositories Username Repo Slug Branch Restrictions
      description: Parameters repositories username repo slug branch restrictions
      operationId: parametersRepositoriesUsernameRepoSlugBranchRestrictions
      x-api-path-slug: repositoriesusernamerepo-slugbranchrestrictions-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Branch
      - Restrictions
    post:
      summary: Add Repositories Username Repo Slug Branch Restrictions
      description: |-
        Creates a new branch restriction rule for a repository.

        `kind` describes what will be restricted. Allowed values are: `push`,
        `force`, `delete`, and `restrict_merges`.

        Different kinds of branch restrictions have different requirements:

        * `push` and `restrict_merges` require `users` and `groups` to be
          specified. Empty lists are allowed, in which case permission is
          denied for everybody.
        * `force` can not be specified in a Mercurial repository.

        `pattern` is used to determine which branches will be restricted.

        A `'*'` in `pattern` will expand to match zero or more characters, and
        every other character matches itself. For example, `'foo*'` will match
        `'foo'` and `'foobar'`, but not `'barfoo'`. `'*'` will match all
        branches.

        `users` and `groups` are lists of user names and group names.

        `kind` and `pattern` must be unique within a repository; adding new
        users or groups to an existing restriction should be done via `PUT`.

        Note that branch restrictions with overlapping patterns are allowed,
        but the resulting behavior may be surprising.
      operationId: postRepositoriesUsernameRepoSlugBranchRestrictions
      x-api-path-slug: repositoriesusernamerepo-slugbranchrestrictions-post
      parameters:
      - in: body
        name: _body
        description: The new rule
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Branch
      - Restrictions
  /repositories/{username}/{repo_slug}/branch-restrictions/{id}:
    delete:
      summary: Delete Repositories Username Repo Slug Branch Restrictions
      description: Delete repositories username repo slug branch restrictions
      operationId: deleteRepositoriesUsernameRepoSlugBranchRestrictions
      x-api-path-slug: repositoriesusernamerepo-slugbranchrestrictionsid-delete
      parameters:
      - in: path
        name: id
        description: The restriction rules id
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Branch
      - Restrictions
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