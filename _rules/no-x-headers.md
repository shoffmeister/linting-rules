---
no-x-headers:
  description: "Please do not use headers with X-"
  message: "Headers cannot start with X-, so please find a new name for {{property}}. More: https://tools.ietf.org/html/rfc6648"
  given: "$..parameters.[?(@.in === 'header')].name"
  then:
    function: pattern
    functionOptions:
      notMatch: '^(x|X)-'    
...
no-x-headers:
  description: "Please do not use headers with X-"
  message: "Headers cannot start with X-, so please find a new name for {{property}}. More: https://tools.ietf.org/html/rfc6648"
  given: "$..parameters.[?(@.in === 'header')].name"
  then:
    function: pattern
    functionOptions:
      notMatch: '^(x|X)-'      