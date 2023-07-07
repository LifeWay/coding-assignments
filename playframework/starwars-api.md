
### Star Wars Coding Assignment

Create a REST API using one of the following technologies in Scala:

* Play Framework 2.8
* ZIO Http
* Akka Http
* AWS Serverless App with JVM lambdas (latency will be ignored for the purpose of this assignment)


Your API must do the following:
* Wrap the Star Wars API (https://swapi.dev/) exposing a single endpoint: `/person/{id}`. Given that I call `/person/1`, for example, I expect to see the following information which you must obtain using various calls to the Star Wars API.

```
{
    "name": "Luke Skywalker",
    "homeworld": "Tatooine",
    "starshipsFlown": [
        {
            "name": "X-wing",
            "crew": "1",
            "passengers": "0"
        },
        {
            "name": "Imperial shuttle",
            "crew": "6",
            "passengers": "20"
        }
    ]
}
```
* Your API must be non-blocking (if using standard scala futures) or properly using the ZIO effect system.

## What we are looking for:
* We are interested in the readability, modularity, and testability of your implementation. Please imagine that this small example is going to turn into a larger application with 30+ endpoints and structure your code accordingly.

Do not commit your example onto a public repository. Please send us a zip file of your code. We will compile it locally and run it.
