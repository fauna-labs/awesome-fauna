# awesome-faunadb

Curated list of FaunaDB resources

## :bookmark_tabs: Contents

- [Gists](#gists)
- [Open source example apps](#open-source-example-apps)
	- [Code sandboxes](#code-sandboxes)
	- [React](#react)
		- [Starter-projects](#starter-projects)
		- [Authentication examples](#authentication-examples)
		- [Incorporating Very Good Security (VGS)](#incorporating-very-good-security-vgs)
		- [Incorporating web sockets](#incorporating-web-sockets)
		- [Other example apps using React](#other-example-apps-using-react)
	- [Vue](#vue)
	- [Svelte](#svelte)
- [Community Drivers](#community-drivers)
- [Other tools](#other-tools)
- [Video tutorials](#video-tutorials)
- [Blogs](#blogs)
	- [Database concepts](#database-concepts)
	- [Code tutorials](#code-tutorials)


## Gists
* [useFauna()](https://gist.github.com/BrunoQuaresma/0236aff64dc44795f19994cbc7a07db6) - React hook used to run Fauna queries
* [Template for building deeply nested FQL queries](https://gist.github.com/ptpaterson/82c01afc9b0ff624f96141a078b5ab54)
* [Docker container testing trait for Scala](https://gist.github.com/tovbinm/5996221ab7a5ecd3d2afbfcd69d6f8e3)


## Open source example apps
All of the apps included here should be open source, with repositories you can fork/clone and run locally.

### React

#### Starter projects
* [netlify-faunadb-example](https://github.com/netlify/netlify-faunadb-example) - Currently our most popular sample application. A lot of the other example apps, even those in other JS frameworks, are based on this. React frontend, Netlify Functions for API calls, and FaunaDB.
* [fauna-nf](https://www.npmjs.com/package/fauna-nf) - npm install a fork of Create React App, with a Fauna backend

#### Authentication examples
* [netlify-faunadb-graphql-auth](https://github.com/ptpaterson/netlify-faunadb-graphql-auth) - A version of the netlify-faunadb-example, using HTTP-only cookies for authentication with FaunaDB's native GraphQL API
* [with-cookie-auth-fauna](https://github.com/zeit/next.js/tree/master/examples/with-cookie-auth-fauna) - Cookie authentication using FaunaDB with Zeit Now
* [with-faunadb-abac-auth](https://github.com/fillipvt/with-faunadb-abac-auth) - Next.js + FaunaDB Cookie Based Login + ABAC + Apollo GraphQL
* [nextjs-auth0-fauna](https://github.com/j0lv3r4/nextjs-auth0-fauna) - Serverless authentication example with Next.js, Auth0, FaunaDB, and ZEIT Now with Python Serverless Functions

#### Incorporating Very Good Security [VGS]
* [A version of netlify-faunadb-example incorporating VGS](https://github.com/preconceptioncode/netlify-faunadb-example) - For interacting with regulated, sensitive data without the liability of securing it [e.g., for compliance with HIPAA, GDPR, etc.]

#### Incorporating web sockets
* [Synchronized Claps with React on Netlify + FaunaDB + Pusher](https://github.com/chron/clap)
* [Outpost 18](https://github.com/chron/outpost18) - Real-time card game for two players

#### Other example apps using React
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


# Video tutorials
* [Building a Serverless JAMStack Todo app with Netlify, Gatsby, GraphQL, and FaunaDB (witth Chris Biscardi)](https://egghead.io/playlists/building-a-serverless-jamstack-todo-app-with-netlify-gatsby-graphql-and-faunadb-53bb)
* [Create a JAMstack Registration Form (with Jason Lengstorf)](https://www.learnwithjason.dev/create-a-jamstack-registration-form)
* [Browser-based charades with Vue.js, Vonage Video API and FaunaDb (with Michael Jolley)](https://www.twitch.tv/videos/575989962)


# Blogs

### Database concepts

#### CSS Tricks series on database consistency
* [Consistency Part 1: Why should you care?](https://css-tricks.com/consistent-backends-and-ux:-why-should-you-care/) - Consistent Backends and UX: Why Should You Care?
* [Consistency Part 2: What can go wrong?](https://css-tricks.com/consistent-backends-and-ux-what-can-go-wrong/) - Consistent Backends and UX: What Can Go Wrong?
* [Consistency Part 3: What are the barriers to adoption?](https://css-tricks.com/consistent-backends-and-ux-what-are-the-barriers-to-adoption/) - Consistent Backends and UX: What are the Barriers to Adoption?
* [Consistency Part 4: How do new algorithms help?](https://css-tricks.com/consistent-backends-and-ux:-how-do-new-algorithms-help/) - Consistent Backends and UX: How Do New Algorithms Help?

#### Serverless
* [What’s next for serverless architecture?](https://www.infoworld.com/article/3526480/whats-next-for-serverless-architecture.html) - Automatic distribution of logic and data to the edge will bring minimal latency to end users, without provisioning, scaling, or configuration worries for developers

### Code tutorials
* [Instant GraphQL Backend with Fine-grained Security Using FaunaDB](https://css-tricks.com/instant-graphql-backend-using-faunadb/)
* [Build a dynamic JAMstack app with GatsbyJS and FaunaDB](https://css-tricks.com/build-a-dynamic-jamstack-app-with-gatsbyjs-and-faunadb/)
* [Build Your Own Serverless Writing Pad with Gatsby, Netlify, and FaunaDB](https://owlypixel.com/build-serverless-writing-pad/)
* [How To Integrate FaunaDB In NodeJS](http://codigofacilito.com/articulos/faunadb-node)
