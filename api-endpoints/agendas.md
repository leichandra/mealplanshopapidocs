# Agendas

{% api-method method="get" host="http://mealplanshop.herokuapp.com" path="/api/agendas/" %}
{% api-method-summary %}
Get the agendas list for a user.
{% endapi-method-summary %}

{% api-method-description %}
You can get the list of agendas for a user with a list of recipe ids.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="" type="string" required=false %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "agendas": [
        {
            "id": 4,
            "date": "April 1, 2021",
            "breakfast_recipe": 9,
            "lunch_recipe": 54,
            "dinner_recipe": 6
        },
        {
            "id": 5,
            "date": "April 2, 2021",
            "breakfast_recipe": 86,
            "lunch_recipe": 4,
            "dinner_recipe": 67
        },
        {
            "id": 6,
            "date": "April 3, 2021",
            "breakfast_recipe": 5,
            "lunch_recipe": 33,
            "dinner_recipe": 43 
        },
        {
            "id": 7,
            "date": 22,
            "breakfast_recipe": 48,
            "lunch_recipe": 3,
            "dinner_recipe": 8
        }
    ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="http://mealplanshop.herokuapp.com/api/agendas" path="/" %}
{% api-method-summary %}
Create an agenda for a given date for a user.
{% endapi-method-summary %}

{% api-method-description %}
Create an agenda for a given date for a user.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="" type="string" required=false %}

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

{% api-method method="get" host="http://mealplanshop.herokuapp.com/api/agendas/{agenda id}/" path="" %}
{% api-method-summary %}
Get the information for an agenda given the agenda id.
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="" type="string" required=false %}

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

{% api-method method="patch" host="http://mealplanshop.com/api/agenda/{agenda id}/" path="" %}
{% api-method-summary %}
Update an agenda date.
{% endapi-method-summary %}

{% api-method-description %}
Update an agenda date.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="" type="string" required=false %}

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

{% api-method method="delete" host="http://mealplanshop.herokuapp.com/api/agendas/{agenda id}/" path="" %}
{% api-method-summary %}
Delete an agenda date.
{% endapi-method-summary %}

{% api-method-description %}
Delete an agenda date.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="" type="string" required=false %}

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

