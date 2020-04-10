# awesome-faunadb

Curated list of FaunaDB resources that live outside of the fauna.com or docs.fauna.com domains. Please feel free to make a PR to add more, or to propose a different organizational structure.

## :bookmark_tabs: Contents

- [Gists](#gists)
- [Open source example apps](#open-source-example-apps)
	- [React](#react)
		- [Code sandboxes](#code-sandboxes)
		- [Starter-projects](#starter-projects)
		- [Authentication examples](#authentication-examples)
		- [Incorporating Very Good Security (VGS)](#incorporating-very-good-security-vgs)
		- [Incorporating web sockets](#incorporating-web-sockets)
		- [Other example apps using React](#other-example-apps-using-react)
	- [Vue](#vue)
	- [Svelte](#svelte)
	- [Other or no framework](#other-or-no-framework)
- [Community Drivers](#community-drivers)
- [Other tools](#other-tools)
- [Videos](#videos)
	- [Coding tutorial videos](#coding-tutorial-videos)
	- [Database concept videos](#database-concept-videos)
- [Podcasts](#podcasts)
- [Articles](#articles)
	- [Coding tutorial blogs](#coding-tutorial-blogs)
	- [Database concept blogs](#database-concept-blogs)


## Gists
Example FQL queries, UDFs, role predicates, etc. Any examples in this section can be removed once they are added to the official docs.fauna.com documentation (which Fauna has plans to open source as well). This section will eventually need to be organized.

* [useFauna()](https://gist.github.com/BrunoQuaresma/0236aff64dc44795f19994cbc7a07db6) - React hook used to run Fauna queries
* [Template for building deeply nested FQL queries](https://gist.github.com/ptpaterson/82c01afc9b0ff624f96141a078b5ab54)
* [Docker container testing trait for Scala](https://gist.github.com/tovbinm/5996221ab7a5ecd3d2afbfcd69d6f8e3)
* [Auth0 and GraphQL example](https://gist.github.com/colllin/52d741f830a98c1a652e817aea0d22d0)
* [Managing roles memberships in FaunaDB](https://gist.github.com/gahabeen/089bea4720f7bb8ec8fc47e0eb094ad7)
* [FaunaDB User Token Expiration (for ABAC)](https://gist.github.com/colllin/fd7a40bb4f0f16603e68db0e6621369f) - Auth0 + FaunaDB ABAC integration: How to expire Fauna user secrets
* [fauna-graphql-relations](https://gist.github.com/tovbinm/f76bcbf56ea8e2e3740e237b6c2f2ab9) - FaunaDB Relations: GraphQL schemas, mutations and resulting documents
* [nGram example](https://gist.github.com/eigilsagafos/c4ab8c2dd8e8a47d017d7e543fa5887e) - Please note that there is currently no official Fauna documentation on this "secret" function because they want to make some improvements to it first. That said, use this function in production code at your own risk.
* [Clean up Docker](https://gist.github.com/beeman/aca41f3ebd2bf5efbd9d7fef09eac54d) - Not Fauna-specific, but might be useful to anyone working with the FaunaDB Docker image
* [Recursion UDF example](https://gist.github.com/n400/6b565a5d0ce99d1bffc1d0c2c3926cfd)


## Open source example apps
All of the apps included here should be open source, with repositories you can fork/clone and run locally.


### React

###### Code sandboxes
* [Code Sandbox by Josh Parrot (Apollo GraphQL + Fauna)](https://codesandbox.io/s/festive-haibt-y61bw)

###### Starter projects
* [netlify-faunadb-example](https://github.com/netlify/netlify-faunadb-example) - Currently Fauna's most popular sample application. A lot of the other example apps, even those in other JS frameworks, are based on this. React frontend, Netlify Functions for API calls, and FaunaDB.
* [fauna-nf](https://www.npmjs.com/package/fauna-nf) - npm install a fork of Create React App, with a Fauna backend

###### Authentication examples
* [netlify-faunadb-graphql-auth](https://github.com/ptpaterson/netlify-faunadb-graphql-auth) - A version of the netlify-faunadb-example, using HTTP-only cookies for authentication with FaunaDB's native GraphQL API
* [with-cookie-auth-fauna](https://github.com/zeit/next.js/tree/master/examples/with-cookie-auth-fauna) - Cookie authentication using FaunaDB with Zeit Now
* [with-faunadb-abac-auth](https://github.com/fillipvt/with-faunadb-abac-auth) - Next.js + FaunaDB Cookie Based Login + ABAC + Apollo GraphQL
* [nextjs-auth0-fauna](https://github.com/j0lv3r4/nextjs-auth0-fauna) - Serverless authentication example with Next.js, Auth0, FaunaDB, and ZEIT Now with Python Serverless Functions

###### Incorporating Very Good Security [VGS]
* [A version of netlify-faunadb-example incorporating VGS](https://github.com/preconceptioncode/netlify-faunadb-example) - For interacting with regulated, sensitive data without the liability of securing it [e.g., for compliance with HIPAA, GDPR, etc.]

###### Incorporating web sockets
* [Synchronized Claps with React on Netlify + FaunaDB + Pusher](https://github.com/chron/clap)
* [Outpost 18](https://github.com/chron/outpost18) - Real-time card game for two players

###### Other example apps using React
* [Code Sandbox by Josh Parrot (Apollo GraphQL + Fauna)](https://codesandbox.io/s/festive-haibt-y61bw)
* [Just notes](https://github.com/BrunoQuaresma/justnotes.io) - Note-taking app by one of Fauna's frontend engineer's, using Create React App, Redux Starter Kit, React Redux, and Typescript ([related blog](https://www.brunoquaresma.dev/new-project-justnotes-io/))
* [Talent Hub](https://github.com/spacehelmet/talenth) - Open source HR platform on React, Apollo and GraphQL https://talenth.co ([related blog](https://fauna.com/blog/building-a-job-posting-platform-with-faunadb-and-apollo))
* [fauna-market](https://github.com/fauna/fauna-market) - A market for Emoji goods, to demonstrate global consistency in FaunaDB
* [flash-fauna](https://github.com/NickFoden/flash-fauna) - Flash cards app using FaunaDB and some hooks
* [serverless-graphql-potter](https://github.com/molebox/serverless-graphql-potter) - A playground project for practicing serverless graphql end points. Built with Gatsby, Netlify functions, Apollo, and FaunaDB. Data provided via the Potter API.

### Vue
* [Got Lobstah](https://github.com/shortdiv/got-lobstah) - A Vue version of netlify-faunadb-example, from the team at Netlify
* [Vue-netlify-fauna-starter-kit](https://github.com/chiubaca/vue-netlify-fauna-starter-kit) - A serverless stack for building CRUD applications with authentication baked in
* [notes-app-azure-serverless](https://github.com/bhaidar/notes-app-azure-serverless) - A sample Vue.js app to manage Notes written in Markdown using Azure Functions and FaunaDB
* [vue-apollo-fauna-tutorial](https://github.com/tylermercer/vue-apollo-fauna-tutorial) - A tutorial on using Vue, FaunaDB, and Apollo to create a simple notes app in TypeScript

### Svelte
* [covid-19-vs-markets](https://github.com/Prubby/covid-19-vs-markets) - Educational web application which tracks the effects of COVID-19 on indexes such as stocks and currencies ([live app](https://covid-19-vs-market.now.sh/))
* [cv-svelte-netlify-faunadb](https://github.com/ganesankar/cv-svelte-netlify-faunadb) - A responsive CV/Resume SPA built with Svelte, bulma, and Netlify Functions

### Other or no framework
* [https://github.com/zeusdeux/jwt-example](https://github.com/zeusdeux/jwt-example) - Playing with user registration, login/logout, auth, etc using JWTs, serverless functions & faunadb as the data store. 


## Community drivers
In addition to Fauna's official, open source drivers in [JavaScript](https://docs.fauna.com/fauna/current/drivers/javascript), [Python](https://docs.fauna.com/fauna/current/drivers/python), [Go](https://docs.fauna.com/fauna/current/drivers/go), [JVM (Java, Scala, Android)](https://docs.fauna.com/fauna/current/drivers/jvm), [C#](https://docs.fauna.com/fauna/current/drivers/csharp), [Ruby](https://docs.fauna.com/fauna/current/drivers/ruby), and [Swift](https://docs.fauna.com/fauna/current/drivers/swift), the following drivers are currently maintained by the community:

* [Rust driver](https://github.com/prisma/faunadb-rust)
* [Elixir driver #1 - admittedly a bit old](https://github.com/anildigital/faunadb-elixir)
* [Elixir driver #2 - admittedly a bit older](https://github.com/sprsquish/faunadb-elixir )


## Other tools
* [Gatsby plugin for FaunaDB](https://www.gatsbyjs.org/packages/gatsby-source-faunadb/)
* [FaunaDB Migrate](https://github.com/BrunoQuaresma/faunadb-migrate) - For migrating schema [not data] between Fauna databases 
* [faunadb-fql-lib](https://github.com/shiftx/faunadb-fql-lib) - JS library with utility functions that extends FQL with just FQL
* [Fill Fauna](https://github.com/lkatartn/fill-fauna) - Fill your faunaDB collection with data from JSON file
* [Nanohash](https://github.com/gahabeen/nanohash) - A tiny unique string ID generator including a matching 64-bit numeric value
* [Tool that translates Fauna's wire protocol to FQL](https://github.com/trevorsibanda/fauna-tool)


## Videos

#### Coding tutorial videos

###### JavaScript
* [Building a Serverless JAMStack Todo app with Netlify, Gatsby, GraphQL, and FaunaDB (Chris Biscardi)](https://egghead.io/playlists/building-a-serverless-jamstack-todo-app-with-netlify-gatsby-graphql-and-faunadb-53bb)
* [Create a JAMstack Registration Form (Jason Lengstorf)](https://www.learnwithjason.dev/create-a-jamstack-registration-form)
* [Browser-based charades with Vue.js, Vonage Video API and FaunaDb (Michael Jolley)](https://www.twitch.tv/videos/575989962)
* [Learn with Jason: Deploy a Gatsby Site + API Using ZEIT Now (Leo Lamprecht, Jason Lengstorf)](https://www.youtube.com/watch?v=6pfi4tx8yNA) - [demo](https://zeitplusgatsby.com), [repo](https://github.com/jlengstorf/zeit-prod)
* [Building a data layer for awesum.io with FaunaDb (Michael Jolley, 9/19/2019)](https://www.youtube.com/watch?v=E2YP4v5eT4Q)

###### Golang
* [Exploring Netlify and FaunaDB using Go Functions (Chris Biscardi)](https://www.youtube.com/watch?v=80c3088hXWQ) - We insert our first documents into a FaunaDB database using the Golang driver. 
* [Querying FaunaDB with FQL and GoLang (Chris Biscardi)](https://www.youtube.com/watch?v=4S7BNMIuwgk)

###### Other
* [Oracle & PostgreSQL To FaunaDB FullMode](https://www.youtube.com/watch?v=33a1nSxU32E)

#### Database concept videos
* [Webinar: Comparing Distributed Transaction Architectures for the Cloud Era (Kyle Kingsbury)](https://www.youtube.com/watch?v=w_zYYF3-iSo&t=2628s) - Geographically distributed transactional workloads are an emerging problem in distributed databases. Consensus algorithms like Raft offer us totally ordered operations in the context of a single replication group, but there is (as of yet) no consensus on how to build fast, isolated transactions across multiple consensus groups. Kyle Kingsbury, author of the famous Jepsen testing series, presents several approaches for transactional databases, including those based on Percolator (TiDB), Spanner (CockroachDB), MongoDB, Yugabyte and Calvin (FaunaDB).


## Podcasts
* [Unpacking Fauna: A Global Scale Cloud Native Database](https://www.youtube.com/watch?v=idex_BnG_c0) - Data Engineering Podcast Episode 78 (Tobias Macey, 6/4/2019)


## Articles

#### Coding tutorial blogs
* [Instant GraphQL Backend with Fine-grained Security Using FaunaDB](https://css-tricks.com/instant-graphql-backend-using-faunadb/)
* [Build a dynamic JAMstack app with GatsbyJS and FaunaDB](https://css-tricks.com/build-a-dynamic-jamstack-app-with-gatsbyjs-and-faunadb/)
* [Build Your Own Serverless Writing Pad with Gatsby, Netlify, and FaunaDB](https://owlypixel.com/build-serverless-writing-pad/)
* [How To Integrate FaunaDB In NodeJS](http://codigofacilito.com/articulos/faunadb-node)
* [Serverless GraphQL - Part 3](https://nickymeuleman.netlify.app/blog/serverless-graphql-part-3)
* [JAMstack Dynamic and Async functionality](https://overflowjs.com/posts/JAMstack-Dynamic-and-Async-functionality.html)

#### Database concept blogs

###### Database consistency
* [Consistent backends and UX - Part 1: Why should you care?](https://css-tricks.com/consistent-backends-and-ux:-why-should-you-care/) -  CSS Tricks, 03/26/2020
* [Consistent backends and UX - Part 2: What can go wrong?](https://css-tricks.com/consistent-backends-and-ux-what-can-go-wrong/) -  CSS Tricks, 03/26/2020
* [Consistent backends and UX - Part 3: What are the barriers to adoption?](https://css-tricks.com/consistent-backends-and-ux-what-are-the-barriers-to-adoption/) -  CSS Tricks, 03/26/2020
* [Consistent backends and UX - Part 4: How do new algorithms help?](https://css-tricks.com/consistent-backends-and-ux:-how-do-new-algorithms-help/) -  CSS Tricks, 03/27/2020
###### Serverless
* [What’s next for serverless architecture?](https://www.infoworld.com/article/3526480/whats-next-for-serverless-architecture.html) - Automatic distribution of logic and data to the edge will bring minimal latency to end users, without provisioning, scaling, or configuration worries for developers (InfoWorld, 2/13/2020)
