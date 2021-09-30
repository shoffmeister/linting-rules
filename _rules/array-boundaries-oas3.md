---
array-boundaries-oas3:
  description: >-
    Array size should be limited to mitigate resource exhaustion attacks. This can be done using `maxItems` and `minItems`, like in the example below. You should ensure that the schema referenced in  `items` is constrained too.  If you delegate input validation to a library or framework, be sure to test it thoroughly and ensure that it verifies `maxItems`.
  message: Schema of type array must specify maxItems and minItems. {{path}} {{error}}
  formats:
    - oas3
  severity: warn
  recommended: true
  given:
    - $.[?(@.type=="array")]
  then:
    - field: maxItems
      function: defined
    - field: minItems
      function: defined     
  x-tags:
    - Arrays  
    - Security    
...
array-boundaries-oas3:
  description: >-
    Array size should be limited to mitigate resource exhaustion attacks. This can be done using `maxItems` and `minItems`, like in the example below. You should ensure that the schema referenced in  `items` is constrained too.  If you delegate input validation to a library or framework, be sure to test it thoroughly and ensure that it verifies `maxItems`.
  message: Schema of type array must specify maxItems and minItems. {{path}} {{error}}
  formats:
    - oas3
  severity: warn
  recommended: true
  given:
    - $.[?(@.type=="array")]
  then:
    - field: maxItems
      function: defined
    - field: minItems
      function: defined     
  x-tags:
    - Arrays  
    - Security 