---
description: Contact name should be `Manual`.
given: $.info.contact
then:
  field: name
  function: pattern
  functionOptions:
    match: ^Manual$
...
given: $.info.contact
then:
  field: name
  function: pattern
  functionOptions:
    match: ^Manual$