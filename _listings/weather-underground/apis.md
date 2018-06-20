---
name: Weather Underground
x-slug: weather-underground
description: Weather Underground provides local & long range weather forecasts, weather
  reports, maps & tropical weather conditions for locations worldwide.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/966-weather-underground.jpg
x-kinRank: "10"
x-alexaRank: "619"
tags: History
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/weather-underground/apis.md
specificationVersion: "0.14"
apis:
- name: Weather Underground Get Key History 20101018 Q Sfo
  x-api-slug: weather-underground
  description: This example will return historical data for San Francisco, California
    for the specified date.    If you search by zip or lat/long you will get nearest
    airport.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/966-weather-underground.jpg
  humanURL: http://www.wunderground.com
  baseURL: https://api.wunderground.com//api///{key}/history_20101018/q/SFO.json
  tags: Weather,Key,History,20101018,Q,SFO,Json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/weather-underground/keyhistory-20101018qsfo-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/weather-underground/keyhistory-20101018qsfo-json-get-openapi.md
- name: Weather Underground Get Key History 20101018 Q Pws Kcasanfr14
  x-api-slug: weather-underground
  description: This example will return historical data for a Personal Weather Station
    for the specified date.    The feature only works with JSON.    XML will come
    out soon.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/966-weather-underground.jpg
  humanURL: http://www.wunderground.com
  baseURL: https://api.wunderground.com//api///{key}/history_20101018/q/pws:KCASANFR14.json
  tags: Weather,Key,History,20101018,Q,Pws:KCASANFR14,Json
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/weather-underground/keyhistory-20101018qpwskcasanfr14-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/weather-underground/keyhistory-20101018qpwskcasanfr14-json-get-openapi.md
- name: Weather Underground
  x-api-slug: weather-underground
  description: Weather Underground provides local & long range weather forecasts,
    weather reports, maps & tropical weather conditions for locations worldwide.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/966-weather-underground.jpg
  humanURL: http://www.wunderground.com
  baseURL: https://api.wunderground.com//api/
  tags: History
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/history/master/_listings/weather-underground/openapi.md
x-common:
- type: x-application-gallery
  url: http://www.wunderground.com/weather/api/d/featured_applications.html
- type: x-crunchbase
  url: https://crunchbase.com/organization/weather-underground
- type: x-crunchbase
  url: http://www.crunchbase.com/company/weather-underground
- type: x-developer
  url: http://www.wunderground.com/weather/api
- type: x-email
  url: help@wunderground.com
- type: x-email
  url: press@wunderground.com
- type: x-email
  url: ademail@wunderground.com
- type: x-email
  url: wuhelp@wunderground.com
- type: x-forum
  url: http://www.wunderground.com/weather/api/d/community.html
- type: x-knowledgebase
  url: http://help.wunderground.com/knowledgebase
- type: x-pricing
  url: http://www.wunderground.com/weather/api/d/pricing.html
- type: x-privacy
  url: http://www.wunderground.com/members/tos.asp#privacy
- type: x-selfservice-registration
  url: http://www.wunderground.com/weather/api/d/login.html
- type: x-terms-of-service
  url: http://www.wunderground.com/members/tos.asp
- type: x-twitter
  url: https://twitter.com/wunderground
- type: x-twitter
  url: https://twitter.com/weatherapi
- type: x-website
  url: http://www.wunderground.com
- type: x-website
  url: http://wunderground.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---