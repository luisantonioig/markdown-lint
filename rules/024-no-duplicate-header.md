---
title: MD024 - Multiple headers with the same content
tags:  [headers]
alias: no-duplicate-header
---

This rule is triggered if there are multiple headers in the document that have
the same text:

    # Some text

    ## Some text

To fix this, ensure that the content of each header is different:

    # Some text

    ## Some more text

Rationale: Some markdown parses generate anchors for headers based on the
header name, and having headers with the same content can cause problems with
this.

