---
has-x-audience:
  message: Missing info.x-audience.
  description: MUST contain API meta information [218]
  documentationUrl: https://opensource.zalando.com/restful-api-guidelines/#218
  severity: error
  given: $.info
  then:
    field: x-audience
    function: truthy
...
has-x-audience:
  message: Missing info.x-audience.
  description: MUST contain API meta information [218]
  documentationUrl: https://opensource.zalando.com/restful-api-guidelines/#218
  severity: error
  given: $.info
  then:
    field: x-audience
    function: truthy