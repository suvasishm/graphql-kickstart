# graphql-kickstart
Understanding GraphQL


Key points:
1. New API standard; alternative to REST; a better REST
1. Query language for API
1. Declarative data fetching; get exactly what you need from an API
1. GraphQL server expose a _single endpoint_ and responds with precisely the data that was queried from the client
1. Developed by Facebook for efficient data loading to serve application even in poor network/low bandwidth situation
1. GraphQL has its own type system that is used to define schema of an API. [SDL](https://www.prisma.io/blog/graphql-sdl-schema-definition-language-6755bcb9ce51)
1. GraphQL schema defines capabilities of the API and defines how clients can create/update (Mutations) and fetch data;
contract between the client and server; collection of GraphQL types
1. Each schema will have some Root types: Query, Mutation, Subscription
1. Possible to define relationships between types
1. _Single Endpoint_ architecture is radically different from REST endpoints. This works because structure of the data 
that is retuned is not fixed. The client decides (through query) what it needs from the API. 

GraphQL server and use cases:
1. GraphQl is only a specification [Ref# 3]. Implement your server in the language of your [choice](https://www.howtographql.com/choose/).
1. GraphQL is transport layer agnostic
1. Can be connected with SQL/NOSQL database
1. Can be integrated with existing legacy systems behind a single coherent GraphQL API
1. Payload of a GraphQL queries/mutations consist of a set of fields
1. GraphQL server has one resolver function per field

GraphQL client:
1. You have to just fire queries following the schema!

Ref: 
1. https://www.howtographql.com/
1. https://github.com/howtographql/howtographql
1. http://spec.graphql.org/
1. Netflix has similar solution called [Falcor](https://netflix.github.io/falcor/)
