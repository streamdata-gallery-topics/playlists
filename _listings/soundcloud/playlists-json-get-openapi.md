---
swagger: "2.0"
x-collection-name: SoundCloud
x-complete: 0
info:
  title: Sound Cloud Get Playlists
  description: Returns a collection of playlists
  version: 1.0.0
host: api.soundcloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}/playlists.json:
    get:
      summary: Get Users Playlists
      description: Returns a collection of playlists created by user with user id
      operationId: getUsersUserPlaylists.json
      x-api-path-slug: usersuser-idplaylists-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Playlists
  /me/playlists.json:
    get:
      summary: Get Me Playlists
      description: Returns a collection of playlists created by the logged-in user
      operationId: getMePlaylists.json
      x-api-path-slug: meplaylists-json-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Playlists
  /playlists.json:
    get:
      summary: Get Playlists
      description: Returns a collection of playlists
      operationId: getPlaylists.json
      x-api-path-slug: playlists-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Playlists
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---