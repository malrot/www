---
layout: base.hbs
title: MALROT – Making cultural event data universally accessible
---

# MALROT

Making cultural event data universally accessible.

## TL;DR

Cultural institutions are experts at organizing events and exhibitions, but they might have less experience building apps. MALROT (pronounced `/mal-ROH/`) lets them publish their events data **once** and **worldwide** (while staying in full control) and developers **freely** consume these data to build innovative services.

At its core, MALROT is 4 things:

- A **simple**, **open** and **interoperable file format** that describes cultural events and associated metadata like schedules, description, location, etc.

- An **open-access repository** where live worldwide, standardized and up-to-date cultural events data (aka MALROT file) or link to them.

- A **public static `API`** allowing anyone to consume MALROT files (JSON files that live on a _Content Delivery Network_) and build app.

- **Open-source tools** to help generate, validate and host MALROT files.

## How do I start?

- **Quick links**

  - Read MALROT [specification](https://spec.malrot.org) (_work in progress_)
  - [Start a discussion](https://github.com/orgs/malrot/discussions/categories/spec) if you have any ideas

- **Full table of contents**
  - [What are the problems MALROT wants to solve?](#problems)
  - [So what's MALROT?](#whats)
  - [What are the benefits?](#benefits)
  - [What's next: I'm a cultural institution](#concretely)
  - [What's next: I'm a developer, data-scientist or enthusiast](#concretely)
  - [Contributing to MALROT](#contributing)
  - [Project Status](#status)
  - [License](#license)

## <a name="problems"></a>What are the problems MALROT wants to solve?

### Undiscoverable culture = no culture

Nowadays, you can order a cab or book a room with your phone in seconds almost everywhere in the world, but can't get a quick answer to _"is there, one kilometer around, a painting exhibition opened this evening, accessible to the disabled and free?"_. That's not understandable.

### Time and money to create culture, not to copy/paste agendas

Cultural institutions spend a lot of time sending their calendars to media or filling forms to list their events in some closed and not so well-known platforms. At the same time, media manually type cultural calendars into their _Content Management System_.

Both are a time consuming, error prone, low value-added and never ending task to get nor an exhaustive nor an accurate listing. What a mess.

### No standard + no open data = no innovation

Before 2005, there were no transit routes in Google Maps and other mobility apps, and no innovation in riders experience. At this time, it was missing _(i)_ a data specification that allows transit agencies to publish their data in an interoperable format and _(ii)_ transit operators open data. Since the invention of [GTFS](https://en.wikipedia.org/wiki/General_Transit_Feed_Specification), an array of services has appeared for the greatest good.

Such a move is yet to be made in arts and culture.

### Ticket fees must fund culture, not middlemen

Proprietary ticketing plateforms are complex middlemen and often a crossing point for public because they aggregate a part of cultural events.

Cultural institutions should regain control of their ticketing gateway while communicating their events simply, quickly and broadly.

## <a name="whats"></a>So what's MALROT?

At its core, MALROT is 4 things:

- A **simple**, **open** and **interoperable file format** that describes cultural events and associated metadata like schedules, description, location, etc.

- An **open-access repository** where live worldwide, standardized and up-to-date cultural events data (aka MALROT file) or link to them.

- A **public static `API`** allowing anyone to consume MALROT files (JSON files that live on a _Content Delivery Network_) and build app.

- **Open-source tools** to help generate, validate and host MALROT files.

## <a name="benefits"></a>What are the benefits?

- **For cultural institutions**

  - Engage with **broader** and **new audiences**
  - Get a **renewed control** of your ticketing gateway and **increase revenue**
  - Publish your events **worldwide** in a **one-time** task
  - Keep **full** and **constant control** over your event data
  - **Devote less resources** to low value-added and repetitive tasks

- **For people**

  - Have **all surrounding cultural events** at your fingertips
  - Get a brand new **cultural and area discovery experience**

- **For media and platforms**

  - **Waste less** time manually typing events into your systems
  - **Invest more** time curating and editorializing events

- **For developers**

  - Build amazing apps and invent new services!
  - Request a public `API` to `GET` worldwide cultural events data
  - Use a standard and interoperable format, fully documented

- **For public authorities**

  - Make **local cultural events discovery** far more easier
  - Increase **territorial attractiveness** and local GDP

## <a name="concretely"></a>Concretely, what's next?

_Some tools are currently unavailable until MALROT spec reaches a stable version._

- **I'm a cultural institution and I want to:**
  - contribute to MALROT [spec](#spec)
  - ~~generate and host events on MALROT website _(forever free)_~~
- **I'm an enthusiat, developer or data-scientist and I want to:**
  - contribute to MALROT [spec](#spec), [tools](#tools) or [API](#tools)
  - read [`API` docs](/api) to consume MALROT files (_work in progress_)

## <a name="contributing"></a>Contributing

Help and support are more than welcome to make MALROT real.  
See [roadmap and TODO](https://github.com/orgs/malrot/projects/1).

### <a name="spec"></a>Contribute to MALROT spec

You can [read](https://spec.malrot.org) MALROT specification (_work in progress_) and [give feedback](https://github.com/orgs/malrot/discussions/categories/spec).

### <a name="tools"></a>Build and make better open source tools

MALROT tools are an [API](https://github.com/malrot/api) and an [app](https://github.com/malrot/app) for generating, validating and hosting MALROT files (_works in progress_). Do not hesitate to make improvements, add tests, report bugs. Whatever.

### <a name="evangelism"></a>Help evangelize MALROT

The BIG one. Help us evangelize MALROT to cultural institutions and public authorities.

## <a name="status"></a>Project status

- **2022-05-01**  
  MALROT website and GitHub account are live and MALROT specification will be discussed with cultural institutions in the next coming months. Objective is a stable `1.0.0` version in S2 2022.

### Get MALROT updates delivered right to your inbox

<form action="https://tinyletter.com/malrot" method="post" target="popupwindow" onsubmit="window.open('https://tinyletter.com/malrot', 'popupwindow', 'scrollbars=yes,width=800,height=600');return true"><input type="text" name="email" id="tlemail" placeholder="Email" /><input type="hidden" value="1" name="embed"/><input type="submit" value="Subscribe" /></form>

## <a name="license"></a>License

Except as otherwise noted, content of MALROT GitHub repositories and MALROT files are licensed under the [CC BY SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/), code under the [MIT](https://github.com/malrot/www/blob/master/LICENSE.md).

MALROT is based on an idea from [Charles-Henri ARNOULD](https://github.com/charnould) — [info@malrot.org](mailto:info@malrot.org)
