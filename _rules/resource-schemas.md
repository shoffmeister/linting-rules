---
severity: error
given: $..['application/json']
then:
  field: schema
  function: truthy
...
given: $..['application/json']
then:
  field: schema
  function: truthy