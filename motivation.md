# Motivation

RISS aims to facilitate development of independent but interoperable tools, services and platforms that together will constitute a distributed, social network.

<br>

## Why a Social Network?

Because social interaction with existing content is one of the most successful "simplifiers" for content creation. Liking something someone else wrote is pretty easy, and with a press of a button, you've created some (tiny) content of your own. Commenting on someone else's post is far easier than writing one from scratch, and so on.

This essentially democratises content creation on the internet, resulting in more people actively engaged in sharing and circulating ideas and information.

A counter-argument for that sentiment might be the fact that lowering the barrier also results in a lot of noise, spam and outright harmful content as well (misinformation, fraud, etc). I personally don't see that as a reason to not further democratise content creation by making it easier and more accessible, but as a reason to focus on the problem of accessing and discovering useful content and separating it from said noise.

<br>

## Why a Distributed Network?

Mainly because centralised networks fragment circulation of ideas and information.

One tangible symptom of this defect is that centralised platforms will get more "spammy" over time. A centralised platform maintains a monopoly on access and discovery of its content (e.g. search and recommendation). The key strength of such a platform is typically ease of content creation, which also produces more "noise", a problem that is exacerbated by a lagging access and discovery mechanism. The combination often leads to the platform playing catch-up with its own access and discovery needs and grow more "spammy" as its usage grows, in a self-destructive cycle.

Another practical downside is fragmentation of audiences and discussions. A viral post is typically cross-posted on multiple platforms, with walled-off discussions and interactions on each. Creators need to actively manage presence on multiple platforms and try to convert their audience from one platform to another to bridge these gaps. Users need to hop between apps to follow their desired content, and so on.

A final downside of centralisation is a regulatory one. Anyone should have the right to say whatever they want (as long as it is not illegal), anyone who is interested in that should have the right to hear that. Companies, on the other hand, should maintain the right to not promote content at their own discretion. These rights are intertwined in a centralised platform, making it difficult to regulate separately (speech vs reach).

<br>

## How is this Different From the Fediverse?

The [Fediverse][fediverse] is a "federated" solution, [not a distributed one][fed-v-dist]. In a distributed network, there is no central authority and people can participate with minimum requirements (in case of RISS, to be able to make static content available to others on the web). In a federated network, there are multiple "centers", and participation goes through them.

<br>

## Why Not a Federated Network?

A federated network can alleviate some of the downsides of centralisation. However, "federation" implies still limiting participation, typically due to some resource or trust requirement (typically both). For example current federated protocols like [ActivityPub][activity-pub] are "push-first", meaning a content is not published unless it is pushed to all of its intended audience, which necessarily increases the participation bar both in terms of required resources and in terms of trust.

The trust requirement specifically has great potential to lead to a particularly centrally conttrolled network. For example, while running an email server is not particularly demanding, the trust requirements are still overall dicated by a few mail providers, and independent participation (i.e. personal email servers) are quite rare as a result.

<br>

## Why Should Non-Technical People Care?

As mentioned above, in general fragmentation of flow of ideas and information is an essential problem affecting anyone. To be more specific, the following use cases would not be possible without a protocol for distributed social networking:

<br>

> 🧭 **DISCOVERY** \
> I find a new video blogger on a video sharing platform. I _subscribe_ to them right there. I now automatically get their content on the microblogging platform I frequent. I also automatically get notified of their podcasts, livestreams and even posts on their personal website on the same microblogging platform.

<br>

> 💬 **INTERACTION** \
> I am listening to a song on a music streaming platform. I _share_ the song in the platform. My friends and followers on another microblogging platform, or on a short-video platform, get notified of that, and react to that. I can see their reactions on the music streaming platform. I later can see the discussion on other platforms and engage as well.

<br>

> ✏️ **CONTENT CREATION** \
> I see a video essay on a video platform. I write a response on my personal blog, and the discussion continues with users from an online forum and a microblogging platform, as well as the video platform itself, all able to see the whole discussion and participate via their own platform of choice.

<br>

> ✨ **RECOMMENDATION** \
> I can easily switch between different discovery and recommendation mechanisms, without limiting the social content I am looking through. I could do this before for more generic content: for example I could discover content about tech via a newsletter, via a news website, via a forum, a social network, a video platform, a podcast, etc. Now I get the same for ideas and content discussed in discussions and interactions as well.

<br>

> 🧩 **PORTABILITY** \
> I want to no longer be active on this photo-sharing platform I used to frequent, and instead be more active on a microblogging platform. I create an account on the microblogging platform and link the two accounts, my followers and friends not even noticing the change (except that I don't post photos as much).

<br>

[activity-pub]: https://www.w3.org/TR/activitypub/
[fediverse]: https://en.wikipedia.org/wiki/Fediverse
[fed-v-dist]: https://en.wikipedia.org/wiki/Distributed_social_network#Differences_between_distributed_and_federated_networks
