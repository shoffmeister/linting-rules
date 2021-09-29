---
description: Operation summary should be short and sweet, no full stops, and less
  than 20 characters
recommended: true
type: style
given: $.paths.*[?( @property === 'get' || @property === 'put' || @property === 'post'
  || @property === 'delete' || @property === 'options' || @property === 'head' ||
  @property === 'patch' || @property === 'trace' )]
then:
- field: summary
  function: pattern
  functionOptions:
    notMatch: \.
- field: summary
  function: length
  functionOptions:
    max: 20
...
  than 20 characters
recommended: true
type: style
given: $.paths.*[?( @property === 'get' || @property === 'put' || @property === 'post'
  || @property === 'delete' || @property === 'options' || @property === 'head' ||
  @property === 'patch' || @property === 'trace' )]
then:
- field: summary
  function: pattern
  functionOptions:
    notMatch: \.
- field: summary
  function: length
  functionOptions:
    max: 20