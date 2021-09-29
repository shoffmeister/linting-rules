---
message: Operation must use problem json as default response
description: MUST specify success and error responses [151]
documentationUrl: https://opensource.zalando.com/restful-api-guidelines/#151
severity: error
given: $.paths.*.*.responses.default
then:
  field: content.application/problem+json
  function: truthy
...
description: MUST specify success and error responses [151]
documentationUrl: https://opensource.zalando.com/restful-api-guidelines/#151
severity: error
given: $.paths.*.*.responses.default
then:
  field: content.application/problem+json
  function: truthy