# awesome-fauna

Curated list of Fauna resources that live outside of the fauna.com or docs.fauna.com domains. Please feel free to make a PR to add more, or to propose a different organizational structure.

### :bookmark_tabs: Contents

- [Open source Sample apps](#open-source-example-apps)
- [Videos](#videos)
	- [Coding tutorial videos](#coding-tutorial-videos)
	- [Database concept videos](#database-concept-videos)
- [Podcasts](#podcasts)
- [Database concepts](#database-concepts)


## Sample apps

### Wrappers and libraries
#### JavaScript
* [faunadb-fql-lib](https://github.com/shiftx/faunadb-fql-lib) - JS library with utility functions that extends FQL with just FQL
* [faunadb-connector](https://github.com/SilverFox70/faunadb-connector) - Convenience wrapper class for the basic functionality of the Fauna Javascript API
* [faunadb-geo](https://www.npmjs.com/package/faunadb-geo) - JS library for creating, managing, and querying geospatial resources in Fauna

#### Typescript
* [FaunaDB](https://github.com/gmencz/faunadb) - TypeScript-first FaunaDB client with static type inference.

### Database Frameworks
* [Biota](https://github.com/gahabeen/biota) - A simple opiniated database framework for Fauna

### Community Drivers
In addition to Fauna's official, open source drivers in [JavaScript](https://docs.fauna.com/fauna/current/drivers/javascript), [Python](https://docs.fauna.com/fauna/current/drivers/python), [Go](https://docs.fauna.com/fauna/current/drivers/go), [JVM (Java, Scala, Android)](https://docs.fauna.com/fauna/current/drivers/jvm), and [C#](https://docs.fauna.com/fauna/current/drivers/csharp), the following drivers are currently maintained by the community:

* [Dart](https://github.com/gavanitrate/faunadb-http-dart)
* [Elixir #1 - admittedly a bit old](https://github.com/anildigital/faunadb-elixir)
* [Elixir #2 - admittedly a bit older](https://github.com/sprsquish/faunadb-elixir )
* [PHP](https://github.com/m50/faunadb-php)
* [Ruby](https://docs.fauna.com/fauna/current/drivers/ruby)
* [Rust](https://github.com/prisma/faunadb-rust)
* [Swift](https://docs.fauna.com/fauna/current/drivers/swift)

### Data migration

* [DB Migration Tool](https://github.com/fauna-labs/db-migration-tool/) - Fauna-Labs tool to sync data between multiple Fauna databases. Useful for migrating data from one Region Group to another.

### Other tools
* [Gatsby plugin for FaunaDB](https://www.gatsbyjs.org/packages/gatsby-source-faunadb/)
* [Nanohash](https://github.com/gahabeen/nanohash) - A tiny unique string ID generator including a matching 64-bit numeric value
* [Tool that translates Fauna's wire protocol to FQL](https://github.com/trevorsibanda/fauna-tool)
* [gatsby-source-faunadb](https://github.com/paulcuth/gatsby-source-faunadb/blob/master/package.json) - A Gatsby source plugin to fetch documents from Fauna DB
* [Fill Fauna](https://github.com/lkatartn/fill-fauna) - Fill your Fauna collection with data from JSON file


## Gists
Example FQL queries, UDFs, role predicates, etc. Any examples in this section can be removed once they are added to the official docs.fauna.com documentation (which Fauna has plans to open source as well). This section will eventually need to be organized.

* [VS Code snippets](https://gist.github.com/gahabeen/7d2b2b1226c8052c439fd77bf15f9b75) - Add code snippets to Fauna's [VS Code extension](https://docs.fauna.com/fauna/current/start/vs_code) (and please contribute to this gist!)
* [useFauna()](https://gist.github.com/BrunoQuaresma/0236aff64dc44795f19994cbc7a07db6) - React hook used to run Fauna queries
* [Template for building deeply nested FQL queries](https://gist.github.com/ptpaterson/82c01afc9b0ff624f96141a078b5ab54)
* [Docker container testing trait for Scala](https://gist.github.com/tovbinm/5996221ab7a5ecd3d2afbfcd69d6f8e3)
* [Auth0 Rule to generate Fauna user token on login](https://github.com/osa9/nextjs-fauna-auth0-spa/blob/master/resources/auth0/login-fauna-on-login-auth0.js)
* [Managing roles memberships in Fauna](https://gist.github.com/gahabeen/089bea4720f7bb8ec8fc47e0eb094ad7)
* [Fauna User Token Expiration (for ABAC)](https://gist.github.com/colllin/fd7a40bb4f0f16603e68db0e6621369f) - Auth0 + Fauna ABAC integration: How to expire Fauna user secrets
* [nGram example](https://gist.github.com/eigilsagafos/c4ab8c2dd8e8a47d017d7e543fa5887e) - Please note that there is currently no official Fauna documentation on this "secret" function because they want to make some improvements to it first. That said, use this function in production code at your own risk.
* [Clean up Docker](https://gist.github.com/beeman/aca41f3ebd2bf5efbd9d7fef09eac54d) - Not Fauna-specific, but might be useful to anyone working with the Fauna Docker image
* [Recursion UDF example](https://gist.github.com/n400/6b565a5d0ce99d1bffc1d0c2c3926cfd)
* [Expose response headers from JS driver to get query metrics](https://gist.github.com/n400/76530c146e45e19f4bd95efefd04aae4)
* [Recursive function to get nested documents](https://gist.github.com/PierBover/70652ded623c6a76db1a0a6fb938a09f)
* [Fauna Query Builder with test](https://gist.github.com/TracyNgot/291738b403cfa012fe7bf05614c22408)
* [Fauna adapter for next-auth](https://gist.github.com/s-kris/fbb9e5d7ba5e9bb3a5f7bd11f3c42b96)
* [Fauna authentication example with Python](https://gist.github.com/LordGhostX/9d70357f9803904506939ab6f4bb3a9a)


## Open source example apps
All of the apps included here should be open source, with repositories you can fork/clone and run locally.

### React

#### Starter projects
* [Fwitter](https://github.com/fauna-brecht/fwitter) - Fauna's "official unofficial" flagship sample application on which you can build your own project. It comes with with built-in authentication, rate limiting (to deter bots), UDFs, tests, and lots of well-commented example queries. This is a work in progress that will eventually incorporate more features. Feel free to fork and modify it, then link to it from this Awesome-Fauna list.
* [netlify-faunadb-example](https://github.com/netlify/netlify-faunadb-example) - Before Fwitter was created, this was Fauna's most popular sample application. A lot of the other example apps, even those in other JS frameworks, are based on this. React frontend, Netlify Functions for API calls, and Fauna.
* [fauna-nf](https://www.npmjs.com/package/fauna-nf) - npm install a fork of Create React App, with a Fauna backend

#### Authentication examples
* [with-cookie-auth-fauna](https://github.com/zeit/next.js/tree/master/examples/with-cookie-auth-fauna) - Cookie authentication using Fauna with Zeit Now
* [nextjs-auth0-fauna](https://github.com/j0lv3r4/nextjs-auth0-fauna) - Serverless authentication example with Next.js, Auth0, Fauna, and ZEIT Now with Python Serverless Functions
* [magic-link-fauna](https://docs.magic.link/integrations/todomvc) - A fullstack get started tutorial using Fauna + Magic + NextJS + Vercel built for the Next.JS conference.   
(_auth_)! **More specifically [With Magic Link](https://github.com/Vadorequest/rwa-faunadb-reaflow-nextjs-magic/pull/15) example, and [With FaunaDB Auth](https://github.com/Vadorequest/rwa-faunadb-reaflow-nextjs-magic/pull/12) example.**
* [fauna-auth-demo](https://github.com/LordGhostX/fauna-auth-demo) - A fullstack application to get started with Fauna authentication using Fauna + Bootstrap + Python + Flask.


#### Incorporating Very Good Security [VGS]
* [A version of netlify-faunadb-example incorporating VGS](https://github.com/preconceptioncode/netlify-faunadb-example) - For interacting with regulated, sensitive data without the liability of securing it [e.g., for compliance with HIPAA, GDPR, etc.]

#### Streaming examples
* [Fauna's official sample app for document streaming (React)](https://github.com/fauna-brecht/fauna-streaming-example)
(_auth_)! **More specifically [With FaunaDB Real Time](https://github.com/Vadorequest/rwa-faunadb-reaflow-nextjs-magic/pull/13) example.**
* [Synchronized Claps with React on Netlify + Fauna + Pusher](https://github.com/chron/clap)
* [Outpost 18](https://github.com/chron/outpost18) - Real-time card game for two players

#### Code sandboxes

#### Other example apps using React
* [FaunaDo](https://github.com/r-kataria/FaunaDo) - A real-time sync to-do list app built with Next.js, Tailwind CSS, and FaunaDB (updated to use FQL10).
* [Just notes](https://github.com/BrunoQuaresma/justnotes.io) - Note-taking app by one of Fauna's frontend engineer's, using Create React App, Redux Starter Kit, React Redux, and Typescript ([related blog](https://www.brunoquaresma.dev/new-project-justnotes-io/))
* [fauna-market](https://github.com/fauna/fauna-market) - A market for Emoji goods, to demonstrate global consistency in Fauna
* [flash-fauna](https://github.com/NickFoden/flash-fauna) - Flash cards app using Fauna and some hooks
* [serverless-graphql-potter](https://github.com/molebox/serverless-graphql-potter) - A playground project for practicing serverless graphql end points. Built with Gatsby, Netlify functions, Apollo, and Fauna. Data provided via the Potter API.
* [Games built with Next.js and Fauna](https://github.com/goldenshun/botwise) - A set of simple games built with Fauna and Next.js which can be seen in action on https://botwise.games/.

### Vue
* [Got Lobstah](https://github.com/shortdiv/got-lobstah) - A Vue version of netlify-faunadb-example, from the team at Netlify
* [Vue-netlify-fauna-starter-kit](https://github.com/chiubaca/vue-netlify-fauna-starter-kit) - A serverless stack for building CRUD applications with authentication baked in
* [notes-app-azure-serverless](https://github.com/bhaidar/notes-app-azure-serverless) - A sample Vue.js app to manage Notes written in Markdown using Azure Functions and Fauna
* [vue-apollo-fauna-tutorial](https://github.com/tylermercer/vue-apollo-fauna-tutorial) - A tutorial on using Vue, Fauna, and Apollo to create a simple notes app in TypeScript
* [vuejs-faunadb-boilerplate](https://github.com/parag1997/vuejs-faunadb-boilerplate) - A skeleton application to get started with VueJS, Fauna, TailwindCSS and Vuesax and Vee Validate.
* [gridsome-fauna-auth-boilerplate](https://github.com/parag1997/gridsome-fauna-auth-boilerplate) - A nicely designed skeleton app with authentication to get started with VueJS, Fauna and Gridsome
* [Gridsome-FaunaDB-Todo](https://github.com/Vinayak-k160/Gridsome-FaunaDB-Todo) - A Todo application built with VueJS, Gridsome and Fauna
* [vue-netlify-fauna-starter-kit](https://github.com/chiubaca/vue-netlify-fauna-starter-kit) - A serverless stack that uses Vue for the front-end, Netlify for APIs (via Netlify Functions) and Fauna for persistent data storage.


### Svelte
* [covid-19-vs-markets](https://github.com/Prubby/covid-19-vs-markets) - Educational web application which tracks the effects of COVID-19 on indexes such as stocks and currencies
* [cv-svelte-netlify-faunadb](https://github.com/ganesankar/cv-svelte-netlify-faunadb) - A responsive CV/Resume SPA built with Svelte, bulma, and Netlify Functions
* [Vidu](https://github.com/pa-nic/vidu) - Example minimal web analytics SPA build with Netlify (Identity, Functions), Svelte, Windi CSS(TailwindCSS) and Fauna

### Other or no framework
* [https://github.com/zeusdeux/jwt-example](https://github.com/zeusdeux/jwt-example) - Playing with user registration, login/logout, auth, etc using JWTs, serverless functions & fauna as the data store.
* [BigCommerce channels starter app](https://github.com/bigcommerce/channels-app) - A reference implementation by BigCommerce for Channel, Sites, and Routes APIs and BigDesign React Components based on Fauna.
* [JavaScript/TypeScript backend](https://github.com/fauna/js-sample-app) - This sample app shows how to use Fauna in a production application.
The app uses Node.js and the Fauna v10 JavaScript driver to create HTTP API endpoints for an e-commerce store. You can use the app's API endpoints to manage products, customers, and orders for the store.
* [Java](https://github.com/fauna/java-sample-app) - This sample app shows how to use Fauna in a production application.
The app uses Java 17 with Gradle 8.9 and the Fauna v10 JVM driver to create HTTP API endpoints for an e-commerce store. You can use the app's API endpoints to manage products, customers, and orders for the store.
* [Event Streaming](https://github.com/fauna-labs/chat-app-streaming) - This reference application show how you can use Fauna Event Streaming to build real-time apps. You can use it as a starting point for your apps.

## Videos

### Coding tutorial videos
* [Build a Real-time Next.js 14 Chat App with Fauna](https://egghead.io/courses/build-a-real-time-next-js-14-chat-app-with-fauna-f8679b5b) - You’ll learn how to build a chat application using Fauna Streams and Next.js 14, focusing on the essentials and best practices.
* [Fauna JumpStart - Essentials of Fauna](https://www.youtube.com/watch?v=QpuCo9iWK_c&list=PLmNbC0InqwK111JMUS_kAtNz-ymxKAXWN&ab_channel=FaunaInc.) - You'll learn the basics of Fauna
and FQL in this youtube series

### Database concept videos
* [Webinar: Comparing Distributed Transaction Architectures for the Cloud Era (Kyle Kingsbury)](https://www.youtube.com/watch?v=w_zYYF3-iSo&t=2628s) - Geographically distributed transactional workloads are an emerging problem in distributed databases. Consensus algorithms like Raft offer us totally ordered operations in the context of a single replication group, but there is (as of yet) no consensus on how to build fast, isolated transactions across multiple consensus groups. Kyle Kingsbury, author of the famous Jepsen testing series, presents several approaches for transactional databases, including those based on Percolator (TiDB), Spanner (CockroachDB), MongoDB, Yugabyte and Calvin (Fauna).


## Podcasts
* [Unpacking Fauna: A Global Scale Cloud Native Database](https://www.youtube.com/watch?v=idex_BnG_c0) - Data Engineering Podcast Episode 78 (Tobias Macey, 6/4/2019)

## Database concepts
* [Consistent backends and UX - Part 1: Why should you care?](https://css-tricks.com/consistent-backends-and-ux:-why-should-you-care/) -  CSS Tricks, 03/26/2020
* [Consistent backends and UX - Part 2: What can go wrong?](https://css-tricks.com/consistent-backends-and-ux-what-can-go-wrong/) -  CSS Tricks, 03/26/2020
* [Consistent backends and UX - Part 3: What are the barriers to adoption?](https://css-tricks.com/consistent-backends-and-ux-what-are-the-barriers-to-adoption/) -  CSS Tricks, 03/26/2020
* [Consistent backends and UX - Part 4: How do new algorithms help?](https://css-tricks.com/consistent-backends-and-ux:-how-do-new-algorithms-help/) -  CSS Tricks, 03/27/2020
* [What’s next for serverless architecture?](https://www.infoworld.com/article/3526480/whats-next-for-serverless-architecture.html) - Automatic distribution of logic and data to the edge will bring minimal latency to end users, without provisioning, scaling, or configuration worries for developers (InfoWorld, 2/13/2020)


# Contributing

All contributions are greatly appreciated!

If you have a suggestion that would make this better, please fork the repo and create a pull request. You may also simply open an issue.

Don't forget to give the project a star! Thanks again!