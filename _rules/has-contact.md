---
x-tags:
- metadata
description: 'API MUST reference a contact, either url or email in #/info/contact'
given: $
severity: error
recommended: true
type: style
formats:
- oas3
then:
  field: info.contact
  function: truthy
...
- metadata
description: 'API MUST reference a contact, either url or email in #/info/contact'
given: $
severity: error
recommended: true
type: style
formats:
- oas3
then:
  field: info.contact
  function: truthy