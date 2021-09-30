--- 
response-forbidden-headers: 
  description: |-
      OAS do not allow using the following HTTP headers in a specification
      file Authorization, Content-Type and Accept. You MUST use the associate functionalities provided by OAS, instead.
  given: 
    - "$.[responses][*].headers.*~"
  message: "{{error}} in {{path}} {{value}}"
  severity: error
  then: 
    function: pattern
    functionOptions: 
      notMatch: /^(accept|content-type|authorization)$/i
  x-tags: 
    - standards   
...
response-forbidden-headers: 
  description: |-
      OAS do not allow using the following HTTP headers in a specification
      file Authorization, Content-Type and Accept. You MUST use the associate functionalities provided by OAS, instead.
  given: 
    - "$.[responses][*].headers.*~"
  message: "{{error}} in {{path}} {{value}}"
  severity: error
  then: 
    function: pattern
    functionOptions: 
      notMatch: /^(accept|content-type|authorization)$/i
  x-tags: 
    - standards 