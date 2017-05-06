---
title: Example

area_tabs:
  - design: Design
  - ux: UX
  - ui: UI
  - backend: Backend
  - qe: QE
  - support: Support
  - resources: Resources
  - planning: Planning
  - notes: Notes

search: true
---

# Introduction

This is an example page that uses the customized Slate theme. Click [here](../users/index.html) to view the User Guide for Syndesis.


<blockquote class="area-specific design">
You must replace <code>meowmeowmeow</code> with your personal API key.
</blockquote>

<blockquote class="area-specific qe">
QE
</blockquote>

<blockquote class="area-specific design">
Design
</blockquote>

<blockquote class="area-specific backend">
</blockquote>

```backend
Backend
```


# Architecture

Coming soon.

<blockquote class="area-specific ui qe notes">
UI You must replace <code>meowmeowmeow</code> with your personal API key.
</blockquote>

<blockquote class="area-specific design">
<img src="https://cloud.githubusercontent.com/assets/3844502/24225759/9d8ebdd6-0f38-11e7-8c76-8d6ce48dda5f.jpg">
</blockquote>

```ruby
UX 2
<img src="https://cloud.githubusercontent.com/assets/3844502/24225759/9d8ebdd6-0f38-11e7-8c76-8d6ce48dda5f.jpg">
```

# Getting Started

## API

The API can be run locally or you can use the staging API. If you'll strictly be working on the UI, or just want to get the app running as quickly as possible, we recommend using the API staging server rather than running it locally. 

### Running the API Locally

Instructions here.


### Authentication

>  To authorize via the UI, simply access it in your browser, where you'll be redirected to an OpenShift login/registration page where you are prompted for your name, email address, etc. You'll then be redirected to a  GitHub permissions page. You'll be prompted to grant OpenShift the proper permissions. Once you accept, you'll finally be granted access to the UI. You should only need to do this once. 


```python
Design
<img src="https://cloud.githubusercontent.com/assets/3844502/24225759/9d8ebdd6-0f38-11e7-8c76-8d6ce48dda5f.jpg">
```

```csharp
Backend
import kittn

api = kittn.authorize('meowmeowmeow')
```

```php
QE
# With shell, you can just pass the correct header with each request
curl "api_endpoint_here"
  -H "Authorization: meowmeowmeow"
```

```c
Notes
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
```

> Make sure to replace `meowmeowmeow` with your API key.

Kittn uses API keys to allow access to the API. You can register a new Kittn API key at our [developer portal](http://example.com/developers).

Kittn expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: meowmeowmeow`

<aside class="notice">
You must replace <code>meowmeowmeow</code> with your personal API key.
</aside>


## Running the UI

Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Curabitur blandit tempus porttitor. Vestibulum id ligula porta felis euismod semper.

Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Aenean lacinia bibendum nulla sed consectetur. Maecenas faucibus mollis interdum. Cras justo odio, dapibus ac facilisis in, egestas eget quam.

### If you'll be using the staging API

Coming soon.

### If you've set up the API locally

Coming soon.


# Pages

## Connections

### Create Connection

## Integrations

### Integration List

### Create Integration

## Tags

### Create Tag

## Templates

### Create Tag

## Users

# Tests

## E2E Tests

Points of Contact: 

[Happy Path](https://issues.jboss.org/browse/IPAAS-285) for E2E Tests


## Unit Tests

We are very behind on unit tests.


# Contributing

## UI

We have a [Style Guide](https://github.com/syndesisio/syndesis-ui-style-guide) for the UI that should be followed when contributing. In addition, we follow the [official Angular 2 Style Guide](https://angular.io/styleguide) when possible.


# Kittens

## Get All Kittens

```php
QE
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.get
```

```ruby
Notes
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.get()
```

```java
Backend
curl "http://example.com/api/kittens"
  -H "Authorization: meowmeowmeow"
```

```csharp
Design
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let kittens = api.kittens.get();
```

> The above command returns JSON structured like this:

```ruby
UX
[
  {
    "id": 1,
    "name": "Fluffums",
    "breed": "calico",
    "fluffiness": 6,
    "cuteness": 7
  },
  {
    "id": 2,
    "name": "Max",
    "breed": "unknown",
    "fluffiness": 5,
    "cuteness": 10
  }
]
```

This endpoint retrieves all kittens.

### HTTP Request

`GET http://example.com/api/kittens`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
include_cats | false | If set to true, the result will also include cats.
available | true | If set to false, the result will include kittens that have already been adopted.

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Get a Specific Kitten

```c
UI
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.get(2)
```

```python
UX
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.get(2)
```

```javascript
Design
curl "http://example.com/api/kittens/2"
  -H "Authorization: meowmeowmeow"
```

```python
Notes
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let max = api.kittens.get(2);
```

> The above command returns JSON structured like this:

```python
Notes
{
  "id": 2,
  "name": "Max",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```

This endpoint retrieves a specific kitten.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### HTTP Request

`GET http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to retrieve
