---
description: The second path segment should be a whole-number version like `v1`.
given: $.paths
then:
  field: '@key'
  function: pattern
  functionOptions:
    match: ^/[^/]+/v\d+/.+$
...
given: $.paths
then:
  field: '@key'
  function: pattern
  functionOptions:
    match: ^/[^/]+/v\d+/.+$