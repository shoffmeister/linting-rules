---
paths-method-posts-id:
  severity: error
  description: Use PUT/PATCH rather than POSTing with a user-supplied identifier
  given: $.paths.[?(@property.toString().match(/[ -_]id}$|[a-z]Id}$/))]
  then:
    field: post
    function: falsy
...
paths-method-posts-id:
  severity: error
  description: Use PUT/PATCH rather than POSTing with a user-supplied identifier
  given: $.paths.[?(@property.toString().match(/[ -_]id}$|[a-z]Id}$/))]
  then:
    field: post
    function: falsy