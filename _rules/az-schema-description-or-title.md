---
description: All schemas should have a description or title.
message: Schema should have a description or title.
severity: warn
formats:
- oas2
- oas3
given:
- $.definitions[?(!@.description && !@.title)]
- $.components.schemas[?(!@.description && !@.title)]
then:
  function: falsy
...
message: Schema should have a description or title.
severity: warn
formats:
- oas2
- oas3
given:
- $.definitions[?(!@.description && !@.title)]
- $.components.schemas[?(!@.description && !@.title)]
then:
  function: falsy