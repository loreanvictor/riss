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

- **Social Context**: Adds social context to RSS items, so they can specify if they are an interaction with some other content / feed.
- **Aggregated Feeds**: Proposes a complentary standard for a feed representing some aggregation of items in multiple other feeds.
- **Social Hubs**: Proposes a standard method for easily _notifying_ the owner of some content of interactions with the content, optionally supporting a method for retrieving an aggregation of interactions as well (using **Aggregated Feeds**).
- **Feed Linking**: Proposes a standard method for linking feeds to each other, allowing a user to have multiple feeds (potentially on different platforms) while consumers can verify that the feeds belong to the same user.

<br>

## Benefits

These extensions not only address the issues mentioned above, but also provide a number of other benefits:

- *Portability*: through **Social Context**, a user's social presence is their feed, which they can easily move around. Additionally, either by controlling the URL of their feed, or by additionally leveraging **Feed Linking**, creators can move between platforms without affecting their audience.
- *Multiplatform*: With **Feed Linking**, creators can be active on multiple platforms without fragmenting their audience or having to convert them across platforms.
- *Privacy Control*: With **Social Context**, users can control access to their social activity with the same granularity of controlling access to any other resouce on the web. Combined with **Feed Linking**, they can even break their activity into different feeds with independent access control.
- *Exposure Control*: Through **Social Hubs**, users can explicitly control whether they want to notify authors about their interaction. Authors can similarly opt-out of being notified without affecting anyones ability to interact with their content.
- *Aggregation Choice*: With **Aggregated Feeds**, combined with **Social Context**, all recommendation and aggregation mechanisms can be standardised mappings of user feeds to aggregated feeds, enabling interoperability between different recommendation services and various tools and platforms.


[rss]: https://www.rssboard.org/rss-specification
[rss-page]: https://datatracker.ietf.org/doc/html/rfc5005
[web-sub]: https://www.w3.org/TR/websub/
[fediverse]: https://en.wikipedia.org/wiki/Fediverse
[hn-post]: https://news.ycombinator.com/item?id=39548343
[og-gist]: https://gist.github.com/loreanvictor/bddd8824c744024d338e935bd7e96707