---
request-bodies-json:
  description: Payload must be in json format
  message: Payload must be in JSON format, please correct the format for {{path}}.
  recommended: true
  type: style
  given: $.paths.*.*.requestBody.*
  severity: warn
  resolved: false
  then:
  - field: application/json
    function: truthy
...
request-bodies-json:
  description: Payload must be in json format
  message: Payload must be in JSON format, please correct the format for {{path}}.
  recommended: true
  type: style
  given: $.paths.*.*.requestBody.*
  severity: warn
  resolved: false
  then:
  - field: application/json
    function: truthy