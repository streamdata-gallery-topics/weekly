---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite VWAP Get Historical Weekly VWAP
  description: Returns historical weekly VWAP information for a date range.
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetEventsForWeek:
    get:
      summary: Get Events For Week
      description: Get all the events released during the week specified. Weeks are
        Monday - Sunday.
      operationId: postGeteventsforweek
      x-api-path-slug: geteventsforweek-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Events
      - Week
  /GetGlobalHistoricalWeeklyQuotesRange:
    get:
      summary: Get Global Historical Weekly Quotes Range
      description: Returns a range of weekly Global Historical quotes for a security.
        For more information, go to http://www.xignite.com/
      operationId: postGetglobalhistoricalweeklyquotesrange
      x-api-path-slug: getglobalhistoricalweeklyquotesrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Global
      - Historical
      - Weekly
      - Quotes
      - Range
  /GetGlobalHistoricalWeeklyQuotesRangeExtended:
    get:
      summary: Get Global Historical Weekly Quotes Range Extended
      description: Returns a range of weekly Global Historical quotes extended for
        a security. For more information, go to http://www.xignite.com/
      operationId: postGetglobalhistoricalweeklyquotesrangeextended
      x-api-path-slug: getglobalhistoricalweeklyquotesrangeextended-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Global
      - Historical
      - Weekly
      - Quotes
      - Range
      - Extended
  /GetHistoricalWeeklyQuotesRangeAdjusted:
    get:
      summary: Get Historical Weekly Quotes Range Adjusted
      description: This operation returns end of week quotes for a US equity. This
        includes split and dividends adjusted price.
      operationId: postGethistoricalweeklyquotesrangeadjusted
      x-api-path-slug: gethistoricalweeklyquotesrangeadjusted-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Weekly
      - Quotes
      - Range
      - Adjusted
  /GetHistoricalWeeklyQuotesRange:
    get:
      summary: Get Historical Weekly Quotes Range
      description: This operation returns end of week quotes for a US equity. This
        includes split adjusted price.
      operationId: postGethistoricalweeklyquotesrange
      x-api-path-slug: gethistoricalweeklyquotesrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Weekly
      - Quotes
      - Range
  /GetHistoricalWeeklyRates:
    get:
      summary: Get Historical Weekly Rates
      description: Returns a rate for a range of dates.
      operationId: postGethistoricalweeklyrates
      x-api-path-slug: gethistoricalweeklyrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Weekly
      - Rates
  /GetHistoricalWeeklyVWAP:
    get:
      summary: Get Historical Weekly VWAP
      description: Returns historical weekly VWAP information for a date range.
      operationId: GetHistoricalWeeklyVWAP
      x-api-path-slug: gethistoricalweeklyvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Weekly
      - VWAP
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