---
request-headers-x-prefix-oas3:
  description: Headers must start with X
  message: Headers must start with X-, so please find a new value for {{path}}.
  recommended: true
  type: style
  given: $..parameters.[?(@.in === 'header')].name
  severity: error
  resolved: false
  then:
    function: pattern
    functionOptions:
      match: ^(x|X)-
...
request-headers-x-prefix-oas3:
  description: Headers must start with X
  message: Headers must start with X-, so please find a new value for {{path}}.
  recommended: true
  type: style
  given: $..parameters.[?(@.in === 'header')].name
  severity: error
  resolved: false
  then:
    function: pattern
    functionOptions:
      match: ^(x|X)-