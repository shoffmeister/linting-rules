---
description: A `GET` request MUST NOT accept a `body` parameter
severity: error
recommended: true
given: $.paths..get.parameters..in
then:
  function: pattern
  functionOptions:
    notMatch: /^body$/
...
severity: error
recommended: true
given: $.paths..get.parameters..in
then:
  function: pattern
  functionOptions:
    notMatch: /^body$/