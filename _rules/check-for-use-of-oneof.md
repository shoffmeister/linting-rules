---
check-for-use-of-oneof:
  description: API Connect has a compatibility issue with the oneOf functionality.
  given: $..
  severity: warn
  then:
    field: oneOf
    function: falsy
...
check-for-use-of-oneof:
  description: API Connect has a compatibility issue with the oneOf functionality.
  given: $..
  severity: warn
  then:
    field: oneOf
    function: falsy