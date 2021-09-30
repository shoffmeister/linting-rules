---
parameters-camelCase-alphanumeric-oas3:
  description: Path parameters MUST follow camelCase
  given: $..parameters[?(@.in == 'path')].name
  message: '{{property}} path parameter is not camelCase {{error}}'
  recommended: true
  severity: warn
  then:
    function: pattern
    functionOptions:
      match: ^[a-z][a-zA-Z0-9]+$
  x-tags:
    - Adidas      
...
parameters-camelCase-alphanumeric-oas3:
  description: Path parameters MUST follow camelCase
  given: $..parameters[?(@.in == 'path')].name
  message: '{{property}} path parameter is not camelCase {{error}}'
  recommended: true
  severity: warn
  then:
    function: pattern
    functionOptions:
      match: ^[a-z][a-zA-Z0-9]+$
  x-tags:
    - Adidas   