---
version-segment-second:
  description: The second path segment should be a whole-number version like v1.
  given: $.paths
  then:
    field: '@key'
    function: pattern
    functionOptions:
      match: ^/[^/]+/v\d+/.+$
...
version-segment-second:
  description: The second path segment should be a whole-number version like v1.
  given: $.paths
  then:
    field: '@key'
    function: pattern
    functionOptions:
      match: ^/[^/]+/v\d+/.+$