---
description: OperationId should be pascalCased.
given: $.paths.[*][get,post,put,delete,options]
then:
  field: operationId
  function: casing
  functionOptions:
    type: pascal
type: style
...
given: $.paths.[*][get,post,put,delete,options]
then:
  field: operationId
  function: casing
  functionOptions:
    type: pascal
type: style