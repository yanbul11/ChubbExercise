# ChubbExercise
Coding Exercise

The solution is a WebAPI and uses SQLite, Entity Framework and .NET Core.

The WebAPI provides 2 services with the reuqested functionality:

1. To retrieve as a food provider the number of portions of tiramisu per restaurant: /api/chain/demands/[productId], e.g. /api/chain/demands/1.
2. To retrieve as a restaurant chef the number of eggs to be supplied: api/restaurant/supply/[restaurantId]/[materialId], e.g. api/restaurant/supply/1/1.

The solution includes sample data and unit tests. A database diagram can also be found in the repository.

Note:
The proportion 1 tiramisu / 3 eggs is not applied in the solution as the requested functionalities don't include calculation of eggs needed, e.g. the request is "I would like to know the number of portions of tiramisu ordered by clients for each restaurant so I can order enough eggs for next month", so what is asked is the number of portions of tiramisu, not of the eggs that will be needed for these.
Such a functionality can be added with an addition to the database schema to relate Products and Materials so that we know which materials and in which quantity are needed for each product.
