---
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
severity: error
formats:
- oas3
given: $.servers[0].url
then:
  function: pattern
  functionOptions:
    match: http://localhost:4010