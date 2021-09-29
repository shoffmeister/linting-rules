---
description: |-
  Cache usage SHOULD be extensively detailed in the `description` property
  to avoid data leaks or the usage of stale data.

  This rule should ensure in some way that the api provider
  documented extensively the cache usage to avoid data leaks
  or usage of stale data.

  For now this ruleset tests:
  * the presence of following keywords
    in the `description`: `max-age`, `private`, `no-store`, `no-cache`.
  * that one and only one between Expires and Cache-Control is used.

  `Cache-Control` and `Expires` should not be used in conjuction,
  because `Cache-Control` overrides `Expires` when `max-age` is set.
  Instead if neither `Cache-Control` or `Expires` are set, clients MAY use euristic cache
  like described in RFC7234.
message: Cache usage SHOULD be documented when used.
formats:
- oas3
severity: warn
recommended: true
given: $..[parameters][?(@.in == "header" && @.name.match(/Cache-Control/i))]
then:
- field: description
  function: truthy
- field: description
  function: pattern
  functionOptions:
    match: .*(max-age|private|no-store|no-cache).*
...
  Cache usage SHOULD be extensively detailed in the `description` property
  to avoid data leaks or the usage of stale data.

  This rule should ensure in some way that the api provider
  documented extensively the cache usage to avoid data leaks
  or usage of stale data.

  For now this ruleset tests:
  * the presence of following keywords
    in the `description`: `max-age`, `private`, `no-store`, `no-cache`.
  * that one and only one between Expires and Cache-Control is used.

  `Cache-Control` and `Expires` should not be used in conjuction,
  because `Cache-Control` overrides `Expires` when `max-age` is set.
  Instead if neither `Cache-Control` or `Expires` are set, clients MAY use euristic cache
  like described in RFC7234.
message: Cache usage SHOULD be documented when used.
formats:
- oas3
severity: warn
recommended: true
given: $..[parameters][?(@.in == "header" && @.name.match(/Cache-Control/i))]
then:
- field: description
  function: truthy
- field: description
  function: pattern
  functionOptions:
    match: .*(max-age|private|no-store|no-cache).*