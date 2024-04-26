---
title: "An Update on Milestones"
category: bcp
docname: draft-schinazi-update-on-milestones-latest
submissiontype: IETF
number:
date:
consensus: true
v: 3
area: GEN
updates: 2418
workgroup:
keyword:
 - working group
 - charter
 - milestones
venue:
#  group:
#  type:
#  mail:
#  arch:
  github: "DavidSchinazi/draft-schinazi-update-on-milestones"
  latest: "https://davidschinazi.github.io/draft-schinazi-update-on-milestones/draft-schinazi-update-on-milestones.html"

author:
  -
    ins: D. Schinazi
    name: David Schinazi
    org: Google LLC
    street: 1600 Amphitheatre Parkway
    city: Mountain View
    region: CA
    code: 94043
    country: United States of America
    email: dschinazi.ietf@gmail.com

normative:

informative:
  DATELESS:
    title: "GitHub issue: Option to Remove Dates from Milestones"
    author:
    - org:
    date: false
    target: "https://github.com/ietf-tools/datatracker/issues/2799"

--- abstract

As mandated in RFC 2418, working group charters currently contain milestones.
However, these milestones are often sufficiently out of date that they no
longer provide value. This document exists to facilitate a community discussion
around the future of milestones. This document could potentially update RFC
2418.

--- middle

# Introduction

As mandated in {{Section 2.2 of !RFC2418}}, a working group charter "enumerates
a set of milestones together with time frames for their completion". That
document also leans heavily on milestones as a process mechanism that dictates
how a working group spends its time and conducts its business. However, more
than 15 years after the publication of that document, the reality is often
different. Milestones are now commonly ignored, and often insufficiently
updated to the point of irrelevance. Since 2020, it has been possible for some
working groups to use dateless milestones (see {{DATELESS}}). Since current
usage has diverged significantly from the requirements mandated by {{RFC2418}},
it seems valuable that we update that document to the current community
consensus, assuming such consensus exists. This document currently describes
possible options as a way to facilitate this community discussion, and if such
a consensus were to emerge, this document would then update {{RFC2418}}.

## Conventions and Definitions

{::boilerplate bcp14-tagged}

# Current Text

At the time of writing this document, the current normative language around
milestones is in {{Section 2.2 of RFC2418}}:

> The working group charter MUST establish a timetable for specific work items.
While this may be renegotiated over time, the list of milestones and dates
facilitates the Area Director's tracking of working group progress and status,
and it is indispensable to potential participants identifying the critical
moments for input. Milestones shall consist of deliverables that can be
qualified as showing specific achievement; e.g., "Internet-Draft finished" is
fine, but "discuss via email" is not. It is helpful to specify milestones for
every 3-6 months, so that progress can be gauged easily. This milestone list is
expected to be updated periodically (see {{Section 5 of RFC2418}}).

# Issues

Milestones were designed as a tool to share information from the corresponding
working group to various interested parties. When milestones are years out of
date, they can no longer serve that purpose. They can also cause harm if
someone interprets them as being timely when they are in fact out of date.

# Potential Path Forwards

The list of potential paths forward below is meant as a mostly exchaustive list
of options that the author was aware of at the time of writing. If you think of
one that isn't listed, please notify the author so it can be added.

## Do Nothing

As is often the case, the simplest path forward is to do nothing at all. It has
the advantage of requiring the least work, but the obvious downside of not
addressing the issues described in {{issues}}.

## Ensure Chairs Update Milestones

One potential solution to the issue of out of date milestones is,
unsurprisingly, to update the milestones often enough. This solution has the
advantage of not requiring community consensus to update RFC 2418. Since
working chairs serve at the discretion of the Area Director, it is absolutely
within the area directors' mandate to request that chairs update milestones.
However, since chairs are a volunteer unpaid position, they might not always
have the time to fulfill all the tasks requested by their responsible area
director. The IESG would need to demonstrate the benefits of up-to-date
milestones in order to motivate their use.

## Improve Tooling to Automate Milestones

The overwhelming majority of milestones currently on the datatracker are
specific to a given draft. The datatracker even includes tooling that allows
attaching a draft to a milestone as an "associated document". This tooling
could be enhanced to automatically update the milestone based on the status of
the corresponding document. However, this begs the question: if the relevant
information is already available in the datatracker, what is the purpose of
duplicating it in a milestone?

## Formalize Dateless Milestones

The current datatracker tooling that allows dateless milestones appears to be
in violation of the RFC 2418 text quoted above. While this is not a critical
issue in and of itself, it helps motivate updating RFC 2418. We could update
RFC 2418 to reflect the reality of our current process.

## Make Milestones Optional

Another potential update to RFC 2418 would be to make milestones optional.
Since some area directors find milestones helpful and others do not, we could
have the best of both worlds by formally making milestones optional: they would
then be enabled or disabled for each working group on a case-by-case basis. The
responsible area director would decide whether to enable milestones or not,
though they should involve the working group chairs in that decision as
milestones can only be successful is chairs update them.

Making milestones optional allows removing them from working groups that would
otherwise perpetually have out-of-date milestones, while retaining them when
the chairs do keep them up-to-date.

## Remove Milestones Entirely

Another more drastic option would be to remove milestones entirely from the
datatracker, and update RFC 2418 to no longer mention them.

## Rewrite RFC 2418

During the 15 years that have gone by since RFC 2418 was published, many
aspects of the IETF process have changed. At this point, some portions of RFC
2418 now feel anachronistic. As a random example, working group minutes are
theoretically required to be encoded in ASCII, and that almost never happens
any more in order to allow using the names of working group members that
require different character sets. Similarly, RFC 2418 still requires chairs to
circulate an attendance list (also known as the "blue sheets"), a task that has
now been automated.

While such small points do help motivate updating RFC 2418, it is unclear if
much larger changes would be beneficial.

# Conclusion

Based on the above, the author currently believes that the best path forward
would be to update RFC 2418 to both make milestones optional, and codify the
availability of dateless milestones. Making such a change would require IETF
consensus.

# Security Considerations

Readers of the datatracker REALLY SHOULD NOT make important decisions based
solely on the status of working group milestones as those could be out of date.

# IANA Considerations

This document has no IANA actions.

--- back

# Acknowledgments
{:numbered="false"}

Some of the contents of this document were inspired by a presentation given by
Adam Roach at the WG Chairs’ Forum at IETF 103 in November 2018.
