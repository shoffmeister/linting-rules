---
message: Missing `info.contact.name`.
description: MUST contain API meta information [218]
documentationUrl: https://opensource.zalando.com/restful-api-guidelines/#218
severity: error
given: $.info
then:
  field: contact.name
  function: truthy
...
description: MUST contain API meta information [218]
documentationUrl: https://opensource.zalando.com/restful-api-guidelines/#218
severity: error
given: $.info
then:
  field: contact.name
  function: truthy