---
message: Enum values should be in UPPER_SNAKE_CASE format
description: SHOULD declare enum values using UPPER_SNAKE_CASE format [240]
documentationUrl: https://opensource.zalando.com/restful-api-guidelines/#240
severity: warn
given: $.paths..[?(@.type=='string')].[enum,x-extensible-enum].*
then:
  function: pattern
  functionOptions:
    match: ^[A-Z][A-Z_0-9]*$
...
description: SHOULD declare enum values using UPPER_SNAKE_CASE format [240]
documentationUrl: https://opensource.zalando.com/restful-api-guidelines/#240
severity: warn
given: $.paths..[?(@.type=='string')].[enum,x-extensible-enum].*
then:
  function: pattern
  functionOptions:
    match: ^[A-Z][A-Z_0-9]*$