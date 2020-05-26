---
description: Embedded Web REST API
---

# REST API

The login server has an embedded web server that servers an API on port 6000 unless otherwise specified in the config

{% code title="login.json" %}
```javascript
{
  "web_api": {
    "enabled": true, // enable/disable embedded webserver api
    "port": 6000 // the port you want the web api to serve on (recommended not to change)
  },
}
```
{% endcode %}

You have the option to disable it, or change the port altogether

## API Tokens

The login server requires API tokens to interact with the API, they can be generated via the CLI

### Using the CLI Interface

```bash
eqemu@dc25a75287d7:~/server$ ./loginserver web-api-token:create --write --read
```

The token will persist to the `login_api_tokens` table

```text
MariaDB [peq]> select * from login_api_tokens;
+----+--------------------------------------+-----------+----------+---------------------+---------------------+
| id | token                                | can_write | can_read | created_at          | updated_at          |
+----+--------------------------------------+-----------+----------+---------------------+---------------------+
|  1 | b1bb9eb7-416c-487a-bb91-aedc59e0c57d |         1 |        1 | 2019-09-17 04:23:30 | 2019-09-17 04:23:30 |
+----+--------------------------------------+-----------+----------+---------------------+---------------------+
```

{% hint style="warning" %}
To create read only users, simply specify **only** the **--read** flag when creating users
{% endhint %}

{% hint style="info" %}
**Note** As a general rule, API calls that are **GET** are going to require **--read** while **POST** HTTP calls will require **--write**
{% endhint %}

## API Endpoints

The login server has a small handful of endpoints which have been created, it is easy to add more as needed

## PHP Client

There is an example of a PHP client that interacts with this API located here

{% embed url="https://github.com/Akkadius/eqemu-loginserver-php-api-client" %}

## Login Accounts

{% api-method method="post" host="http://loginserver:6000" path="/v1/account/create" %}
{% api-method-summary %}
Login Account Create
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Authorization: Bearer &lt;token&gt;
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
[
	{
		"local_ip" : "127.0.0.1",
		"players_online" : 0,
		"remote_ip" : "",
		"server_list_id" : 3,
		"server_long_name" : "Akkas Docker PEQ Installer (L)",
		"server_short_name" : "Akkas Docker PEQ Installer (L)",
		"server_status" : -2,
		"zones_booted" : 0
	}
]
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% code title="Request Body" %}
```text
{
    "username": "test",
    "password": "test",
    "email": "<optional>"
}
```
{% endcode %}

{% api-method method="post" host="http://loginserver:6000" path="/v1/account/credentials/validate/local" %}
{% api-method-summary %}
Validate Login Account Credentials
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Authorization: Bearer &lt;token&gt;
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "data": {
        "account_id": 3,
    },
    "message": "Credentials valid!"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% code title="Request Body" %}
```javascript
{
    "username": "test",
    "password": "test",
    "email": "<optional>"
}
```
{% endcode %}

{% api-method method="post" host="http://loginserver:6000" path="/v1/account/credentials/update/local" %}
{% api-method-summary %}
Update Login Account Credentials
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Authorization: Bearer &lt;token&gt;
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "message": "Loginserver account credentials updated!"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=400 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
{
    "error": "Failed to update loginserver account credentials!"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

```javascript
{
    "username": "test",
    "password": "newpassword"
}
```

## World Servers

{% api-method method="get" host="http://loginserver:6000" path="/v1/servers/list" %}
{% api-method-summary %}
Get World Server List
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Authorization: Bearer &lt;token&gt;
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```
[
	{
		"local_ip" : "127.0.0.1",
		"players_online" : 0,
		"remote_ip" : "",
		"server_list_id" : 3,
		"server_long_name" : "Akkas Docker PEQ Installer (L)",
		"server_short_name" : "Akkas Docker PEQ Installer (L)",
		"server_status" : -2,
		"zones_booted" : 0
	}
]
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

