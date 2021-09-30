---
responses-have-default-oas3:
  description: All operations should have a default (error) response.
  message: Operation is missing a default response.
  severity: warn
  given: $.paths.*.*.responses
  then:
    field: default
    function: truthy
...
responses-have-default-oas3:
  description: All operations should have a default (error) response.
  message: Operation is missing a default response.
  severity: warn
  given: $.paths.*.*.responses
  then:
    field: default
    function: truthy