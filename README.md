# Public GraphQL APIs

*A collective list of public [GraphQL](http://graphql.org/) APIs. PRs are welcome :smile:*
If you are interested in GraphQL in general, check out [awesome-graphql](https://github.com/chentsulin/awesome-graphql).

## Official APIs

| API | Description | Graph*i*QL | Docs/Repo 
| --- | ----------- | :--------: | :-: |
| Brandfolder | Digital asset management platform | [Try it!](https://graphql.brandfolder.com/) | [Repo](https://github.com/brandfolder/graphqlify)
| Buildkite | Continuous integration and deployments | [Try it!](https://graphql.buildkite.com/) | [Docs](https://building.buildkite.com/tutorial-getting-started-with-graphql-queries-and-mutations-11211dfe5d64#.7uhjusw1q)
| EHRI | Holocaust-related archival materials | [Try it!](https://portal.ehri-project.eu/api/graphql/ui) | [Docs](https://portal.ehri-project.eu/api/graphql)
| GraphQL Fake | Fake is a tool for generating fake data using GraphQL queries. | [Try it!](http://fake.graphql.guru) |
| Gdom | DOM Traversing and Scraping using GraphQL | [Try it!](http://gdom.graphene-python.org/graphql?query=%7B%0A++page%28url%3A%22http%3A%2F%2Fnews.ycombinator.com%22%29+%7B%0A++++items%3A+query%28selector%3A%22tr.athing%22%29+%7B%0A++++++rank%3A+text%28selector%3A%22td+span.rank%22%29%0A++++++title%3A+text%28selector%3A%22td.title+a%22%29%0A++++++sitebit%3A+text%28selector%3A%22span.comhead+a%22%29%0A++++++url%3A+attr%28selector%3A%22td.title+a%22%2C+name%3A%22href%22%29%0A++++++attrs%3A+next+%7B%0A+++++++++score%3A+text%28selector%3A%22span.score%22%29%0A+++++++++user%3A+text%28selector%3A%22a%3Aeq%280%29%22%29%0A+++++++++comments%3A+text%28selector%3A%22a%3Aeq%282%29%22%29%0A++++++%7D%0A++++%7D%0A++%7D%0A%7D) | [Repo](https://github.com/syrusakbary/gdom)
| GitHub | Web-based Git repository hosting service | [Try it!](https://developer.github.com/early-access/graphql/explorer/) | [Docs](https://developer.github.com/early-access/graphql/)
| GraphQL World | The fastest growing community of GraphQL developers | [Try it!](https://us-west-2.api.scaphold.io/graphql/graphql-world) | [Docs](https://graphql-docs.com/docs/?graphqlUrl=https://us-west-2.api.scaphold.io/graphql/graphql-world)<br>[Site](https://graphql-world.com/)
| HIVDB | A curated database to represent, store and analyze HIV drug resistance data | [Try it!](https://hivdb.stanford.edu/page/graphiql/) | [Docs](https://hivdb.stanford.edu/page/webservice/)
| Digitransit HSL | Transit routes and realtime schedules from Helsinki Regional Transport Authority, Finland | [Try it!](http://dev.hsl.fi/graphql/console/) | [Docs](https://digitransit.fi/en/developers/services-and-apis/1-routing-api/)
| melodyRepo | Fast and reliable dependency manager for Go | [Try it!](https://melody.sh/play/) | [Docs](https://melody.sh/docs/api)
| Shopify Storefront | The Storefront API gives you full creative control to build customized purchasing experiences for your customers. | [Try it!](https://help.shopify.com/api/storefront-api/graphql-explorer) | [Docs](https://help.shopify.com/api/storefront-api)<br>[Examples](https://github.com/Shopify/storefront-api-examples)
| SuperChargers | Locations of Tesla Stores, Superchargers, Destination Chargers and Service centers | [Try it!](https://www.superchargers.io/graphiql) | [Docs](https://www.superchargers.io/faq)<br>[Repo](https://github.com/wattapp/superchargers)

## Unofficial API proxies

| API | Description | Graph*i*QL | Docs/Repo 
| --- | ----------- | :--------: | :-: |
| Hacker News<br>Reddit<br>Twitter<br>Giphy | GraphQL Hub | [Try HN!](https://www.graphqlhub.com/playground/hn2)<br>[Try Reddit!](https://www.graphqlhub.com/playground/reddit)<br>[Try Twitter!](https://www.graphqlhub.com/playground/twitter)<br>[Try Giphy!](https://www.graphqlhub.com/playground/giphy) | [Docs](https://www.graphqlhub.com/)<br>[Repo](https://github.com/clayallsopp/graphqlhub)
| MusicBrainz |  Open music encyclopedia that collects music metadata | [Try it!](https://graphbrainz.herokuapp.com/?query=query%20NirvanaAlbumSingles%20%7B%0A%20%20lookup%20%7B%0A%20%20%20%20artist(mbid%3A%20%225b11f4ce-a62d-471e-81fc-a69a8278c7da%22)%20%7B%0A%20%20%20%20%20%20name%0A%20%20%20%20%20%20releaseGroups(type%3A%20ALBUM)%20%7B%0A%20%20%20%20%20%20%20%20edges%20%7B%0A%20%20%20%20%20%20%20%20%20%20node%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20title%0A%20%20%20%20%20%20%20%20%20%20%20%20firstReleaseDate%0A%20%20%20%20%20%20%20%20%20%20%20%20relationships%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20releaseGroups(type%3A%20%22single%20from%22)%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20edges%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20node%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20target%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20...%20on%20ReleaseGroup%20%7B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20title%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20firstReleaseDate%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%7D%0A%7D%0A&operationName=NirvanaAlbumSingles) | [Repo](https://github.com/exogen/graphbrainz)
| NYC Restaurant Grades |  NYC Restaurant Inspection Results data (letter ratings for restaurants) | [Try it!](http://nyc-restaurant-grades.com/) | [Docs](https://github.com/bswinnerton/nyc-restaurant-grades)
| PokeAPI | Pokémon Data API | [Try it!](https://pokeapi-graphiql.herokuapp.com/) | [Repo](https://github.com/patrickshaughnessy/PokeAPI-GraphQL)
| Spotify | Spotify gives you instant access to millions of songs – from old favorites to the latest hits. | [Try it!](http://spotify.thefrench.house/graphql-console/) | [Repo](https://github.com/thefrenchhouse/spotify-graphql)<br>[Examples](https://github.com/thefrenchhouse/spotify-graphql-examples)
| SWAPI | Star Wars API	| [Try it!](http://graphql.org/swapi-graphql/) | [Repo](https://github.com/graphql/swapi-graphql)

## Demonstration-only APIs

| API | Description | Graph*i*QL | Docs/Repo 
| --- | ----------- | :--------: | :-: |
| GraphQL Pokémon | Get information of a Pokémon with GraphQL or [Demo App](https://react-relay-pokemon.now.sh/#/)! | [Try it!](https://graphql-pokemon.now.sh/?query=%7B%0A%20%20pokemon(name%3A%20%22Pikachu%22)%20%7B%0A%20%20%20%20id%0A%20%20%20%20number%0A%20%20%20%20name%0A%20%20%20%20attacks%20%7B%0A%20%20%20%20%20%20special%20%7B%0A%20%20%20%20%20%20%20%20name%0A%20%20%20%20%20%20%20%20type%0A%20%20%20%20%20%20%20%20damage%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%20%20evolutions%20%7B%0A%20%20%20%20%20%20id%0A%20%20%20%20%20%20number%0A%20%20%20%20%20%20name%0A%20%20%20%20%20%20weight%20%7B%0A%20%20%20%20%20%20%20%20minimum%0A%20%20%20%20%20%20%20%20maximum%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20attacks%20%7B%0A%20%20%20%20%20%20%20%20fast%20%7B%0A%20%20%20%20%20%20%20%20%20%20name%0A%20%20%20%20%20%20%20%20%20%20type%0A%20%20%20%20%20%20%20%20%20%20damage%0A%20%20%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%7D%0A%7D) | [Repo](https://github.com/lucasbento/graphql-pokemon)<br>[ClientRepo](https://github.com/lucasbento/react-relay-pokemon)
| MongoDB Northwind demo | [Demo App](https://nodkz.github.io/relay-northwind/) build on top of [graphql-compose](https://github.com/nodkz/graphql-compose) and [mongoose](https://github.com/Automattic/mongoose) | [Try it!](https://graphql-compose.herokuapp.com/northwind/)<br>[Try Relay version!](https://nodkz.github.io/relay-northwind/) | [Docs](https://github.com/nodkz/graphql-compose)<br>[ServerRepo](https://github.com/nodkz/graphql-compose-examples)<br>[ClientRepo](https://github.com/nodkz/relay-northwind-app)
| MongoDB TODO-List | TODO List using GraphQL and MongoDb | [Try it!](https://todo-mongo-graphql-server.herokuapp.com/) | [Docs](https://www.compose.com/articles/using-graphql-with-mongodb/)<br>[Repo](https://github.com/igorlima/todo-mongo-graphql-server)
| Scaphold Slackr | Real-time API to power Scaphold Slackr | [Try it!](https://us-west-2.api.scaphold.io/graphql/slackr-api) | [Docs](https://scaphold.io/blog/2016/11/09/build-realtime-apps-with-subs.html)<br>[Repo](https://github.com/scaphold-io/slackr-graphql-subscriptions-starter-kit)
| Spotify GraphQL Server | This demonstrates how to build a GraphQL server which fetches data from an external API (Spotify) | [Try it!](https://spotify-graphql-server.herokuapp.com/graphql?query=%7B%0A%20%20queryArtists(byName%3A%22Red%20Hot%20Chili%20Peppers%22)%20%7B%0A%20%20%20%20name%0A%20%20%20%20id%0A%20%20%20%20image%0A%20%20%7D%0A%7D%0A) | [Docs](https://blog.codecentric.de/en/2017/01/lets-build-spotify-graphql-server)<br> [Repo](https://github.com/lowsky/spotify-graphql-server)
| Three.js demo | Declare a Three.js program with GraphQL | [Try it!](https://jwerle.github.io/three.graphql/) | [Repo](https://github.com/jwerle/three.graphql)
