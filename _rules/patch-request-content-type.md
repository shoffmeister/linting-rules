---
severity: error
description: '`PATCH` requests cannot use `application/json`'
given: $.paths.*.[?(@property == 'patch')].requestBody.content[?(@property == 'application/json')]^
then:
  function: falsy
...
description: '`PATCH` requests cannot use `application/json`'
given: $.paths.*.[?(@property == 'patch')].requestBody.content[?(@property == 'application/json')]^
then:
  function: falsy