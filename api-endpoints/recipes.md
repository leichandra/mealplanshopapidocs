# Recipes

{% api-method method="get" host="https://mealplanshop.herokuapp.com" path="/api/recipes" %}
{% api-method-summary %}
Returns list of recipes
{% endapi-method-summary %}

{% api-method-description %}
You will see a list of recipes for a given user.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
You should get a return of the list of recipe names for a given user.
{% endapi-method-response-example-description %}

```
{
    "recipes": [
        {
            "name": "pop tart"
        },
        {
            "name": "jello pudding"
        },
        {
            "name": "k"
        },
        {
            "name": "jambalya"
        }
    ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://mealplanshop.herokuapp.com" path="/api/recipes/" %}
{% api-method-summary %}
Create a recipe for a user.
{% endapi-method-summary %}

{% api-method-description %}
You will be able to create a recipe with this method.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-form-data-parameters %}
{% api-method-parameter name="instructions" type="string" required=false %}
Instructions for the recipe
{% endapi-method-parameter %}

{% api-method-parameter name="ingredients" type="string" required=false %}
Ingredients used in a recipe
{% endapi-method-parameter %}

{% api-method-parameter name="name" type="string" required=true %}
The recipe name
{% endapi-method-parameter %}
{% endapi-method-form-data-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "id": 54,
    "name": "pop tart",
    "created_at": "08/07/2020",
    "updated_at": "04/01/2021",
    "ingredients": "pop tart",
    "Instructions": "1. Put pop tart in toaster\n2. Let cool down\n3. Eat"
}



```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://mealplanshop.herokuapp.com" path="/api/recipes/{recipe id}/" %}
{% api-method-summary %}
Get the recipe id for a user.
{% endapi-method-summary %}

{% api-method-description %}
Get the recipe id if you have the user id.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="{recipe id}" type="number" required=true %}
This is the recipe id.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "name": "pop tart",
    "created_at": "08/07/2020",
    "updated_at": "04/01/2021",
    "ingredients": "pop tart",
    "Instructions": "1. Put pop tart in toaster\n2. Let cool down\n3. Eat"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="patch" host="https://mealplanshop.com/herokuapp.com/api" path="/api/recipes/{recipe id}/" %}
{% api-method-summary %}
Update the information for a recipe.
{% endapi-method-summary %}

{% api-method-description %}
Update the information for a recipe given the recipe id.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="{recipe id}" type="integer" required=true %}
This is the recipe id
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="name" type="string" required=false %}
This is the name of the recipe
{% endapi-method-parameter %}

{% api-method-parameter name="ingredients" type="string" required=false %}
This includes the ingredients of the recipe
{% endapi-method-parameter %}

{% api-method-parameter name="instructions" type="string" required=false %}
This includes the instructions for the recipe
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "name": "pop tart",
    "created_at": "08/07/2020",
    "updated_at": "04/01/2021",
    "ingredients": "pop tart",
    "Instructions": "1. Put pop tart in toaster\n2. Let cool down\n3. Eat"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://mealplanshop.herokuapp.com" path="/api/recipe/{recipe id}/" %}
{% api-method-summary %}
Delete a recipe
{% endapi-method-summary %}

{% api-method-description %}
Delete a recipe given a recipe id.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="{recipe id}" type="integer" required=false %}
This is the recipe id.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

