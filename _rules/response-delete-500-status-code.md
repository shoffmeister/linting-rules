---
response-delete-500-status-code:
  description: A delete operation should have a 500 response.
  message: A DELETE operation should have a 500 response.
  severity: warn
  formats:
  - oas2
  - oas3
  given: $.paths[*].delete.responses
  then:
    field: "500"
    function: truthy
  x-status: validated
  x-tags:
      - Methods
      - Status Codes       
...
response-delete-500-status-code:
  description: A delete operation should have a 500 response.
  message: A DELETE operation should have a 500 response.
  severity: warn
  formats:
  - oas2
  - oas3
  given: $.paths[*].delete.responses
  then:
    field: "500"
    function: truthy
  x-status: validated
  x-tags:
      - Methods
      - Status Codes  