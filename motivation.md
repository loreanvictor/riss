# Motivation

RISS aims to facilitate development of independent but interoperable tools, services and platforms, that together  constitute a large, distributed, social network.

<br>

## Why a Social Network?

Because social interaction with existing content lowers the barrier of active participation in content creation and circulation. It is fairly easy to like, repost or comment on existing content, encouraging more people to actively share ideas and information on the network.

A counter-argument might be that with lowering the barrier more "spam" is also created. While true, I personally don't see this as a reason to keep the entry barrier high, instead as a key challenge to solve. The purpose of the internet is to further facilitate the flow of ideas and informations, and I believe it will keep constantly evolving in that direction.

<br>

## Why a Distributed Network?

Because centralised networks fragment circulation of ideas and information. This root cause yields a number of more tangible symptoms:

- **Spammy Networks**: Centralised platforms maintain a monopoly on access and discovery of content on their platform, while they mainly drive value through simplifying content creation and not access (e.g. search or discovery). The result is typically accumulation of spam as the platform grows in usage with improvements to access and discovery lagging behind, resulting in the platform getting more _spammy_ over time.

- **Fragmentation**: Audiences, discussions, and general flow of content is fragmented into walled-off gardens. Posts get cross-posted, while the discussions they inspire remain isolated. Creators have to maintain presence on multiple platforms, encouraging their audiences to follow them on multiple platforms to bridge the gap. Users need to hop between different platforms to get the content they desire, etc.
  
- **Speech vs Reach**: Individuals have the right to say whatever they desire (within legal bounds), their audiences have the right to get notified and hear that, and platforms should have to right to not promote any content solely at their own discretion. In a centralised platform, however, these rights are intertwined, and can't be regulated and enforced independently.

<br>

## How is this Different From the Fediverse?

The [Fediverse][fediverse] is a "federated" solution, [not a distributed one][fed-v-dist]. In a distributed network, there is no central authority and anyone can participate with minimum requirements. In a federated network, there are multiple "centers", and participation goes through, and is moderated by, them.

<br>

## Why Not a Federated Network?

A federated network can alleviate some of the downsides of centralisation. However, "federation" implies limiting general participation by design, typically due to some resource or trust constraints, usually both.

For example current federated protocols like [ActivityPub][activity-pub] are "push-first", meaning content is not published unless it is pushed to all of its intended audience, which is costlier (you need to push to multiple other servers, maintain user collections, manage inbox and outbox, etc.) and more trust-requiring (e.g. other servers need to trust you to not count you as spam), compared to a pull-based system (you just make your content available, anyone who desires can pull it).

This design has great potential to gravitate towards a more centralised network. E-mail is a great example (specifically as ActivityPub is modelled after it): personal instances are rare, and most participation happens through a handful providers who also dictate the rules of the network, which seems a natural outcome considering the trust requirements of the network.

<br>

## Why Should Non-Technical People Care?

As mentioned above, generally speaking, fragmentation of flow of ideas and information is an anti-thesis to evolution of internet itself. For example, the following use cases would only be possible with a protocol for distributed social networking:

<br>

> 🧭 **DISCOVERY** \
> I find a new video blogger on a video sharing platform. I _subscribe_ to them right there. I now automatically get their content on the microblogging platform I frequent. I also automatically get notified of their podcasts, livestreams and even posts on their personal website on the same microblogging platform (or wherever else I choose to frequent).

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

## Why Such a Network Needs Multiple Platforms?

For the same reasons we have multiple platforms today, despite a lot of content being cross-posted between them, and a lot of content creators and users actively participating in a multitude of them:

- **Different Content Formats**: The main role of content platforms is to ease creation (and potentially but not necessarily consumption) of various forms of content.
- **Different Discovery Needs**: As is today, some platforms specialise in distributing content using social graphs while others have stronger semantic or topical discovery mechanisms. With interoperable access to more content and alleviation of monopoly of big content platforms, there is potential for even more diversity and innovation on this front.

<br>

[activity-pub]: https://www.w3.org/TR/activitypub/
[fediverse]: https://en.wikipedia.org/wiki/Fediverse
[fed-v-dist]: https://en.wikipedia.org/wiki/Distributed_social_network#Differences_between_distributed_and_federated_networks
