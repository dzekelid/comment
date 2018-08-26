---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Get Repositories Username Repo Slug Issues Issue  Comments Comment
  description: Get repositories username repo slug issues issue  comments comment
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
  /repositories/{username}/{repo_slug}/commit/{sha}/comments/{comment_id}:
    get:
      summary: Get Repositories Username Repo Slug Commit Sha Comments Comment
      description: Get repositories username repo slug commit sha comments comment
      operationId: getRepositoriesUsernameRepoSlugCommitShaCommentsComment
      x-api-path-slug: repositoriesusernamerepo-slugcommitshacommentscomment-id-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Commit
      - Sha
      - Comments
      - Comment
    parameters:
      summary: Parameters Repositories Username Repo Slug Commit Sha Comments Comment
      description: Parameters repositories username repo slug commit sha comments
        comment
      operationId: parametersRepositoriesUsernameRepoSlugCommitShaCommentsComment
      x-api-path-slug: repositoriesusernamerepo-slugcommitshacommentscomment-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Commit
      - Sha
      - Comments
      - Comment
  /repositories/{username}/{repo_slug}/issues/{issue_id}/comments/{comment_id}:
    get:
      summary: Get Repositories Username Repo Slug Issues Issue  Comments Comment
      description: Get repositories username repo slug issues issue  comments comment
      operationId: getRepositoriesUsernameRepoSlugIssuesIssueCommentsComment
      x-api-path-slug: repositoriesusernamerepo-slugissuesissue-idcommentscomment-id-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Issues
      - Issue
      - ""
      - Comments
      - Comment
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