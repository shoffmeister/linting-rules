---
description: parameter name should be snake_case.
type: style
severity: error
given: $..get.parameters..name
then:
  function: casing
  functionOptions:
    type: snake
...
type: style
severity: error
given: $..get.parameters..name
then:
  function: casing
  functionOptions:
    type: snake