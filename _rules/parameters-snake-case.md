---
parameters-snake-case:
  message: Query parameters must be snake_case
  description: MUST use snake_case (never camelCase) for query parameters [130]
  documentationUrl: https://opensource.zalando.com/restful-api-guidelines/#130
  severity: error
  given: $.paths.*.*.parameters[?(@.in=='query')].name
  then:
    function: pattern
    functionOptions:
      match: ^[a-z][_a-z0-9]*$
...
parameters-snake-case:
  message: Query parameters must be snake_case
  description: MUST use snake_case (never camelCase) for query parameters [130]
  documentationUrl: https://opensource.zalando.com/restful-api-guidelines/#130
  severity: error
  given: $.paths.*.*.parameters[?(@.in=='query')].name
  then:
    function: pattern
    functionOptions:
      match: ^[a-z][_a-z0-9]*$