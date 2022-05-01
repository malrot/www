---
layout: base.hbs
title: MALROT – API Documentation
---

# [←](/) API Doc

## Introduction

_Work in progress. API returns fake or no data. Do not use._

MALROT `API` is **no-auth**, **public** and **forever free to use**. It's also **static** because it doesn't perform any action other than delivering flat JSON files that live on a CDN.

This `API` is organized around REST, has predictable resource-oriented URL, uses standard HTTP codes and verbs, and returns JSON (see [API code](https://github.com/malrot/malrot-api)).

All endpoints below assume `HTTP 200 OK`. Payload examples are fictional.

## > List events

### Endpoint

```http
GET https://api.malrot.org/v1/events?PARAMETERS
```

**Optional parameters**

- `org`
  - A filter on the list based on the organization domain name
  - Value must be a string (e.g. `louvre.fr`)
  - Only one value is allowed (e.g. `org=louvre.fr`)
- `country`
  - A filter on the list based on the country where the event occurs
  - Value must be a valid ISO 3166-1 alpha-2 string (e.g. `FR` for France)
  - Multiple values, separated by a comma, are allowed (e.g. `country=FR,BE,LU`)
- `around`
  - A filter on the list based on a geographic point (WGS 84) and a radius around this point
  - Value must be a string of 3 numbers separated by a comma (e.g. `4.805,43.949,10`)
    - First number must be the _longitude_ of the center of the search area
    - Second number must be the _latitude_ of the center of the search area
    - Third number must be the _radius_ in kilometers of the search area
- `updated_after`
  - A filter on the list based on when an event has been updated
  - Value must be a Unix timestamp (e.g. `1647420160`)

### Returns a JSON array of objects

```jsonc
[
  {
    "endpoint":"https://api.malrot.org/v1/events/louvre.fr__defF7d1D.json",
    "country":"FR",
    "created_at":1644401946288,
    "updated_at":1644738558865,
    "longitude":4.805,
    "latitude":43.949,
    "distance":9.45
    },
    {...}
  ]
```

### With properties

| PROPERTY   | TYPE     | DESCRIPTION                                                   |
| ---------- | -------- | ------------------------------------------------------------- |
| endpoint   | `string` | API endpoint to event data                                    |
| created_at | `number` | When this event has been created (Unix timestamp)             |
| updated_at | `number` | When this event has been updated (Unix timestamp)             |
| country    | `string` | ISO 3166-1 alpha-2 country code where the event occurs        |
| longitude  | `number` | WGS 84 longitude of the event                                 |
| latitude   | `number` | WGS 84 latitude of the event                                  |
| distance   | `number` | Distance in km between event and `GET` params _(if provided)_ |

## > Get event data

### Endpoint

```http
GET https://api.malrot.org/v1/events/:event
```

### Returns

`JSON` data, formatted according to MALROT [specification](https://spec.malrot.org) and describing an event.

## > Check API health

### Endpoint

```http
GET https://api.malrot.org/v1/health
```

### Returns

`HTTP 200 OK` if `API` and `CDN` are up and running.
