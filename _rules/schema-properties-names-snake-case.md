---
schema-properties-names-snake-case:
  description: Schema property names should be snake case.
  message: Schema name should be snake case.
  severity: error
  given: $..properties.*
  then:
    field: "@key"
    function: casing
    functionOptions:
      type: snake
  x-status: validated
  x-tags:
      - Schema
      - Casing          
...
schema-properties-names-snake-case:
  description: Schema property names should be snake case.
  message: Schema name should be snake case.
  severity: error
  given: $..properties.*
  then:
    field: "@key"
    function: casing
    functionOptions:
      type: snake
  x-status: validated
  x-tags:
      - Schema
      - Casing  