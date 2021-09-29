---
description: All JSON Schema properties MUST follow fields-camelCase and be ASCII
  alphanumeric characters or `_` or `$`.
given: $.definitions..properties[*]~
message: '{{property}} MUST follow camelCase and be ASCII alphanumeric characters
  or `_` or `$`.'
recommended: true
severity: error
then:
  function: pattern
  functionOptions:
    match: /^[a-z$_]{1}[A-Z09$_]*/
...
  alphanumeric characters or `_` or `$`.
given: $.definitions..properties[*]~
message: '{{property}} MUST follow camelCase and be ASCII alphanumeric characters
  or `_` or `$`.'
recommended: true
severity: error
then:
  function: pattern
  functionOptions:
    match: /^[a-z$_]{1}[A-Z09$_]*/