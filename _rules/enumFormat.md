---
description: Must be in upper snake case
message: '{{error}}'
recommended: true
type: style
given: $.[?(/~*/.test(@.enum))].enum
severity: warn
resolved: false
then:
  function: checkEnum
...
message: '{{error}}'
recommended: true
type: style
given: $.[?(/~*/.test(@.enum))].enum
severity: warn
resolved: false
then:
  function: checkEnum