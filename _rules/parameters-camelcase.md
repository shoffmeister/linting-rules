---
parameters-camelcase:
  description: Path and query parmeters must use camelCase.
  given: $..parameters[?(@.in=="query" || @.in=="path")]
  then:
    field: name
    function: casing
    functionOptions:
      type: camel
...
parameters-camelcase:
  description: Path and query parmeters must use camelCase.
  given: $..parameters[?(@.in=="query" || @.in=="path")]
  then:
    field: name
    function: casing
    functionOptions:
      type: camel