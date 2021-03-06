---
title: MD022 - Headers should be surrounded by blank lines
tags:  [headers, blank_lines]
alias: blanks-around-headers
---

This rule is triggered when headers (any style) are either not preceded or not
followed by a blank line:

    # Header 1
    Some text

    Some more text
    ## Header 2

To fix this, ensure that all headers have a blank line both before and after
(except where the header is at the beginning or end of the document):

    # Header 1

    Some text

    Some more text

    ## Header 2

Rationale: Aside from aesthetic reasons, some parsers, including kramdown, will
not parse headers that don't have a blank line before, and will parse them as
regular text.


