# link-flow
A protocol for signalling copyright waivers

PRs very welcome!

## Why
As the EU has pressed ahead with it's disastrous articles 11 and 13, this project is an attempt to keep the open web alive.

## What
The proposal is a protocal I've tentatively named link-flow. I envisage that the protocol will be backed by tools built into websites and applications.

# Proposal

This document proposes the following:

1. A per [url](#needs-explicit-definition) server-side header to indicate the following:

    1. That the host asserts that the content at this address is theirs, or is licenced to them.
    2. That the host waives all rights to any link-fee for sites linking to the content url.
    3. That the host waives its copyright with respect to linking to this content for fair use purposes where:
  
        1. The content is not duplicated in its entirety
        2. A link to the original article is [prominently displayed](#needs-explicit-definition) to any [user](#needs-explicit-definition) to whom the content is presented.
    4. That the link-flow header _will not_ be removed from this url.
    5. That by placing the link-flow header on the url the host acknowledges that these conditions will not be changed or invalidated henceforth.
    
2. The development of a checking system that:
    1. Checks that links added to a dynamic web-page have the link-flow header.
    2. Allows the party using the system to decide what to display to users in the case that the link does not have the link-flow header.
