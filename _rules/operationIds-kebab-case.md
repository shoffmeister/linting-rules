---
description: Operation IDs MUST be written in kebab-case
message: '{{property}} is not kebab-case: {{error}}'
recommended: true
type: style
given: $.paths.*[?( @property === 'get' || @property === 'put' || @property === 'post'
  || @property === 'delete' || @property === 'options' || @property === 'head' ||
  @property === 'patch' || @property === 'trace' )]
then:
  field: operationId
  function: pattern
  functionOptions:
    match: ^([a-z0-9-]+)$
...
message: '{{property}} is not kebab-case: {{error}}'
recommended: true
type: style
given: $.paths.*[?( @property === 'get' || @property === 'put' || @property === 'post'
  || @property === 'delete' || @property === 'options' || @property === 'head' ||
  @property === 'patch' || @property === 'trace' )]
then:
  field: operationId
  function: pattern
  functionOptions:
    match: ^([a-z0-9-]+)$