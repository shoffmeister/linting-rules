---
response-post-201-oas2:
  description: Using post for a create operation is discouraged.
  message: Using post for a create operation is discouraged.
  severity: warn
  formats:
  - oas2
  given: $.paths[*].post.responses
  then:
    field: "201"
    function: falsy
...
response-post-201-oas2:
  description: Using post for a create operation is discouraged.
  message: Using post for a create operation is discouraged.
  severity: warn
  formats:
  - oas2
  given: $.paths[*].post.responses
  then:
    field: "201"
    function: falsy