---
components-security-schemes-oauth-implicit:
  description: The API must contain the security mechanism OAuth2 implicit
  message: The API must contain the security mechanism type OAuth2 implicit
  recommended: true
  severity: error
  formats:
  - oas3
  type: style
  given: $
  then:
    field: $.components.securitySchemes.[*].flows.implicit
    function: truthy
...
components-security-schemes-oauth-implicit:
  description: The API must contain the security mechanism OAuth2 implicit
  message: The API must contain the security mechanism type OAuth2 implicit
  recommended: true
  severity: error
  formats:
  - oas3
  type: style
  given: $
  then:
    field: $.components.securitySchemes.[*].flows.implicit
    function: truthy