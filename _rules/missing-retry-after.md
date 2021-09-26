---
missing-retry-after:
    description: |-
        When a client is either:
        * throttled out with a 429 status code;
        * warned about a temporary server issue with a 503 status code;
        the server should explicitly communicate how long to wait
        before issuing further requests using the Retry-After header.

        Retry-After is defined in RFC7231.
    message: "Missing ratelimit header: {{property}} in {{path}}"
    formats:
        - oas3
    severity: warn
    recommended: true
    given: $.[responses][?(@property == "429" || @property == "503"  )][headers]
    then:
        field: Retry-After
        function: truthy 
...
missing-retry-after:
    description: |-
        When a client is either:
        * throttled out with a 429 status code;
        * warned about a temporary server issue with a 503 status code;
        the server should explicitly communicate how long to wait
        before issuing further requests using the Retry-After header.

        Retry-After is defined in RFC7231.
    message: "Missing ratelimit header: {{property}} in {{path}}"
    formats:
        - oas3
    severity: warn
    recommended: true
    given: $.[responses][?(@property == "429" || @property == "503"  )][headers]
    then:
        field: Retry-After
        function: truthy 