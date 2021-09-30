--- 
operations-operationids-kebab-case:
  description: "Operation IDs MUST be written in kebab-case"
  given: "$.paths.*[?( @property === 'get' || @property === 'put' || @property === 'post' || @property === 'delete' || @property === 'options' || @property === 'head' || @property === 'patch' || @property === 'trace' )]"
  message: "{{property}} is not kebab-case {{error}}"
  recommended: true
  then: 
    field: operationId
    function: pattern
    functionOptions: 
      match: "^([a-z0-9-]+)$"
  type: style
...
operations-operationids-kebab-case:
  description: "Operation IDs MUST be written in kebab-case"
  given: "$.paths.*[?( @property === 'get' || @property === 'put' || @property === 'post' || @property === 'delete' || @property === 'options' || @property === 'head' || @property === 'patch' || @property === 'trace' )]"
  message: "{{property}} is not kebab-case {{error}}"
  recommended: true
  then: 
    field: operationId
    function: pattern
    functionOptions: 
      match: "^([a-z0-9-]+)$"
  type: style