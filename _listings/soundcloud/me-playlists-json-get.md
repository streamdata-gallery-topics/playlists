---
swagger: "2.0"
info:
  title: SoundCloud Get My Playlists
  description: Returns a collection of playlists created by the logged-in user
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
  /me/playlists.json:
    get:
      summary: Get My Playlists
      description: Returns a collection of playlists created by the logged-in user
      operationId: me.playlists.json.get
      responses:
        200:
          description: OK
      tags:
      - audio
      - me
      - playlists
definitions: []
x-collection-name: SoundCloud
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