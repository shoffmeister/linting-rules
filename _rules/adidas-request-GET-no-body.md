---
description: A 'GET' request MUST NOT accept a 'body` parameter
given: $.paths..get.parameters..in
severity: error
then:
  function: pattern
  functionOptions:
    notMatch: /^body$/
...
given: $.paths..get.parameters..in
severity: error
then:
  function: pattern
  functionOptions:
    notMatch: /^body$/