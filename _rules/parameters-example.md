---
parameters-example:
  description: "Parameters must have a example."
  given: $.paths.*.*.parameters[?(@.example=='query')]
  then:
    - field: example
      function: truthy
    - field: examples
      function: truthy      
  x-status: validated
  x-tags:
    - Parameters      
    - Examples
...
parameters-example:
  description: "Parameters must have a example."
  given: $.paths.*.*.parameters[?(@.example=='query')]
  then:
    - field: example
      function: truthy
    - field: examples
      function: truthy  
  x-status: validated
  x-tags:
    - Parameters      
    - Examples     