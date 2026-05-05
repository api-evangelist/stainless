---
title: "Introducing the (experimental!) Stainless SQL SDK generator"
url: "https://www.stainless.com/blog/introducing-stainless-sql-sdk-generator-from-openapi"
date: "Wed, 18 Feb 2026 00:00:00 GMT"
author: ""
feed_url: "https://www.stainless.com/blog/rss.xml"
---
Introducing our experimental SQL SDK generator, a new way to query REST APIs directly from PostgreSQL using standard SQL. By transforming an OpenAPI spec into a typed PostgreSQL extension, every API endpoint becomes a SQL function and every response becomes a composite type, enabling type-safe queries without JSON parsing or ETL pipelines. Designed for analytics, reconciliation, and batch workflows, this approach lets you join live API data with your existing tables while preserving pagination control and planner optimizations.
