# Fullstack GraphQL

> Learn how to use GraphQL with Node and React

This course comes with some [slides](https://docs.google.com/presentation/d/1IrGA4PtUEZPVDTBg5_WCMmUapElbFBgLwfSBAp8ft1g/edit?usp=sharing)

## What you'll need

- Node version >= 6

## Solutions

The solution branch has the completed course fo reference. There is no one way to finish this course.
`git checkout solution`

# Learning

query on graphql

```gql
query AllCharacter($page: Int) {
  # AllCharacter was a query name, it can be defined at Client Side
  characer(page: $page) {
    # $page was a dynamic variable that can be passed on `Query Variable` on playground
    results {
      fullName: name # so fullName is alias for name,client can't change the BE so the make alias to the name they want
    }
  }
}
```

you can have multiple query in 1 api call

### Appolo Client

use to replace JQUery AJAX and or Axios, can use for state - management and caching ( can be use to replace redux or working with redux)
