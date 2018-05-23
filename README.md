# Quantified-Self

Quantified Self is an exercise in creating RESTful APIs in three different languages: Ruby/Rails, Node.js/Express and Elixir/Phoenix.  The original projec spec can be found [here](http://backend.turing.io/module4/projects/quantified-self/quantified-self).

Below are the repositories for each Quantified Self application:

* [Ruby on Rails](https://github.com/memcmahon/quantified_self)
* [Node.js](https://github.com/memcmahon/quantified-self-express)
* [Elixir](https://github.com/memcmahon/quantified-self-phoenix)

The instructions for starting each of these locally can be found on their individual repos. The following information is common to the three applicaitons above.

## Schema

![Imgur](https://i.imgur.com/T6ImmLI.png)

## Endpoints

### Food Endpoints

```
GET /api/v1/foods
```
```
GET /api/v1/foods/:id
```
```
POST /api/v1/foods
   with body: { "food": { "name": "Name of food here", "calories": "Calories here"} }
```
```
PATCH /api/v1/foods
   with body: { "food": { "name": "Name of food here", "calories": "Calories here"} }
```
```
DELETE /api/v1/foods/:id
```

### Meal Endpoints
```
GET /api/v1/meals
```
```
GET /api/v1/meals/:meal_id/foods
```
```
POST /api/v1/meals/:meal_id/foods/:food_id
```
```
DELETE /api/v1/meals/:meal_id/foods/:food_id
```
