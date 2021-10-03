---
schema-properties-descriptions-length:
  description: The length of the description needs to be lest than 20 characters.
  message: The description length needs to be less than 20 characters {{ property }}.
  severity: warn
  formats:
  - oas3
  given: $..properties.*
  then:
    field: description
    function: length
    functionOptions: 
        max: 20
  x-status: validated
  x-tags:
      - Schema         
...
schema-properties-descriptions-length:
  description: The length of the description needs to be lest than 20 characters.
  message: The description length needs to be less than 20 characters {{ property }}.
  severity: warn
  formats:
  - oas3
  given: $..properties.*
  then:
    field: description
    function: length
    functionOptions: 
        max: 20
  x-status: validated
  x-tags:
      - Schema 