---
description: Parameters should be 'in' a location matching the prefix (Header.)
message: '''{{value}}'' does not match the parameter prefix. {{description}}. Fix
  by assigning the correct ''in'' value, eg. path -> header.'
given: $.components.parameters..[?(@property.match(/^Header\./))]
severity: error
then:
  field: in
  function: pattern
  functionOptions:
    match: ^header$
...
message: '''{{value}}'' does not match the parameter prefix. {{description}}. Fix
  by assigning the correct ''in'' value, eg. path -> header.'
given: $.components.parameters..[?(@property.match(/^Header\./))]
severity: error
then:
  field: in
  function: pattern
  functionOptions:
    match: ^header$