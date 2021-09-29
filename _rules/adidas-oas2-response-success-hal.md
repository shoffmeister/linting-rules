---
description: All success responses MUST be of media type `application/hal+json`
formats:
- oas2
given: $.paths..responses[?( @property >= 200 && @property < 300 && @property != 204)]
message: 'Response documents MUST follow application/hal+json: {{error}}'
recommended: true
severity: error
then:
  field: schema
  function: schema
  functionOptions:
    schema:
      $ref: ./supermodel/adidas/api/HAL.yaml
type: style
...
formats:
- oas2
given: $.paths..responses[?( @property >= 200 && @property < 300 && @property != 204)]
message: 'Response documents MUST follow application/hal+json: {{error}}'
recommended: true
severity: error
then:
  field: schema
  function: schema
  functionOptions:
    schema:
      $ref: ./supermodel/adidas/api/HAL.yaml
type: style