---
info-contact-name-and-url:
  description: Contact should have name and url properties.
  given: $.info.contact
  then:
  - field: name
    function: truthy
  - field: url
    function: truthy
...
info-contact-name-and-url:
  description: Contact should have name and url properties.
  given: $.info.contact
  then:
  - field: name
    function: truthy
  - field: url
    function: truthy