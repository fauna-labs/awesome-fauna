# awesome-fauna

Curated list of Fauna resources that live outside of the fauna.com or docs.fauna.com domains. Please feel free to make a PR to add more, or to propose a different organizational structure.

> [!WARNING]
> Fauna is decommissioning FQL v4 on June 30, 2025.
>
> Many of the resources here still rely on FQL v4. FQL v10 is recommended for
> all new projects.
>
> Accounts created after August 21, 2024 must use FQL v10. Ensure you migrate
> existing projects to the official v10 drivers by the v4 EOL date.
>
> For more information, see the [v4 end of life (EOL)
> announcement](https://docs.fauna.com/fauna/v4/#fql-v4-end-of-life) and
> [related FAQ](https://docs.fauna.com/fauna/v4/migration/faq).

### :bookmark_tabs: Contents

- [Open source Sample apps](#open-source-example-apps)
- [Videos](#videos)
	- [Coding tutorial videos](#coding-tutorial-videos)
	- [Database concept videos](#database-concept-videos)
- [Podcasts](#podcasts)
- [Database concepts](#database-concepts)


## Sample apps
All of the apps included here should be open source, with repositories you can fork/clone and run locally.

* [JavaScript/TypeScript backend](https://github.com/fauna/js-sample-app) - This sample app shows how to use Fauna in a production application.
The app uses Node.js and the Fauna v10 JavaScript driver to create HTTP API endpoints for an e-commerce store. You can use the app's API endpoints to manage products, customers, and orders for the store.
* [Java](https://github.com/fauna/java-sample-app) - This sample app shows how to use Fauna in a production application.
The app uses Java 17 with Gradle 8.9 and the Fauna v10 JVM driver to create HTTP API endpoints for an e-commerce store. You can use the app's API endpoints to manage products, customers, and orders for the store.
* [Event Streaming](https://github.com/fauna-labs/chat-app-streaming) - This reference application show how you can use Fauna Event Streaming to build real-time apps. You can use it as a starting point for your apps.


#### Other example apps using React
* [Just notes](https://github.com/BrunoQuaresma/justnotes.io) - Note-taking app by one of Fauna's frontend engineer's, using Create React App, Redux Starter Kit, React Redux, and Typescript ([related blog](https://www.brunoquaresma.dev/new-project-justnotes-io/))
* [fauna-market](https://github.com/fauna/fauna-market) - A market for Emoji goods, to demonstrate global consistency in Fauna
* [flash-fauna](https://github.com/NickFoden/flash-fauna) - Flash cards app using Fauna and some hooks
* [serverless-graphql-potter](https://github.com/molebox/serverless-graphql-potter) - A playground project for practicing serverless graphql end points. Built with Gatsby, Netlify functions, Apollo, and Fauna. Data provided via the Potter API.
* [Games built with Next.js and Fauna](https://github.com/goldenshun/botwise) - A set of simple games built with Fauna and Next.js which can be seen in action on https://botwise.games/.

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