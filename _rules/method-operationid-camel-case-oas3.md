---
method-operationid-camel-case-oas3:
  description: OperationId must be camelCase in order to generate good method names
  severity: error
  given: $.paths.*.*.operationId
  then:
    function: pattern
    functionOptions:
      match: ^[a-z]+((\d)|([A-Z0-9][a-z0-9]+))*([A-Z])?$
...
method-operationid-camel-case-oas3:
  description: OperationId must be camelCase in order to generate good method names
  severity: error
  given: $.paths.*.*.operationId
  then:
    function: pattern
    functionOptions:
      match: ^[a-z]+((\d)|([A-Z0-9][a-z0-9]+))*([A-Z])?$