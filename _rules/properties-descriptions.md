---
description: all properties children should have a description
severity: error
given: $..properties.*
then:
  field: description
  function: truthy
...
severity: error
given: $..properties.*
then:
  field: description
  function: truthy