---
swagger: "2.0"
x-collection-name: International Trade Administration
x-complete: 0
info:
  title: ITA Offices And Centers ITA Offices and Centers Search
  description: This API provides contact and address information for all of ITAs domestic
    and international export assistance centers.
  termsOfService: http://developer.trade.gov/tos.html
  version: "1.0"
host: api.trade.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ita_office_locations/search:
    get:
      summary: ITA Offices and Centers Search
      description: This API provides contact and address information for all of ITAs
        domestic and international export assistance centers.
      operationId: office
      x-api-path-slug: ita-office-locationssearch-get
      parameters:
      - in: query
        name: city
        description: Returns office locations based on city name
      - in: query
        name: countries
        description: Returns office locations based on ISO alpha-2 country codes
      - in: query
        name: keyword
        description: Returns office locations for a match within the post or office
          name fields
      - in: query
        name: offset
        description: The offset parameter defines the offset from the first result
          you want to fetch
      - in: query
        name: size
        description: The size parameter allows you to configure the maximum amount
          of hits to be returned
      - in: query
        name: state
        description: Returns locations for export assistance centers located in a
          specific U
      responses:
        200:
          description: OK
      tags:
      - Offices
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