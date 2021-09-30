---
request-body-not-allowed-oas2:
  description: A get or delete operation must not accept a body parameter.
  severity: error
  formats:
  - oas2
  given:
  - $.paths[*].[get,delete].parameters[*]
  then:
    field: in
    function: pattern
    functionOptions:
      notMatch: /^body$/
...
request-body-not-allowed-oas2:
  description: A get or delete operation must not accept a body parameter.
  severity: error
  formats:
  - oas2
  given:
  - $.paths[*].[get,delete].parameters[*]
  then:
    field: in
    function: pattern
    functionOptions:
      notMatch: /^body$/