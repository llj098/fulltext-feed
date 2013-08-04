# fulltext-feed

fulltext feed service

## How does it work

- add a new feed by `/add/raw-rss-url`, fetch raw rss content
- create in memory cache {:raw-rss-link link :cache-item {:url url1 :fulltext-content content1} }
- add job to fectch all the fulltext contents of links which are in the raw rss
- so new item will be ready to serve in minutes.

- get fulltext feed by `/f/raw-rss-url`
- always return the content in the cache

## Usage

## License

Copyright © 2013 FIXME

Distributed under the Eclipse Public License, the same as Clojure.
