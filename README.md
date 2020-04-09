
In addition to Fauna's official [and open source] drivers in (https://docs.fauna.com/fauna/current/drivers/javascript)[JavaScript], (https://docs.fauna.com/fauna/current/drivers/python)[Python], (https://docs.fauna.com/fauna/current/drivers/go)[Go], (https://docs.fauna.com/fauna/current/drivers/jvm)[JVM [Java, Scala, Android], (https://docs.fauna.com/fauna/current/drivers/csharp)[C#], (https://docs.fauna.com/fauna/current/drivers/ruby)[Ruby], and (https://docs.fauna.com/fauna/current/drivers/swift)[Swift], the following drivers are currently maintained by the community:

* (https://github.com/prisma/faunadb-rust)[Rust driver]
* (https://github.com/anildigital/faunadb-elixir)[Elixir driver #1]
* (https://github.com/sprsquish/faunadb-elixir )[Elixir driver #2] 

# Other tools

* (https://www.gatsbyjs.org/packages/gatsby-source-faunadb/)[Gatsby plugin for FaunaDB]
* (https://github.com/BrunoQuaresma/faunadb-migrate)[FaunaDB Migrate] - For migrating schema [not data] between Fauna databases 
* (https://github.com/shiftx/faunadb-fql-lib)[faunadb-fql-lib] - JS library with utility functions that extends FQL with just FQL
* (https://github.com/lkatartn/fill-fauna)[Fill Fauna] - Fill your faunaDB collection with data from JSON file
* (https://github.com/gahabeen/nanohash)[Nanohash] - A tiny unique string ID generator including a matching 64-bit numeric value
* (https://github.com/trevorsibanda/fauna-tool)[Tool that translates Fauna's wire protocol to FQL] 

# Gists

* (https://gist.github.com/BrunoQuaresma/0236aff64dc44795f19994cbc7a07db6)[useFauna()] - React hook used to run Fauna queries
* (https://gist.github.com/ptpaterson/82c01afc9b0ff624f96141a078b5ab54)[Template for building deeply nested FQL queries] 
* (https://gist.github.com/tovbinm/5996221ab7a5ecd3d2afbfcd69d6f8e3)[Docker container testing trait for Scala] 

# Sample/starter apps

All of the apps included here should be open source, with repositories you can fork/clone and run locally.

## React

* (https://github.com/netlify/netlify-faunadb-example)[netlify-faunadb-example] - Currently our most popular sample application. A lot of the other example apps, even those in other JS frameworks, are based on this. React frontend, Netlify Functions for API calls, and FaunaDB.

### Authentication examples

* (https://github.com/ptpaterson/netlify-faunadb-graphql-auth)[netlify-faunadb-graphql-auth] - A version of the netlify-faunadb-example, using HTTP-only cookies for authentication with FaunaDB's native GraphQL API
* (https://github.com/zeit/next.js/tree/master/examples/with-cookie-auth-fauna)[with-cookie-auth-fauna] - Cookie authentication using FaunaDB with Zeit Now
* (https://github.com/fillipvt/with-faunadb-abac-auth)[with-faunadb-abac-auth] - Next.js + FaunaDB Cookie Based Login + ABAC + Apollo GraphQL
* (https://github.com/j0lv3r4/nextjs-auth0-fauna)[nextjs-auth0-fauna] - Serverless authentication example with Next.js, Auth0, Fauna, and ZEIT Now

### Incorporating Very Good Security [VGS]
* (https://github.com/preconceptioncode/netlify-faunadb-example)[A version of netlify-faunadb-example incorporating VGS] - For interacting with regulated, sensitive data without the liability of securing it [e.g., for compliance with HIPAA, GDPR, etc.]

### Incorporating web sockets
* (https://github.com/chron/clap)[Synchronized Claps with React on Netlify + FaunaDB + Pusher]
* (https://github.com/chron/outpost18)[Outpost 18] - Real-time card game for two players

## Starter projects

* (https://www.npmjs.com/package/fauna-nf)[fauna-nf] - npm install a fork of Create React App, with a Fauna backend

### Other React apps

* (https://github.com/NickFoden/flash-fauna)[flash-fauna] - Flash cards app using FaunaDB and some hooks
* ()[]
* ()[]
* ()[]


## Vue

* ()[]
* ()[]
* ()[]
* ()[]

## Typescript

* (https://github.com/BrunoQuaresma/justnotes.io)[Just notes] - Note-taking app by one of Fauna's frontend engineer's, using Create React App, Redux Starter Kit, React Redux, and Typescript [(https://www.brunoquaresma.dev/new-project-justnotes-io/)[related blog]]
* ()[]
* ()[]
* ()[]

## Svelte

* (https://github.com/ganesankar/cv-svelte-netlify-faunadb)[Responsive CV/Resume SPA using Svelte, bulma, and Netlify Functions]
