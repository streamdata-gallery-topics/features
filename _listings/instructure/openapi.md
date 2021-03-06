swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/features:
    get:
      summary: List features
      description: List features.
      operationId: list-features
      x-api-path-slug: coursescourse-idfeatures-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Features
  /courses/{course_id}/features/enabled:
    get:
      summary: List enabled features
      description: List enabled features.
      operationId: list-enabled-features
      x-api-path-slug: coursescourse-idfeaturesenabled-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Features
      - Enabled
  /courses/{course_id}/features/flags/feature:
    delete:
      summary: Remove feature flag
      description: Remove feature flag.
      operationId: remove-feature-flag
      x-api-path-slug: coursescourse-idfeaturesflagsfeature-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Features
      - Flags
      - Feature
    get:
      summary: Get feature flag
      description: Get feature flag.
      operationId: get-feature-flag
      x-api-path-slug: coursescourse-idfeaturesflagsfeature-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Features
      - Flags
      - Feature
    put:
      summary: Set feature flag
      description: Set feature flag.
      operationId: set-feature-flag
      x-api-path-slug: coursescourse-idfeaturesflagsfeature-put
      parameters:
      - in: query
        name: locking_account_id
        description: If set, this FeatureFlag may only be modified by someone withnadministrative
          rights in the specified account
      - in: query
        name: state
        description: u201coffu201dnnThe feature is not available for the course, user,
          or account andnsub-accounts
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Features
      - Flags
      - Feature
  /users/{user_id}/features:
    get:
      summary: List features
      description: List features.
      operationId: list-features
      x-api-path-slug: usersuser-idfeatures-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Features
  /users/{user_id}/features/enabled:
    get:
      summary: List enabled features
      description: List enabled features.
      operationId: list-enabled-features
      x-api-path-slug: usersuser-idfeaturesenabled-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Features
      - Enabled
  /users/{user_id}/features/flags/feature:
    delete:
      summary: Remove feature flag
      description: Remove feature flag.
      operationId: remove-feature-flag
      x-api-path-slug: usersuser-idfeaturesflagsfeature-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Features
      - Flags
      - Feature
    get:
      summary: Get feature flag
      description: Get feature flag.
      operationId: get-feature-flag
      x-api-path-slug: usersuser-idfeaturesflagsfeature-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Features
      - Flags
      - Feature
    put:
      summary: Set feature flag
      description: Set feature flag.
      operationId: set-feature-flag
      x-api-path-slug: usersuser-idfeaturesflagsfeature-put
      parameters:
      - in: query
        name: locking_account_id
        description: If set, this FeatureFlag may only be modified by someone withnadministrative
          rights in the specified account
      - in: query
        name: state
        description: u201coffu201dnnThe feature is not available for the course, user,
          or account andnsub-accounts
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Features
      - Flags
      - Feature