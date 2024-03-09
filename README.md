<br>

<img src="logo-dark.svg#gh-dark-mode-only" height="36px"/>
<img src="logo-light.svg#gh-light-mode-only" height="36px"/>

<br>

RISS (Really Intuitive Social Syndication) is a collection of independently proposed extensions for [RSS][rss] to improve distribution of content with social context (e.g. likes, comments, shares, etc.). The goal is to facilitate a distributed social network where anyone can easily and independently participate.

<br>

## Why?

- Social platforms reduce entry barrier to content creation, by making it easy to create content via interacting with existing content.
- Centralised platforms fragment the web though, hindering circulation of content, ideas, and information.
- On centralised platforms, "what gets published" and "what gets recommended" are intertwined, making it difficult to regulate them separately (speech vs reach).
- A federated approach is also potentially not the solution, as it probably ends up where email ended up: pretty centrally controlled.
- In both a centralised and a federated solution, people don't own their content and social activities.

<br>

Subsequently, an ideal platform would be a distributed network where benefits of social platforms are retained, but barrier to independent participation is as low as hosting static content (e.g. personal blogging).

<br>

> Read more about the motivation [here][motivation], and more about this topic [here][og-gist], and [here][hn-post].

<br>

## Overview

The main idea behind RISS is ***Interaction as Content***:

- Any interaction is content, and should be treated as such.
- This means interactions can be published and syndicated as any other static web content, i.e. via [RSS feeds][rss].

<br>

> 💡 **EXAMPLE** \
> I see a post that I like. It might be some blog post on a personal blog, some post on Reddit or Hacker News, some YouTube video, etc. I can "like it", as in publishing a post in my own feed that says "I liked this post". I can even comment on it, which will be another post by me, with a link (perhaps in the post, and in my feed) to the original post. I might even follow the original author, which again will be a post in my feed with a link to their corresponding feed.

<br>

The core extension of RISS is the **[Social Context][social-context]** extension, which specifies how a feed entry, which is the result of interaction with some other content, to specify if that in a standardized manner. This provides the following benefits:
- **Distributed Network**: participation in the network merely requires the ability to host a static file at a set URL (the feed).
- **Data Portability**: Each user is represented fully by their feed, which can be easily moved between different platforms and hosting providers. As long as the feed URL remains the same, the audience (e.g. the followers) would also not even notice the change.
- **Granular Privacy**: With this model, access control to social data of a user is reduced to access control of a feed, i.e. a web resource at a set URL. This allows for fine-grained control over who can see what.
- **Content Ownership**: A user is in full control of their feed and as a result their content and activities. Service providers might enforce policies as to which content they help circulate, but they cannot control the content itself, the audience that is subscribed to it, or the interactions with it.

<br>

RSS, and by extension RISS, are inherently pull-based models, affecting speed and ease of content distribution, a problem that can get exacerbated with social content. For example, _who has interacted with my content?_ becomes a hard question as theoretically one would need to pull all existing feeds and filter them for social context to find out.

This problem can however be solved by independent extensions such as **[WebSub][web-sub]** and **[Social Hubs][social-hubs]**:

- Authors can use WebSub to notify their audience of updates to their feed,
- Users can notify original authors of interactions with their content using Social Hubs.

<br>

Users might also have multiple feeds, for example as they are active on multiple platforms, or to further control access to their activity (e.g. keeping posts and likes public while keeping their comments more private). **[Feed Linking][feed-linking]** can be independently adopted to link these feeds in a verifiable and standardised manner:

- Authors can be active on multiple platforms with their feeds linked, without fragmenting their audience,
- Authors can move to different platforms even when they don't control access to their feed URL, by simply linking their new feed.
- Authors can break their activity into multiple different feeds with different access control while maintaining their identity.

<br>

Aggregating content from multiple feeds will be a recurring need in such a network. **[Aggregate Feeds][aggregate-feeds]** independently proposes a standardisation for that:

- This enables **Social Hubs** to also provide aggregation of interactions in a standardised manner,
- Combined with **Social Context**, this standardises recommendation algorithms into blackboxes that generate aggregate feeds from a set of input user feeds (since they include all the user's interaction history).

<br>

## Design Goals

- *RISS is social*: it aims to facilitate development and interoperability of tools that lower barrier to entry for content creation via social means, i.e. interaction with other content.
- *RISS is distributed*: it aims to create an interoperable network wherein participation requires only the ability to host a static file at a set URL. All additional features should be optional, and have minimum requirements in terms of computational resources and trust.
- *RISS is about content syndication*: interactions are content, users are feeds of content. If a problem can't be modelled as such, it is possible that it is out of RISS's scope.

<br>

## Document Status

RISS is a work in progress. Any and all feedback on the proposals and the project goals are more than appreciated. This includes, but is not limited to:

- Feedback on how a proposal would affect complying tools and services,
- Feedback on how a proposal can be improved,
- Feedback on existing standards that might better complement proposed extensions,
- Feedback on why some proposal isn't needed, or should be out of scope,
- Feedback on new proposals that should be part of RISS, as they are essential in achieving the design goals.

<br>

## Proposed Extensions

RISS is made up of the following extensions to RSS, enabling a distributed social network:

- **[Social Context][social-context]**: Adds social context to RSS items, so they can specify if they are an interaction with some other content / feed.
- **[Aggregated Feeds][aggregate-feeds]**: Proposes a complentary standard for a feed representing some aggregation of items in multiple other feeds.
- **[Social Hubs][social-hubs]**: Proposes a standard method for easily _notifying_ the owner of some content of interactions with the content, optionally supporting a method for retrieving an aggregation of interactions as well (*using **Aggregated Feeds***).
- **[Feed Linking][feed-linking]**: Proposes a standard method for linking feeds to each other, allowing a user to have multiple feeds (potentially on different platforms) while consumers can verify that the feeds belong to the same user. *Is dependent on **Social Context***.
- **[Content Verification][content-verification]**: Proposes a standard method for verifying some content, by someone beyond the owner of the feed. Useful, for example, for one-directional **Feed Linking**, allowing data portability to be not dependent on platforms.

<br>

## Complementary Standards

The following existing standards also complement tools built on RISS, so it is adivsable to consider them:

- **[Feed Pagination][rss-page]**: RISS results in large feeds, so it is advisable to use feed pagination to avoid large feeds.
- **[WebSub][web-sub]**: RISS feeds can be used as WebSub topics, allowing for real-time updates of social activity. This can be combined with **[Social Hubs][social-hubs]** to enable real-time distribution of social interactions while keeping participation cost low.

<br>

[rss]: https://www.rssboard.org/rss-specification
[rss-page]: https://datatracker.ietf.org/doc/html/rfc5005
[web-sub]: https://www.w3.org/TR/websub/
[fediverse]: https://en.wikipedia.org/wiki/Fediverse
[hn-post]: https://news.ycombinator.com/item?id=39548343
[og-gist]: https://gist.github.com/loreanvictor/bddd8824c744024d338e935bd7e96707

[motivation]: ./motivation.md

[social-context]: ./proposals/social-context.md
[aggregate-feeds]: ./proposals/aggregate-feeds.md
[social-hubs]: ./proposals/social-hubs.md
[feed-linking]: ./proposals/feed-linking.md
[content-verification]: ./proposals/content-verification.md
