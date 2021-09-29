---
description: Schema names should be Pascal case.
message: Schema name should be Pascal case.
severity: hint
formats:
- oas2
given: $.definitions.*~
then:
  function: casing
  functionOptions:
    type: pascal
...
message: Schema name should be Pascal case.
severity: hint
formats:
- oas2
given: $.definitions.*~
then:
  function: casing
  functionOptions:
    type: pascal