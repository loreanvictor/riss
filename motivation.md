# Motivation

The aim of RISS is facilitate development of interoperable tools, services and platforms that together will constitute a distributed, social network. 

<br>

## Why a Social Network?

Because social interaction with other content is one of the most successful "simplifiers" for content creation. Liking something someone else wrote is pretty easy, and with a press of a button, you've created some (tiny) content of your own. Commenting on someone else's post is far easier than writing one from scratch, and so on.

This essentially democratises content creation on the internet, resulting in more people actively engaged on that front. This is why internet was created to begin with and what it should be all about: better circulation of ideas and information.

A counter-argument for that sentiment might be the fact that lowering the barrier also results in a lot of noise, spam and outright harmful content as well (misinformation, fraud, etc). I personally don't see that as a reason to not further democratise content creation by making it easier and more accessible, but as a reason to focus on the problem of accessing and discovering useful content and separating it from said noise.

<br>

## Why a Distributed Network?

Mainly because centralised networks fragment circulation of ideas, which is again, against "better circulation of ideas and information".

One tangible symptom of this defect is that centralised platforms will get more "spammy" over time. A centralised platform maintains a monopoly on access and discovery of its content (e.g. search and recommendation). The key strength of such a platform is typically in ease of content creation, which also produces more "noise", a problem that is exacerbated by a lagging access and discovery mechanism. The combination often leads to the platform playing catch-up with its own access and discovery needs and grow more "spammy" as its usage grows, in a self-destructive cycle.

Another practical downside is fragmentation of audiences and content. A viral post is typically cross-posted on multiple platforms, with walled-off discussions and interactions on each. Creators need to actively manage presence on multiple platforms and try to convert their audience from one platform to another to bridge these gaps. Users need to hop between apps to follow their desired content, and so on.

A final downside of centralisation is a regulatory one. Anyone should have the right to say whatever they want (as long as it is not illegal), anyone who is interested in that shoudl have the right to hear that. Companies, on the other hand, should maintain the right to not promote any specific content. These twi rights are intertwined in a centralised platform, making it difficult to regulate them separately (speech vs reach).

<br>

## Why Not Federated?

A federated network can alleviate some of the downsides of centralisation. However, "federation" implies still limiting participation, typically due to some resource or trust requirement (typically both). For example current federated protocols like [ActivityPub][activity-pub] are "push-first", meaning a content is not published unless it is pushed to all of its intended audience, which necessarily increases the participation bar both in terms of required resources and in terms of trust.

The trust requirement specifically has great potential to lead to a particularly centrally conttrolled network. For example, while running an email server is not particularly demanding, the trust requirements are still overall dicated by a few mail providers, and independent participation (i.e. personal email servers) are quite rare as a result.

[activity-pub]: https://www.w3.org/TR/activitypub/