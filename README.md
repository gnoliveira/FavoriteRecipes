The structure is quite straightforward, divided into controller, service and repository.

I added all the endpoints requested, but implemented the add and update in a single upsert endpoint.
Also added an endpoint to retrieve all the recipes, with no filtering, for debugging.

I used Intellij to create the application, with a default setup, so it can be easily run with any other environment using maven.

There is a postman collection included with the endpoints, each configured with valid data.

I used "tags" in the Recipes, instead of a boolean for "vegetarian", this way it can support other restrictions like vegan or halal.
But did only part of the filtering in the query itself, and another part on the Service logic, because I was too tired to think of proper database schema and query. (Used JPA Query Methods only)

Also didn't add the tests for the same reason (just got home from a 12hrs flight, so ...)