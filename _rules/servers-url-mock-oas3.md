---
servers-url-mock-oas3:
  description: Mock API server must be the first one so that Postman import uses it.
  severity: error
  formats:
  - oas3
  given: $.servers[0].url
  then:
    function: pattern
    functionOptions:
      match: http://localhost:4010
...
servers-url-mock-oas3:
  description: Mock API server must be the first one so that Postman import uses it.
  severity: error
  formats:
  - oas3
  given: $.servers[0].url
  then:
    function: pattern
    functionOptions:
      match: http://localhost:4010