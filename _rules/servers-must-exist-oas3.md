---
servers-must-exist-oas3:
  description: OpenAPI servers must be present and non-empty array.
  severity: error
  formats:
    - oas3
  given: $
  then:
    field: servers
    function: schema
    functionOptions:
      schema:
        items:
          type: object
        minItems: 1
        type: array
  x-tags:
    - Tag        
...
servers-must-exist-oas3:
  description: OpenAPI servers must be present and non-empty array.
  severity: error
  formats:
    - oas3
  given: $
  then:
    field: servers
    function: schema
    functionOptions:
      schema:
        items:
          type: object
        minItems: 1
        type: array
  x-tags:
    - Tag 