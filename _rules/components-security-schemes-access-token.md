---
components-security-schemes-access-token:
  description: The access token is provided according to OIDC specifications
  message: type should be openIdConnect. {{description}}.
  given: $.components.securitySchemes[Oidc.AccessToken]
  severity: error
  then:
    field: type
    function: pattern
    functionOptions:
      match: ^openIdConnect$
...
components-security-schemes-access-token:
  description: The access token is provided according to OIDC specifications
  message: type should be openIdConnect. {{description}}.
  given: $.components.securitySchemes[Oidc.AccessToken]
  severity: error
  then:
    field: type
    function: pattern
    functionOptions:
      match: ^openIdConnect$