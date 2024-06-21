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
    title: "wg-chairs list discussion: Milestones and dates"
    author:
    - org:
    date: false
    target: "https://mailarchive.ietf.org/arch/msg/wgchairs/GKTCAy5As7czqteM-MlhqIvL2Ig/"

--- abstract

As mandated in RFC 2418, working group charters currently contain milestones.
However, these milestones are often sufficiently out of date that they no
longer provide value. This document makes milestones optional and allows more
discretion on their dates. It updates RFC 2418.

--- middle

# Introduction

As mandated in {{Section 2.2 of !RFC2418}}, a working group charter "enumerates
a set of milestones together with time frames for their completion". That
document also leans heavily on milestones as a process mechanism that dictates
how a working group spends its time and conducts its business. However, more
than 25 years after the publication of that document, the reality is often
different. Milestones are now commonly ignored, and often insufficiently
updated to the point of irrelevance. Since 2020, it has been possible for some
working groups to use dateless milestones (see {{DATELESS}}). Since current
usage has diverged significantly from the requirements mandated by {{RFC2418}},
we update that document to better match how the IETF now operates. Making
milestones optional allows removing them from working groups that would
otherwise perpetually have out-of-date milestones, while retaining them when
the chairs do keep them up-to-date.

## Conventions and Definitions

{::boilerplate bcp14-tagged}

# Prior Text

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

Additionally, the current datatracker tooling that allows dateless milestones
appears to be in violation of the RFC 2418 text quoted above. While this is not
a critical issue in and of itself, it helps motivate updating RFC 2418.

# Update

This documents updates the guidance in RFC 2418 in the following ways.

## Optionality of Milestones

Milestones are now optional, on a per-working-group basis. During chartering,
new working groups can now begin existence without milestones. Once a working
group is chartered, milestones can be enabled or disabled without rechartering.

## Optionality of Dates

In RFC 2418, milestones were associated with dates. In 2020, the IESG ran an
experiment that removed dates from milestones from some working groups. This
practice is now officially supported. When a new working group is chartered,
its milestones can be dated or dateless. After chartering, changing whether
dates are enabled does not require rechartering.

## Granularity of Dates

Milestones can carry dates, and those dates have a granularity. Commonly, the
dates have the granularity of a month. Other granularities are possible, such
as a quarter, a half-year, or an IETF meeting. New granularities can be chosen
by the IESG without updating this document.

## Date Management

For each working group that has enabled dated milestones, the dates can be
configured to be modifiable either by the chairs, or by the area director. This
allows the area director to trust the chairs to update dates without approval
in those cases. The decision of who manages change control for the dates lies
with the responsible area director.

## Ownership

As was the case in RFC 2418, changes to milestones are subject to IESG
approval. In particular, whether a specific working group uses milestones,
whether they have dates, and the granularity of those dates, is a decision made
by the Area Director responsible for that working group. Once made, these
decisions need to be posted to the mailing list of the corresponding working
group.

The Area Director is encouraged to discuss these choices with the working group
chairs, as the success of milestones is predicated on the chairs updating them
in a timely manner. While it is expected that this decision will almost always
be made as agreement between working group chairs and their responsible area
director, in the case of a disagreement the final decision lies with the area
director.

## Guidance for Chairs

For working groups where milestones are enabled, chairs are expected to keep
milestones up to date. Chairs are expected to review milestones at least once
per IETF meeting (every four months) to ensure they are accurate.

# Security Considerations

Readers of the datatracker REALLY SHOULD NOT make important decisions based
solely on the status of working group milestones as those could be out of date.

# IANA Considerations

This document has no IANA actions.

--- back

# Alternatives Considered

During discussions around this document, the following alternatives were
considered.

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
director. The benefits of up-to-date milestones would need to demonstrated in
order to motivate their use.

## Improve Tooling to Automate Milestones

The overwhelming majority of milestones currently on the datatracker are
specific to a given draft. The datatracker even includes tooling that allows
attaching a draft to a milestone as an "associated document". This tooling
could be enhanced to automatically update the milestone based on the status of
the corresponding document. However, this raises the question: if the relevant
information is already available in the datatracker, what is the purpose of
duplicating it in a milestone?

## Remove Milestones Entirely

Another more drastic option would be to remove milestones entirely from the
datatracker, and update RFC 2418 to no longer mention them.

## Rewrite RFC 2418

During the 25 years that have gone by since RFC 2418 was published, many
aspects of the IETF process have changed. At this point, some portions of RFC
2418 now feel anachronistic. As a random example, working group minutes are
theoretically required to be encoded in ASCII, and that almost never happens
any more in order to allow using the names of working group members that
require different character sets. Similarly, RFC 2418 still requires chairs to
circulate an attendance list (also known as the "blue sheets"), a task that has
now been automated.

While such small points do help motivate updating RFC 2418, it is unclear if
much larger changes would be beneficial.

# Acknowledgments
{:numbered="false"}

Some of the contents of this document were inspired by a presentation given by
Adam Roach at the WG Chairs’ Forum at IETF 103 in November 2018. The author
would like to thank everyone who commented on the various email discussions
about this topic.
