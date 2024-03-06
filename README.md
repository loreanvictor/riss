<br><br>

<img src="logo-dark.svg#gh-dark-mode-only" height="36px"/>
<img src="logo-light.svg#gh-light-mode-only" height="36px"/>

<br>

RISS (Really Intuitive Social Syndication) is a collection of independently proposed extensions for [RSS][rss] to improve distribution of content with social context (e.g. likes, comments, shares, etc.). The idea is that anyone should be able to create, consume and interact with content on the internet without being confined to centralised, walled-off platforms.

<br>

## Why?

- Social content reduces entry barrier, encouraging more people to actively share their ideas, thoughts, content in general.
- Centralised platforms fragment the web though, hindering circulation of content, ideas, and information.
- On centralised platforms, "what gets published" and "what gets recommended" are intertwined, making it difficult to regulate them separately (speech vs reach).
- A federated approach is also potentially not the solution, as it probably ends up where email ended up: pretty centrally controlled.
- In both a centralised and a federated solution, people don't own their content and social activities.

<br>

> Read more about the topic [here][og-gist], and read some interesting takes on it [here][hn-post].

<br>

## Extensions

RISS is made up of the following extensions to RSS, enabling a distributed social network:

- **[Social Context][social-context]**: Adds social context to RSS items, so they can specify if they are an interaction with some other content / feed.
- **[Aggregated Feeds][aggregate-feeds]**: Proposes a complentary standard for a feed representing some aggregation of items in multiple other feeds.
- **[Social Hubs][social-hubs]**: Proposes a standard method for easily _notifying_ the owner of some content of interactions with the content, optionally supporting a method for retrieving an aggregation of interactions as well (using **Aggregated Feeds**).
- **[Feed Linking][feed-linking]**: Proposes a standard method for linking feeds to each other, allowing a user to have multiple feeds (potentially on different platforms) while consumers can verify that the feeds belong to the same user.

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

[social-context]: ./proposals/social-context.md
[aggregate-feeds]: ./proposals/aggregate-feeds.md
[social-hubs]: ./proposals/social-hubs.md
[feed-linking]: ./proposals/feed-linking.md