---
example-exists-in-parameters:
  description: All models MUST have a valid example.
  formats:
    - oas2
  given: $..parameters..[?(@.in == 'body' && (@.example || @.schema.$ref))]
  message: '{{ property }} MUST have a valid example.'
  recommended: true
  severity: error
  then:
    function: truthy
...
example-exists-in-parameters:
  description: All models MUST have a valid example.
  formats:
  - oas2
  given: $..parameters..[?(@.in == 'body' && (@.example || @.schema.$ref))]
  message: '{{ property }} MUST have a valid example.'
  recommended: true
  severity: error
  then:
    function: truthy