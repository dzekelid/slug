---
name: Bitbucket
x-slug: bitbucket
description: Collaborate on code with inline comments and pull requests. Manage and
  share your Git repositories to build and ship software, as a team.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
x-kinRank: "8"
x-alexaRank: "901"
tags: Slug
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/apis.md
specificationVersion: "0.14"
apis:
- name: Bitbucket - Delete Repositories Username Repo Slug
  x-api-slug: repositoriesusernamerepo-slug-delete
  description: |-
    Deletes the repository. This is an irreversible operation.

    This does not affect its forks.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slug-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slug-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug
  x-api-slug: repositoriesusernamerepo-slug-get
  description: Returns the object describing this repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slug-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slug-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug
  x-api-slug: repositoriesusernamerepo-slug-parameters
  description: Parameters repositories username repo slug
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slug-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slug-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug
  x-api-slug: repositoriesusernamerepo-slug-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slug-post-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug
  x-api-slug: repositoriesusernamerepo-slug-put
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slug-put-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Branch Restrictions
  x-api-slug: repositoriesusernamerepo-slugbranchrestrictions-get
  description: |-
    Returns a paginated list of all branch restrictions on the
    repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugbranchrestrictions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugbranchrestrictions-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Branch Restrictions
  x-api-slug: repositoriesusernamerepo-slugbranchrestrictions-parameters
  description: Parameters repositories username repo slug branch restrictions
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugbranchrestrictions-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugbranchrestrictions-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Branch Restrictions
  x-api-slug: repositoriesusernamerepo-slugbranchrestrictions-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugbranchrestrictions-post-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Branch Restrictions
  x-api-slug: repositoriesusernamerepo-slugbranchrestrictionsid-delete
  description: Delete repositories username repo slug branch restrictions
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugbranchrestrictionsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugbranchrestrictionsid-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Branch Restrictions
  x-api-slug: repositoriesusernamerepo-slugbranchrestrictionsid-get
  description: Get repositories username repo slug branch restrictions
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugbranchrestrictionsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugbranchrestrictionsid-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Branch Restrictions
  x-api-slug: repositoriesusernamerepo-slugbranchrestrictionsid-parameters
  description: Parameters repositories username repo slug branch restrictions
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugbranchrestrictionsid-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugbranchrestrictionsid-parameters-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Branch Restrictions
  x-api-slug: repositoriesusernamerepo-slugbranchrestrictionsid-put
  description: |-
    Updates an existing branch restriction rule.

    Fields not present in the request body are ignored.

    See [`POST`](../../branch-restrictions#post) for details.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugbranchrestrictionsid-put-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Commit Node Approve
  x-api-slug: repositoriesusernamerepo-slugcommitnodeapprove-delete
  description: |-
    Redact the authenticated user's approval of the specified commit.

    This operation is only available to users that have explicit access to
    the repository. In contrast, just the fact that a repository is
    publicly accessible to users does not give them the ability to approve
    commits.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-delete-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Node Approve
  x-api-slug: repositoriesusernamerepo-slugcommitnodeapprove-parameters
  description: Parameters repositories username repo slug commit node approve
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Commit Node Approve
  x-api-slug: repositoriesusernamerepo-slugcommitnodeapprove-post
  description: |-
    Approve the specified commit as the authenticated user.

    This operation is only available to users that have explicit access to
    the repository. In contrast, just the fact that a repository is
    publicly accessible to users does not give them the ability to approve
    commits.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodeapprove-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Node Statuses
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatuses-get
  description: Returns all statuses (e.g. build results) for a specific commit.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatuses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatuses-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Node Statuses
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatuses-parameters
  description: Parameters repositories username repo slug commit node statuses
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatuses-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatuses-parameters-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Node Statuses
    Build
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatusesbuild-parameters
  description: Parameters repositories username repo slug commit node statuses build
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuild-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuild-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Commit Node Statuses Build
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatusesbuild-post
  description: |-
    Creates a new build status against the specified commit.

    If the specified key already exists, the existing status object will
    be overwritten.

    When creating a new commit status, you can use a URI template for the URL.
    Templates are URLs that contain variable names that Bitbucket will
    evaluate at runtime whenever the URL is displayed anywhere similar to
    parameter substitution in
    [Bitbucket Connect](https://developer.atlassian.com/bitbucket/concepts/context-parameters.html).
    For example, one could use `https://foo.com/builds/{repository.full_name}`
    which Bitbucket will turn into `https://foo.com/builds/foo/bar` at render time.
    The context variables available are `repository` and `commit`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuild-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuild-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Node Statuses Build
    Key
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatusesbuildkey-get
  description: Get repositories username repo slug commit node statuses build key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Node Statuses
    Build Key
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatusesbuildkey-parameters
  description: Parameters repositories username repo slug commit node statuses build
    key
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-parameters-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Commit Node Statuses Build
    Key
  x-api-slug: repositoriesusernamerepo-slugcommitnodestatusesbuildkey-put
  description: |-
    Used to update the current status of a build status object on the
    specific commit.

    This operation can also be used to change other properties of the
    build status:

    * `state`
    * `name`
    * `description`
    * `url`
    * `refname`

    The `key` cannot be changed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitnodestatusesbuildkey-put-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Revision
  x-api-slug: repositoriesusernamerepo-slugcommitrevision-get
  description: Get repositories username repo slug commit revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Revision
  x-api-slug: repositoriesusernamerepo-slugcommitrevision-parameters
  description: Parameters repositories username repo slug commit revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitrevision-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Sha Comments
  x-api-slug: repositoriesusernamerepo-slugcommitshacomments-get
  description: |-
    Returns the commit's comments.

    This includes both global and inline comments.

    The default sorting is oldest to newest and can be overridden with
    the `sort` query parameter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacomments-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Sha Comments
  x-api-slug: repositoriesusernamerepo-slugcommitshacomments-parameters
  description: Parameters repositories username repo slug commit sha comments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacomments-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacomments-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commit Sha Comments Comment
  x-api-slug: repositoriesusernamerepo-slugcommitshacommentscomment-id-get
  description: Get repositories username repo slug commit sha comments comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacommentscomment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacommentscomment-id-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commit Sha Comments
    Comment
  x-api-slug: repositoriesusernamerepo-slugcommitshacommentscomment-id-parameters
  description: Parameters repositories username repo slug commit sha comments comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacommentscomment-id-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitshacommentscomment-id-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commits
  x-api-slug: repositoriesusernamerepo-slugcommits-get
  description: |-
    These are the repository's commits. They are paginated and returned
    in reverse chronological order, similar to the output of `git log` and
    `hg log`. Like these tools, the DAG can be filtered.

    ## GET /repositories/{username}/{repo_slug}/commits/

    Returns all commits in the repo in topological order (newest commit
    first). All branches and tags are included (similar to
    `git log --all` and `hg log`).

    ## GET /repositories/{username}/{repo_slug}/commits/master

    Returns all commits on rev `master` (similar to `git log master`,
    `hg log master`).

    ## GET /repositories/{username}/{repo_slug}/commits/dev?exclude=master

    Returns all commits on ref `dev`, except those that are reachable on
    `master` (similar to `git log dev ^master`).

    ## GET /repositories/{username}/{repo_slug}/commits/?exclude=master

    Returns all commits in the repo that are not on master
    (similar to `git log --all ^master`).

    ## GET /repositories/{username}/{repo_slug}/commits/?include=foo&include=bar&exclude=fu&exclude=fubar

    Returns all commits that are on refs `foo` or `bar`, but not on `fu` or
    `fubar` (similar to `git log foo bar ^fu ^fubar`).

    Because the response could include a very large number of commits, it
    is paginated. Follow the 'next' link in the response to navigate to the
    next page of commits. As with other paginated resources, do not
    construct your own links.

    When the include and exclude parameters are more than can fit in a
    query string, clients can use a `x-www-form-urlencoded` POST instead.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommits-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commits
  x-api-slug: repositoriesusernamerepo-slugcommits-parameters
  description: Parameters repositories username repo slug commits
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommits-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommits-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Commits
  x-api-slug: repositoriesusernamerepo-slugcommits-post
  description: |-
    Identical to `GET /repositories/{username}/{repo_slug}/commits`,
    except that POST allows clients to place the include and exclude
    parameters in the request body to avoid URL length issues.

    **Note that this resource does NOT support new commit creation.**
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommits-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommits-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Commits Revision
  x-api-slug: repositoriesusernamerepo-slugcommitsrevision-get
  description: |-
    These are the repository's commits. They are paginated and returned
    in reverse chronological order, similar to the output of `git log` and
    `hg log`. Like these tools, the DAG can be filtered.

    ## GET /repositories/{username}/{repo_slug}/commits/

    Returns all commits in the repo in topological order (newest commit
    first). All branches and tags are included (similar to
    `git log --all` and `hg log`).

    ## GET /repositories/{username}/{repo_slug}/commits/master

    Returns all commits on rev `master` (similar to `git log master`,
    `hg log master`).

    ## GET /repositories/{username}/{repo_slug}/commits/dev?exclude=master

    Returns all commits on ref `dev`, except those that are reachable on
    `master` (similar to `git log dev ^master`).

    ## GET /repositories/{username}/{repo_slug}/commits/?exclude=master

    Returns all commits in the repo that are not on master
    (similar to `git log --all ^master`).

    ## GET /repositories/{username}/{repo_slug}/commits/?include=foo&include=bar&exclude=fu&exclude=fubar

    Returns all commits that are on refs `foo` or `bar`, but not on `fu` or
    `fubar` (similar to `git log foo bar ^fu ^fubar`).

    Because the response could include a very large number of commits, it
    is paginated. Follow the 'next' link in the response to navigate to the
    next page of commits. As with other paginated resources, do not
    construct your own links.

    When the include and exclude parameters are more than can fit in a
    query string, clients can use a `x-www-form-urlencoded` POST instead.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Commits Revision
  x-api-slug: repositoriesusernamerepo-slugcommitsrevision-parameters
  description: Parameters repositories username repo slug commits revision
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Commits Revision
  x-api-slug: repositoriesusernamerepo-slugcommitsrevision-post
  description: |-
    Identical to `GET /repositories/{username}/{repo_slug}/commits`,
    except that POST allows clients to place the include and exclude
    parameters in the request body to avoid URL length issues.

    **Note that this resource does NOT support new commit creation.**
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcommitsrevision-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Components
  x-api-slug: repositoriesusernamerepo-slugcomponents-get
  description: |-
    Returns the components that have been defined in the issue tracker.

    This resource is only available on repositories that have the issue
    tracker enabled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcomponents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcomponents-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Components
  x-api-slug: repositoriesusernamerepo-slugcomponents-parameters
  description: Parameters repositories username repo slug components
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcomponents-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcomponents-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Components Component
  x-api-slug: repositoriesusernamerepo-slugcomponentscomponent-id-get
  description: Get repositories username repo slug components component
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcomponentscomponent-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcomponentscomponent-id-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Components Component
  x-api-slug: repositoriesusernamerepo-slugcomponentscomponent-id-parameters
  description: Parameters repositories username repo slug components component
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcomponentscomponent-id-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugcomponentscomponent-id-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Default Reviewers
  x-api-slug: repositoriesusernamerepo-slugdefaultreviewers-get
  description: |-
    Returns the repository's default reviewers.

    These are the users that are automatically added as reviewers on every
    new pull request that is created.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewers-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Default Reviewers
  x-api-slug: repositoriesusernamerepo-slugdefaultreviewers-parameters
  description: Parameters repositories username repo slug default reviewers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewers-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewers-parameters-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Default Reviewers Target
    Username
  x-api-slug: repositoriesusernamerepo-slugdefaultreviewerstarget-username-delete
  description: Delete repositories username repo slug default reviewers target username
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewerstarget-username-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewerstarget-username-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Default Reviewers Target Username
  x-api-slug: repositoriesusernamerepo-slugdefaultreviewerstarget-username-get
  description: |-
    Returns the specified reviewer.

    This can be used to test whether a user is among the repository's
    default reviewers list. A 404 indicates that that specified user is not
    a default reviewer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewerstarget-username-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewerstarget-username-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Default Reviewers Target
    Username
  x-api-slug: repositoriesusernamerepo-slugdefaultreviewerstarget-username-parameters
  description: Parameters repositories username repo slug default reviewers target
    username
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewerstarget-username-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewerstarget-username-parameters-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Default Reviewers Target
    Username
  x-api-slug: repositoriesusernamerepo-slugdefaultreviewerstarget-username-put
  description: |-
    Adds the specified user to the repository's list of default
    reviewers.

    This method is idempotent. Adding a user a second time has no effect.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewerstarget-username-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdefaultreviewerstarget-username-put-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Diff Spec
  x-api-slug: repositoriesusernamerepo-slugdiffspec-get
  description: |-
    Produces a raw, git-style diff for either a single commit (diffed
    against its first parent), or a revspec of 2 commits (e.g.
    `3a8b42..9ff173` where the first commit represents the source and the
    second commit the destination).

    In case of the latter (diffing a revspec), a 3-way diff, or merge diff,
    is computed. This shows the changes introduced by the left branch
    (`3a8b42` in our example) as compared againt the right branch
    (`9ff173`).

    This is equivalent to merging the left branch into the right branch and
    then computing the diff of the merge commit against its first parent
    (the right branch). This follows the same behavior as pull requests
    that also show this style of 3-way, or merge diff.

    While similar to patches, diffs:

    * Don't have a commit header (username, commit message, etc)
    * Support the optional `path=foo/bar.py` query param to filter
      the diff to just that one file diff

    The raw diff is returned as-is, in whatever encoding the files in the
    repository use. It is not decoded into unicode. As such, the
    content-type is `text/plain`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdiffspec-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdiffspec-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Diff Spec
  x-api-slug: repositoriesusernamerepo-slugdiffspec-parameters
  description: Parameters repositories username repo slug diff spec
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdiffspec-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdiffspec-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Downloads
  x-api-slug: repositoriesusernamerepo-slugdownloads-get
  description: Returns a list of download links associated with the repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloads-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloads-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Downloads
  x-api-slug: repositoriesusernamerepo-slugdownloads-parameters
  description: Parameters repositories username repo slug downloads
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloads-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloads-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Downloads
  x-api-slug: repositoriesusernamerepo-slugdownloads-post
  description: |-
    Upload new download artifacts.

    To upload files, perform a `multipart/form-data` POST containing one
    or more `files` fields:

        $ echo Hello World > hello.txt
        $ curl -s -u evzijst -X POST https://api.bitbucket.org/2.0/repositories/evzijst/git-tests/downloads -F files=@hello.txt

    When a file is uploaded with the same name as an existing artifact,
    then the existing file will be replaced.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloads-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloads-post-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Downloads Filename
  x-api-slug: repositoriesusernamerepo-slugdownloadsfilename-delete
  description: Deletes the specified download artifact from the repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Downloads Filename
  x-api-slug: repositoriesusernamerepo-slugdownloadsfilename-get
  description: |-
    Return a redirect to the contents of a download artifact.

    This endpoint returns the actual file contents and not the artifact's
    metadata.

        $ curl -s -L https://api.bitbucket.org/2.0/repositories/evzijst/git-tests/downloads/hello.txt
        Hello World
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Downloads Filename
  x-api-slug: repositoriesusernamerepo-slugdownloadsfilename-parameters
  description: Parameters repositories username repo slug downloads filename
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugdownloadsfilename-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Forks
  x-api-slug: repositoriesusernamerepo-slugforks-get
  description: |-
    Returns a paginated list of all the forks of the specified
    repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugforks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugforks-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Forks
  x-api-slug: repositoriesusernamerepo-slugforks-parameters
  description: Parameters repositories username repo slug forks
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugforks-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugforks-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Hooks
  x-api-slug: repositoriesusernamerepo-slughooks-get
  description: Returns a paginated list of webhooks installed on this repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slughooks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slughooks-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Hooks
  x-api-slug: repositoriesusernamerepo-slughooks-parameters
  description: Parameters repositories username repo slug hooks
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slughooks-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slughooks-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Hooks
  x-api-slug: repositoriesusernamerepo-slughooks-post
  description: |-
    Creates a new webhook on the specified repository.

    Example:

    ```
    $ curl -X POST -u credentials -H 'Content-Type: application/json'           https://api.bitbucket.org/2.0/repositories/username/slug/hooks           -d '
        {
          "description": "Webhook Description",
          "url": "https://example.com/",
          "active": true,
          "events": [
            "repo:push",
            "issue:created",
            "issue:updated"
          ]
        }'
    ```

    Note that this call requires the webhook scope, as well as any scope
    that applies to the events that the webhook subscribes to. In the
    example above that means: `webhook`, `repository` and `issue`.

    Also note that the `url` must properly resolve and cannot be an
    internal, non-routed address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slughooks-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slughooks-post-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Hooks U
  x-api-slug: repositoriesusernamerepo-slughooksuid-delete
  description: |-
    Deletes the specified webhook subscription from the given
    repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slughooksuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slughooksuid-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Hooks U
  x-api-slug: repositoriesusernamerepo-slughooksuid-get
  description: |-
    Returns the webhook with the specified id installed on the specified
    repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slughooksuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slughooksuid-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Hooks U
  x-api-slug: repositoriesusernamerepo-slughooksuid-parameters
  description: Parameters repositories username repo slug hooks u
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slughooksuid-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slughooksuid-parameters-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Hooks U
  x-api-slug: repositoriesusernamerepo-slughooksuid-put
  description: |-
    Updates the specified webhook subscription.

    The following properties can be mutated:

    * `description`
    * `url`
    * `active`
    * `events`
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slughooksuid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slughooksuid-put-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Issues
  x-api-slug: repositoriesusernamerepo-slugissues-get
  description: Get repositories username repo slug issues
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissues-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissues-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Issues
  x-api-slug: repositoriesusernamerepo-slugissues-parameters
  description: Parameters repositories username repo slug issues
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissues-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissues-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Issues
  x-api-slug: repositoriesusernamerepo-slugissues-post
  description: |-
    Creates a new issue.

    This call requires authentication. Private repositories or private
    issue trackers require the caller to authenticate with an account that
    has appropriate authorisation.

    The authenticated user is used for the issue's `reporter` field.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissues-post-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Issues Issue
  x-api-slug: repositoriesusernamerepo-slugissuesissue-id-delete
  description: |-
    Deletes the specified issue. This requires write access to the
    repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-id-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Issues Issue
  x-api-slug: repositoriesusernamerepo-slugissuesissue-id-get
  description: Get repositories username repo slug issues issue
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-id-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Issues Issue
  x-api-slug: repositoriesusernamerepo-slugissuesissue-id-parameters
  description: Parameters repositories username repo slug issues issue
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-id-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-id-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Issues Issue  Attachments
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idattachments-get
  description: |-
    Returns all attachments for this issue.

    This returns the files' meta data. This does not return the files'
    actual contents.

    The files are always ordered by their upload date.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachments-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Issues Issue  Attachments
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idattachments-parameters
  description: Parameters repositories username repo slug issues issue  attachments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachments-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachments-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Issues Issue  Attachments
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idattachments-post
  description: |-
    Upload new issue attachments.

    To upload files, perform a `multipart/form-data` POST containing one
    or more file fields.

    When a file is uploaded with the same name as an existing attachment,
    then the existing file will be replaced.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachments-post-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Issues Issue  Attachments
    Path
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idattachmentspath-delete
  description: Delete repositories username repo slug issues issue  attachments path
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachmentspath-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachmentspath-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Issues Issue  Attachments
    Path
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idattachmentspath-get
  description: |-
    Returns the contents of the specified file attachment.

    Note that this endpoint does not return a JSON response, but instead
    returns a redirect pointing to the actual file that in turn will return
    the raw contents.

    The redirect URL contains a one-time token that has a limited lifetime.
    As a result, the link should not be persisted, stored, or shared.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachmentspath-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachmentspath-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Issues Issue  Attachments
    Path
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idattachmentspath-parameters
  description: Parameters repositories username repo slug issues issue  attachments
    path
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachmentspath-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idattachmentspath-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Issues Issue  Comments
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idcomments-get
  description: |-
    Returns all comments that were made on the specified issue.

    The default sorting is oldest to newest and can be overridden with
    the `sort` query parameter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idcomments-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Issues Issue  Comments
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idcomments-parameters
  description: Parameters repositories username repo slug issues issue  comments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idcomments-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idcomments-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Issues Issue  Comments Comment
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idcommentscomment-id-get
  description: Get repositories username repo slug issues issue  comments comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idcommentscomment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idcommentscomment-id-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Issues Issue  Comments
    Comment
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idcommentscomment-id-parameters
  description: Parameters repositories username repo slug issues issue  comments comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idcommentscomment-id-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idcommentscomment-id-parameters-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Issues Issue  Vote
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idvote-delete
  description: Delete repositories username repo slug issues issue  vote
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idvote-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idvote-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Issues Issue  Vote
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idvote-get
  description: |-
    Check whether the authenticated user has voted for this issue.
    A 204 status code indicates that the user has voted, while a 404
    implies they haven't.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idvote-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idvote-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Issues Issue  Vote
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idvote-parameters
  description: Parameters repositories username repo slug issues issue  vote
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idvote-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idvote-parameters-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Issues Issue  Vote
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idvote-put
  description: |-
    Vote for this issue.

    To cast your vote, do an empty PUT. The 204 status code indicates that
    the operation was successful.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idvote-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idvote-put-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Issues Issue  Watch
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idwatch-delete
  description: Delete repositories username repo slug issues issue  watch
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idwatch-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idwatch-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Issues Issue  Watch
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idwatch-get
  description: |-
    Indicated whether or not the authenticated user is watching this
    issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idwatch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idwatch-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Issues Issue  Watch
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idwatch-parameters
  description: Parameters repositories username repo slug issues issue  watch
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idwatch-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idwatch-parameters-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Issues Issue  Watch
  x-api-slug: repositoriesusernamerepo-slugissuesissue-idwatch-put
  description: |-
    Start watching this issue.

    To start watching this issue, do an empty PUT. The 204 status code
    indicates that the operation was successful.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idwatch-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugissuesissue-idwatch-put-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Milestones
  x-api-slug: repositoriesusernamerepo-slugmilestones-get
  description: |-
    Returns the milestones that have been defined in the issue tracker.

    This resource is only available on repositories that have the issue
    tracker enabled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugmilestones-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugmilestones-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Milestones
  x-api-slug: repositoriesusernamerepo-slugmilestones-parameters
  description: Parameters repositories username repo slug milestones
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugmilestones-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugmilestones-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Milestones Milestone
  x-api-slug: repositoriesusernamerepo-slugmilestonesmilestone-id-get
  description: Get repositories username repo slug milestones milestone
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugmilestonesmilestone-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugmilestonesmilestone-id-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Milestones Milestone
  x-api-slug: repositoriesusernamerepo-slugmilestonesmilestone-id-parameters
  description: Parameters repositories username repo slug milestones milestone
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugmilestonesmilestone-id-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugmilestonesmilestone-id-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Patch Spec
  x-api-slug: repositoriesusernamerepo-slugpatchspec-get
  description: |-
    Produces a raw patch for a single commit (diffed against its first
    parent), or a patch-series for a revspec of 2 commits (e.g.
    `3a8b42..9ff173` where the first commit represents the source and the
    second commit the destination).

    In case of the latter (diffing a revspec), a patch series is returned
    for the commits on the source branch (`3a8b42` and its ancestors in
    our example). For Mercurial, a single patch is returned that combines
    the changes of all commits on the source branch.

    While similar to diffs, patches:

    * Have a commit header (username, commit message, etc)
    * Do not support the `path=foo/bar.py` query parameter

    The raw patch is returned as-is, in whatever encoding the files in the
    repository use. It is not decoded into unicode. As such, the
    content-type is `text/plain`.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpatchspec-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpatchspec-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Patch Spec
  x-api-slug: repositoriesusernamerepo-slugpatchspec-parameters
  description: Parameters repositories username repo slug patch spec
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpatchspec-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpatchspec-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines
  x-api-slug: repositoriesusernamerepo-slugpipelines-get
  description: Get repositories username repo slug pipelines
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-get-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Pipelines
  x-api-slug: repositoriesusernamerepo-slugpipelines-post
  description: "Endpoint to create and initiate a pipeline. \nThere are a couple of
    different options to initiate a pipeline, where the payload of the request will
    determine which type of pipeline will be instantiated.\n# Trigger a Pipeline for
    a branch or tag\nOne way to trigger pipelines is by specifying the reference for
    which you want to trigger a pipeline (e.g. a branch or tag). \nThe specified reference
    will be used to determine which pipeline definition from the `bitbucket-pipelines.yml`
    file will be applied to initiate the pipeline. The pipeline will then do a clone
    of the repository and checkout the latest revision of the specified reference.\n\n###
    Example\n\n```\n$ curl -X POST -is -u username:password \\\n  -H 'Content-Type:
    application/json' \\\n https://api.bitbucket.org/2.0/repositories/jeroendr/meat-demo2/pipelines/
    \\\n  -d '\n  {\n    \"target\": {\n      \"ref_type\": \"branch\", \n      \"type\":
    \"pipeline_ref_target\", \n      \"ref_name\": \"master\"\n    }\n  }'\n```\n#
    Trigger a Pipeline for a commit on a branch or tag\nYou can initiate a pipeline
    for a specific commit and in the context of a specified reference (e.g. a branch,
    tag or bookmark).\nThe specified reference will be used to determine which pipeline
    definition from the bitbucket-pipelines.yml file will be applied to initiate the
    pipeline. The pipeline will clone the repository and then do a checkout the specified
    reference. \n\nThe following reference types are supported:\n\n* `branch` \n*
    `named_branch`\n* `bookmark` \n * `tag`\n\n### Example\n\n```\n$ curl -X POST
    -is -u username:password \\\n  -H 'Content-Type: application/json' \\\n  https://api.bitbucket.org/2.0/repositories/jeroendr/meat-demo2/pipelines/
    \\\n  -d '\n  {\n    \"target\": {\n      \"commit\": {\n        \"type\": \"commit\",
    \n        \"hash\": \"ce5b7431602f7cbba007062eeb55225c6e18e956\"\n      }, \n
    \     \"ref_type\": \"branch\", \n      \"type\": \"pipeline_ref_target\", \n
    \     \"ref_name\": \"master\"\n    }\n  }'\n```\n# Trigger a specific pipeline
    definition for a commit\nYou can trigger a specific pipeline that is defined in
    your `bitbucket-pipelines.yml` file for a specific commit. \nIn addition to the
    commit revision, you specify the type and pattern of the selector that identifies
    the pipeline definition. The resulting pipeline will then clone the repository
    and checkout the specified revision.\n\n### Example\n\n```\n$ curl -X POST -is
    -u username:password \\\n  -H 'Content-Type: application/json' \\\n https://api.bitbucket.org/2.0/repositories/jeroendr/meat-demo2/pipelines/
    \\\n -d '\n  {\n     \"target\": {\n      \"commit\": {\n         \"hash\":\"a3c4e02c9a3755eccdc3764e6ea13facdf30f923\",\n
    \        \"type\":\"commit\"\n       },\n        \"selector\": {\n           \"type\":\"custom\",\n
    \             \"pattern\":\"Deploy to production\"\n          },\n        \"type\":\"pipeline_commit_target\"\n
    \  }\n  }'\n```\n# Trigger a specific pipeline definition for a commit on a branch
    or tag\nYou can trigger a specific pipeline that is defined in your `bitbucket-pipelines.yml`
    file for a specific commit in the context of a specified reference. \nIn addition
    to the commit revision, you specify the type and pattern of the selector that
    identifies the pipeline definition, as well as the reference information. The
    resulting pipeline will then clone the repository a checkout the specified reference.\n\n###
    Example\n\n```\n$ curl -X POST -is -u username:password \\\n  -H 'Content-Type:
    application/json' \\\n https://api.bitbucket.org/2.0/repositories/jeroendr/meat-demo2/pipelines/
    \\\n -d '\n  {\n     \"target\": {\n      \"commit\": {\n         \"hash\":\"a3c4e02c9a3755eccdc3764e6ea13facdf30f923\",\n
    \        \"type\":\"commit\"\n       },\n       \"selector\": {\n          \"type\":
    \"custom\",\n          \"pattern\": \"Deploy to production\"\n       },\n       \"type\":
    \"pipeline_ref_target\",\n       \"ref_name\": \"master\",\n       \"ref_type\":
    \"branch\"\n     }\n  }'\n```"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuid-get
  description: Get repositories username repo slug pipelines pipeline uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuid-get-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidsteps-get
  description: Get repositories username repo slug pipelines pipeline uu steps
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidsteps-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidsteps-get-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps
    Step Uu
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuid-get
  description: Get repositories username repo slug pipelines pipeline uu steps step
    uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuid-get-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps
    Step Uu Log
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuidlog-get
  description: |-
    Retrieve the log file for a given step of a pipeline.

    This endpoint supports (and encourages!) the use of [HTTP Range requests](https://tools.ietf.org/html/rfc7233) to deal with potentially very large log files.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuidlog-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstepsstep-uuidlog-get-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Pipelines Pipeline Uu Stoppipeline
  x-api-slug: repositoriesusernamerepo-slugpipelinespipeline-uuidstoppipeline-post
  description: Signal the stop of a pipeline and all of its steps that not have completed
    yet.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstoppipeline-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelinespipeline-uuidstoppipeline-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Config
  x-api-slug: repositoriesusernamerepo-slugpipelines-config-get
  description: Get repositories username repo slug pipelines config
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-config-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-config-get-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Pipelines Config
  x-api-slug: repositoriesusernamerepo-slugpipelines-config-put
  description: Update the pipelines configuration for a repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-config-put-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Pipelines Config Ssh Key
    Pair
  x-api-slug: repositoriesusernamerepo-slugpipelines-configsshkey-pair-delete
  description: Delete repositories username repo slug pipelines config ssh key pair
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshkey-pair-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshkey-pair-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Config Ssh Key Pair
  x-api-slug: repositoriesusernamerepo-slugpipelines-configsshkey-pair-get
  description: Retrieve the repository SSH key pair excluding the SSH private key.
    The private key is a write only field and will never be exposed in the logs or
    the REST API.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshkey-pair-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshkey-pair-get-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Pipelines Config Ssh Key
    Pair
  x-api-slug: repositoriesusernamerepo-slugpipelines-configsshkey-pair-put
  description: Create or update the repository SSH key pair. The private key will
    be set as a default SSH identity in your build container.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshkey-pair-put-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Config Ssh Known
    Hosts
  x-api-slug: repositoriesusernamerepo-slugpipelines-configsshknown-hosts-get
  description: Get repositories username repo slug pipelines config ssh known hosts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshknown-hosts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshknown-hosts-get-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Pipelines Config Ssh Known
    Hosts
  x-api-slug: repositoriesusernamerepo-slugpipelines-configsshknown-hosts-post
  description: Post repositories username repo slug pipelines config ssh known hosts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshknown-hosts-post-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Pipelines Config Ssh Known
    Hosts Known Host Uu
  x-api-slug: repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-delete
  description: Delete repositories username repo slug pipelines config ssh known hosts
    known host uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Config Ssh Known
    Hosts Known Host Uu
  x-api-slug: repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-get
  description: Get repositories username repo slug pipelines config ssh known hosts
    known host uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-get-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Pipelines Config Ssh Known
    Hosts Known Host Uu
  x-api-slug: repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-put
  description: Put repositories username repo slug pipelines config ssh known hosts
    known host uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configsshknown-hostsknown-host-uuid-put-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Config Variables
  x-api-slug: repositoriesusernamerepo-slugpipelines-configvariables-get
  description: Get repositories username repo slug pipelines config variables
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configvariables-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configvariables-get-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Pipelines Config Variables
  x-api-slug: repositoriesusernamerepo-slugpipelines-configvariables-post
  description: Post repositories username repo slug pipelines config variables
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configvariables-post-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Pipelines Config Variables
    Variable Uu
  x-api-slug: repositoriesusernamerepo-slugpipelines-configvariablesvariable-uuid-delete
  description: Delete repositories username repo slug pipelines config variables variable
    uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configvariablesvariable-uuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configvariablesvariable-uuid-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pipelines Config Variables
    Variable Uu
  x-api-slug: repositoriesusernamerepo-slugpipelines-configvariablesvariable-uuid-get
  description: Get repositories username repo slug pipelines config variables variable
    uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configvariablesvariable-uuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configvariablesvariable-uuid-get-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Pipelines Config Variables
    Variable Uu
  x-api-slug: repositoriesusernamerepo-slugpipelines-configvariablesvariable-uuid-put
  description: Put repositories username repo slug pipelines config variables variable
    uu
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpipelines-configvariablesvariable-uuid-put-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pullrequests
  x-api-slug: repositoriesusernamerepo-slugpullrequests-get
  description: |-
    Returns a paginated list of all pull requests on the specified
    repository. By default only open pull requests are returned. This can
    be controlled using the `state` query parameter. To retrieve pull
    requests that are in one of multiple states, repeat the `state`
    parameter for each individual state.

    This endpoint also supports filtering and sorting of the results. See
    [filtering and sorting](../../../../meta/filtering) for more details.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequests-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequests-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Pullrequests
  x-api-slug: repositoriesusernamerepo-slugpullrequests-parameters
  description: Parameters repositories username repo slug pullrequests
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequests-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequests-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Pullrequests
  x-api-slug: repositoriesusernamerepo-slugpullrequests-post
  description: Post repositories username repo slug pullrequests
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequests-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pullrequests Activity
  x-api-slug: repositoriesusernamerepo-slugpullrequestsactivity-get
  description: |-
    Returns a paginated list of the pull request's activity log.

    This includes comments that were made by the reviewers, updates and
    approvals.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestsactivity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestsactivity-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Pullrequests Activity
  x-api-slug: repositoriesusernamerepo-slugpullrequestsactivity-parameters
  description: Parameters repositories username repo slug pullrequests activity
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestsactivity-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestsactivity-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pullrequests Pull Request
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-id-get
  description: Get repositories username repo slug pullrequests pull request
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-id-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Pullrequests Pull Request
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-id-parameters
  description: Parameters repositories username repo slug pullrequests pull request
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-id-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-id-parameters-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Pullrequests Pull Request
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-id-put
  description: |-
    Mutates the specified pull request.

    This can be used to change the pull request's branches or description.

    Only open pull requests can be mutated.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-id-put-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pullrequests Pull Request  Activity
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idactivity-get
  description: |-
    Returns a paginated list of the pull request's activity log.

    This includes comments that were made by the reviewers, updates and
    approvals.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idactivity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idactivity-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Pullrequests Pull Request  Activity
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idactivity-parameters
  description: Parameters repositories username repo slug pullrequests pull request  activity
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idactivity-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idactivity-parameters-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Pullrequests Pull Request  Approve
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idapprove-delete
  description: Delete repositories username repo slug pullrequests pull request  approve
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idapprove-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idapprove-delete-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Pullrequests Pull Request  Approve
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idapprove-parameters
  description: Parameters repositories username repo slug pullrequests pull request  approve
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idapprove-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idapprove-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Pullrequests Pull Request  Approve
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idapprove-post
  description: Post repositories username repo slug pullrequests pull request  approve
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idapprove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idapprove-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pullrequests Pull Request  Comments
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idcomments-get
  description: |-
    Returns a paginated list of the pull request's comments.

    This includes both global, inline comments and replies.

    The default sorting is oldest to newest and can be overridden with
    the `sort` query parameter.

    This endpoint also supports filtering and sorting of the results. See
    [filtering and sorting](../../../../../../meta/filtering) for more
    details.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcomments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcomments-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Pullrequests Pull Request  Comments
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idcomments-parameters
  description: Parameters repositories username repo slug pullrequests pull request  comments
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcomments-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcomments-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pullrequests Pull Request  Comments
    Comment
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idcommentscomment-id-get
  description: Get repositories username repo slug pullrequests pull request  comments
    comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcommentscomment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcommentscomment-id-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Pullrequests Pull Request  Comments
    Comment
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idcommentscomment-id-parameters
  description: Parameters repositories username repo slug pullrequests pull request  comments
    comment
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcommentscomment-id-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcommentscomment-id-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pullrequests Pull Request  Commits
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idcommits-get
  description: |-
    Returns a paginated list of the pull request's commits.

    These are the commits that are being merged into the destination
    branch when the pull requests gets accepted.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcommits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcommits-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Pullrequests Pull Request  Commits
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idcommits-parameters
  description: Parameters repositories username repo slug pullrequests pull request  commits
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcommits-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idcommits-parameters-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Pullrequests Pull Request  Decline
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-iddecline-parameters
  description: Parameters repositories username repo slug pullrequests pull request  decline
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-iddecline-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-iddecline-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Pullrequests Pull Request  Decline
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-iddecline-post
  description: Post repositories username repo slug pullrequests pull request  decline
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-iddecline-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-iddecline-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pullrequests Pull Request  Diff
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-iddiff-get
  description: Get repositories username repo slug pullrequests pull request  diff
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-iddiff-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-iddiff-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Pullrequests Pull Request  Diff
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-iddiff-parameters
  description: Parameters repositories username repo slug pullrequests pull request  diff
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-iddiff-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-iddiff-parameters-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Pullrequests Pull Request  Merge
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idmerge-parameters
  description: Parameters repositories username repo slug pullrequests pull request  merge
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idmerge-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idmerge-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Pullrequests Pull Request  Merge
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idmerge-post
  description: Post repositories username repo slug pullrequests pull request  merge
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idmerge-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pullrequests Pull Request  Patch
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idpatch-get
  description: Get repositories username repo slug pullrequests pull request  patch
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idpatch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idpatch-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Pullrequests Pull Request  Patch
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idpatch-parameters
  description: Parameters repositories username repo slug pullrequests pull request  patch
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idpatch-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idpatch-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Pullrequests Pull Request  Statuses
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idstatuses-get
  description: Get repositories username repo slug pullrequests pull request  statuses
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idstatuses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idstatuses-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Pullrequests Pull Request  Statuses
  x-api-slug: repositoriesusernamerepo-slugpullrequestspull-request-idstatuses-parameters
  description: Parameters repositories username repo slug pullrequests pull request  statuses
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idstatuses-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugpullrequestspull-request-idstatuses-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Refs
  x-api-slug: repositoriesusernamerepo-slugrefs-get
  description: Get repositories username repo slug refs
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefs-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Refs
  x-api-slug: repositoriesusernamerepo-slugrefs-parameters
  description: Parameters repositories username repo slug refs
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefs-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefs-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Refs Branches
  x-api-slug: repositoriesusernamerepo-slugrefsbranches-get
  description: Get repositories username repo slug refs branches
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefsbranches-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefsbranches-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Refs Branches
  x-api-slug: repositoriesusernamerepo-slugrefsbranches-parameters
  description: Parameters repositories username repo slug refs branches
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefsbranches-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefsbranches-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Refs Branches Name
  x-api-slug: repositoriesusernamerepo-slugrefsbranchesname-get
  description: Get repositories username repo slug refs branches name
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefsbranchesname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefsbranchesname-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Refs Branches Name
  x-api-slug: repositoriesusernamerepo-slugrefsbranchesname-parameters
  description: Parameters repositories username repo slug refs branches name
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefsbranchesname-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefsbranchesname-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Refs Tags
  x-api-slug: repositoriesusernamerepo-slugrefstags-get
  description: Get repositories username repo slug refs tags
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefstags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefstags-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Refs Tags
  x-api-slug: repositoriesusernamerepo-slugrefstags-parameters
  description: Parameters repositories username repo slug refs tags
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefstags-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefstags-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Refs Tags
  x-api-slug: repositoriesusernamerepo-slugrefstags-post
  description: |-
    Creates a new tag in the specified repository.

    The payload of the POST should consist of a JSON document that
    contains the name of the tag and the target hash.

    ```
    {
        "name" : "new tag name",
        "target" : {
            "hash" : "target commit hash",
        }
    }
    ```

    This endpoint does support using short hash prefixes for the commit
    hash, but it may return a 400 response if the provided prefix is
    ambiguous. Using a full commit hash is the preferred approach.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefstags-post-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Refs Tags Name
  x-api-slug: repositoriesusernamerepo-slugrefstagsname-get
  description: Get repositories username repo slug refs tags name
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefstagsname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefstagsname-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Refs Tags Name
  x-api-slug: repositoriesusernamerepo-slugrefstagsname-parameters
  description: Parameters repositories username repo slug refs tags name
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefstagsname-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugrefstagsname-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Src Node Path
  x-api-slug: repositoriesusernamerepo-slugsrcnodepath-get
  description: Get repositories username repo slug src node path
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugsrcnodepath-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugsrcnodepath-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Src Node Path
  x-api-slug: repositoriesusernamerepo-slugsrcnodepath-parameters
  description: Parameters repositories username repo slug src node path
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugsrcnodepath-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugsrcnodepath-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Versions
  x-api-slug: repositoriesusernamerepo-slugversions-get
  description: |-
    Returns the versions that have been defined in the issue tracker.

    This resource is only available on repositories that have the issue
    tracker enabled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugversions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugversions-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Versions
  x-api-slug: repositoriesusernamerepo-slugversions-parameters
  description: Parameters repositories username repo slug versions
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugversions-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugversions-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Versions Version
  x-api-slug: repositoriesusernamerepo-slugversionsversion-id-get
  description: Get repositories username repo slug versions version
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugversionsversion-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugversionsversion-id-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Versions Version
  x-api-slug: repositoriesusernamerepo-slugversionsversion-id-parameters
  description: Parameters repositories username repo slug versions version
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugversionsversion-id-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugversionsversion-id-parameters-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Watchers
  x-api-slug: repositoriesusernamerepo-slugwatchers-get
  description: |-
    Returns a paginated list of all the watchers on the specified
    repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugwatchers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugwatchers-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Watchers
  x-api-slug: repositoriesusernamerepo-slugwatchers-parameters
  description: Parameters repositories username repo slug watchers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugwatchers-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/slug/master/_listings/bitbucket/repositoriesusernamerepo-slugwatchers-parameters-openapi.md
x-common:
- type: x-api-gallery
  url: http://bigoven.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bitbucket.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/bitbucket
- type: x-developer
  url: https://developer.atlassian.com/cloud/bitbucket/
- type: x-documentation
  url: https://confluence.atlassian.com/bitbucket/bitbucket-cloud-documentation-221448814.html?_ga=2.77295890.629375793.1519179030-1077111323.1516485126
- type: x-status
  url: https://status.bitbucket.org/?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-support
  url: https://support.atlassian.com/bitbucket-cloud/
- type: x-terms-of-service
  url: https://www.atlassian.com/legal/customer-agreement?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-twitter
  url: https://twitter.com/bitbucket
- type: x-website
  url: http://bitbucket.org
- type: x-website
  url: https://bitbucket.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---