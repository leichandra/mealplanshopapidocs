---
description: Requests and Responses are in JSON format.
---

# Agendas

{% api-method method="get" host="http://mealplanshop.herokuapp.com" path="/api/agendas/" %}
{% api-method-summary %}
Get the agendas list for a user.
{% endapi-method-summary %}

{% api-method-description %}
You can get the list of agendas.
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

{% api-method method="post" host="http://mealplanshop.herokuapp.com" path="/api/agendas/" %}
{% api-method-summary %}
Create an agenda for a given date.
{% endapi-method-summary %}

{% api-method-description %}
The following is a sample request body.  
`{   
     "date": "2021-04-28",   
     "breakfast_recipe": 8,   
     "lunch_recipe": 11,   
     "dinner_recipe": 20   
}`  
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="dinner\_recipe" type="integer" required=false %}
Dinner recipe id 
{% endapi-method-parameter %}

{% api-method-parameter name="date" type="string" required=false %}
String representing the date with the 4 digit year separated by a dash, the month with a leading 0, and the day with a leading 0 such as: "2021-04-28"
{% endapi-method-parameter %}

{% api-method-parameter name="breakfast\_recipe" type="integer" required=false %}
Breakfast recipe id
{% endapi-method-parameter %}

{% api-method-parameter name="lunch\_recipe" type="integer" required=false %}
Lunch recipe id
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "id": 5,
    "date": "2021-04-28",
    "breakfast_recipe": 8,
    "lunch_recipe": 11,
    "dinner_recipe": 20
}

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="http://mealplanshop.herokuapp.com" path="/api/agendas/{agenda id}" %}
{% api-method-summary %}
Get the information for an agenda given the agenda id.
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="{agenda id}" type="integer" required=false %}
The agenda id
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "date": "2021-04-28",
    "breakfast_recipe": 20,
    "lunch_recipe": 4,
    "dinner_recipe": 19
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="patch" host="http://mealplanshop.com" path="/api/agenda/{agenda id}" %}
{% api-method-summary %}
Update an agenda date.
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="{agenda id}" type="integer" required=false %}
This is the agenda id
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter type="string" name="date" %}
String representing the date with the month spelled out with the first letter capitalized, the day in number format \(without a leading zero\), and a four digit year such as: "April 2, 2021"
{% endapi-method-parameter %}

{% api-method-parameter type="integer" name="breakfast\_recipe" %}
Breakfast recipe id
{% endapi-method-parameter %}

{% api-method-parameter type="integer" name="lunch\_recipe" %}
Lunch recipe id
{% endapi-method-parameter %}

{% api-method-parameter type="integer" name="dinner\_recipe" %}
Dinner recipe id
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "id": 5,
    "date": "April 28, 2021",
    "breakfast_recipe": 8,
    "lunch_recipe": 11,
    "dinner_recipe": 20
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="http://mealplanshop.herokuapp.com" path="/api/agendas/{agenda id}" %}
{% api-method-summary %}
Delete an agenda date.
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="{agenda id}" type="integer" required=false %}
This is the agenda id
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

