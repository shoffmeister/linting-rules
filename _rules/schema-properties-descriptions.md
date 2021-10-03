---
schema-properties-descriptions:
  description: All schemas properties should have a description.
  message: Should have schema property {{ property }}.
  severity: warn
  formats:
  - oas3
  given: $..properties.*
  then:
      field: description
      function: truthy
  x-status: validated
  x-tags:
      - Schema         
...
schema-properties-descriptions:
  description: All schemas properties should have a description.
  message: Should have schema property {{ property }}.
  severity: warn
  formats:
  - oas3
  given: $..properties.*
  then:
      field: description
      function: truthy
  x-status: validated
  x-tags:
      - Schema  