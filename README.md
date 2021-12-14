# SubQuery - Balances Transfers

#### Run required systems in docker


Under the project directory run following command:

```
docker-compose pull && docker-compose up
```
#### Query the project

Open your browser and head to `http://localhost:3000`.

Finally, you should see a GraphQL playground is showing in the explorer and the schemas that ready to query.

For the `subql-starter` project, you can try to query with the following code to get a taste of how it works.

````graphql
{
  query{
    transfers(first:5){
      nodes{
        id,
        amount,
        blockNumber,
        to {
          id
        }
      }
    }
  }
}
````
