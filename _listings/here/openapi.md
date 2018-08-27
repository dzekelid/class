swagger: "2.0"
x-collection-name: HERE
x-complete: 1
info:
  title: Weather API
  description: the-here-weather-api-provides-weather-forecasts-and-reports-on-current-weather-conditions-provides-information-on-severe-weather-alerts-provides-information-about-when-the-sun-and-moon-rise-and-set-and-the-phase-of-the-moonthis-example-set-works-with-version-1-2-4-or-higheradditional-information-can-be-found-on-developer-here-comhttpsdeveloper-here-comrestapisdocumentationweather
  version: 1.0.0
host: weather.cit.api.here.com
basePath: /weather/1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /6.1/flow.json:
    get:
      summary: Flow using Proximity returning Additional Attributes
      description: |-
        *Request traffic flow information using proximity, returning shape and functional class*

        The request is made through combining the `prox` parameter and the `responseattributes` in the request URL. The server also supports an XML response.



        * **prox**  `prox`
         \- A type of spatial filter. Proximity specifies a circle to search using a latitude, a longitude, and a radius in meters.    e.g. `52.515,13.377,100`

        * **responseattributes**  `multi-enum`
         \- A list indicating optional information to be included in the traffic flow data response

         Valid values are : `fc` - functionalClass, `sh` - shape

        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.
      operationId: 61FlowJsonGet7
      x-api-path-slug: 6-1flow-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: prox
      - in: query
        name: responseattributes
      responses:
        200:
          description: OK
      tags:
      - Flow
      - Using
      - Proximity
      - Returning
      - Itional
      - Attributes