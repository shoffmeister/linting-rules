---
info-description-max-length:
  description: "The description must not be greater than 20 characters."
  given: "$.info"
  severity: error
  recommended: true
  type: style
  formats:
      - oas3
  then:
      field: description
      function: length
      functionOptions: 
        max: 20      
  x-status: validated
  x-tags:
    - Info
    - Length
...
info-description-max-length:
  description: "The description must not be greater than 20 characters."
  given: "$.info"
  severity: error
  recommended: true
  type: style
  formats:
      - oas3
  then:
      field: description
      function: length
      functionOptions: 
        max: 20      
  x-status: validated
  x-tags:
    - Info
    - Length 