---
description: ALL requests MUST go through `https` protocol only
formats:
- oas2
given: $
message: Schemes MUST be https and no other value is allowed.
recommended: true
severity: error
then:
  field: schemes
  function: schema
  functionOptions:
    schema:
      items:
        enum:
        - https
        type: string
      maxItems: 1
      type: array
type: style
...
formats:
- oas2
given: $
message: Schemes MUST be https and no other value is allowed.
recommended: true
severity: error
then:
  field: schemes
  function: schema
  functionOptions:
    schema:
      items:
        enum:
        - https
        type: string
      maxItems: 1
      type: array
type: style