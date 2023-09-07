# Book Search Engine

## Description
This is a book search engine that allows the user to search for their desired books and save them.

[Deployed Link](https://arcane-atoll-01869-41519f6b8d63.herokuapp.com/)

![Book Search](./assets/booksearch.png)

## Built With
* [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
* [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
* [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
* [Git](https://git-scm.com/)
* [Express](https://expressjs.com/en/guide/routing.html)
* [React](https://react.dev/learn)
* [GraphQL](https://graphql.org/learn/)
* [Apollo](https://www.apollographql.com/docs/apollo-server/)

## Usage
The user can travel to the deployed site and create an account using the signup. The User can then search for books and add any of them to their saved books.

## Learning Points
* Using GraphQL queries
* Creating a schema folder for resolvers and typeDefs
* Deploying an application to heroku with MongoDB

## Important Code
```js
 Query: {
    me: async (parent, args, context) => {
      if (context.user) {
        return User.findOne({ _id: context.user._id });
      }
      throw AuthenticationError;
    }
  }
```
This code represents the query that is performed when a GraphQL query is made

## Author Info

### Timothy Su

* [LinkedIn](https://www.linkedin.com/in/timothysu1/)
* [Github](https://github.com/timothysu1)

## License

Please refer to license in the repo. 

## Contributions
N/A
