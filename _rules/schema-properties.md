---
schema-properties:
  description: All schemas should have a properties.
  message: Should have schema properties {{ property }}.
  severity: error
  formats:
    - oas3
  given: $.components.schemas.*
  then:
      field: properties
      function: truthy
  x-status: validated
  x-tags:
      - Schema         
...
schema-properties:
  description: All schemas should have a properties.
  message: Should have schema properties {{ property }}.
  severity: error
  formats:
    - oas3
  given: $.components.schemas.*
  then:
      field: properties
      function: truthy
  x-status: validated
  x-tags:
      - Schema  