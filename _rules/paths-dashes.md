---
paths-dashes:
  description: The URI template (RFC 6570 - https//tools.ietf.org/html/rfc6570) cannot
    contain a - character
  severity: error
  recommended: true
  message: '{{property}} {{description}}'
  given: $.paths[*]~
  then:
    function: pattern
    functionOptions:
      notMatch: /-/
...
paths-dashes:
  description: The URI template (RFC 6570 - https//tools.ietf.org/html/rfc6570) cannot
    contain a - character
  severity: error
  recommended: true
  message: '{{property}} {{description}}'
  given: $.paths[*]~
  then:
    function: pattern
    functionOptions:
      notMatch: /-/