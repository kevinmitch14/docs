---
label: What is Baselime?
order: 2
---

[Baselime](https://baselime.io) is an observability solution built for modern cloud-native environments. It combines logs, metrics, and distributed traces to give you full visibility across your microservices at scale.

![Baselime Console](./assets/images/illustrations/diagrams.png)


---

## How is Baselime different?

Baselime is fundamentally different from most other observability and monitoring providers in 4 key aspects:

### High cardinality and dimentionality

Cardinality and dimentionality are best described using examples. Imagine you log an HTTP request that makes database calls.

- High cardinality means that in your logs, you can have a unique `userId` or `requestId` (which can take over a million distinct values). Those are high cardinality fields. Baselime enables you to query against any specific value of a high cardinality field so that you can narrow down your search to a specific user or request.

- High dimensionality means that in your logs, you can have thousands of possible fields. You can record each HTTP header of your request and the details of each database call. Any log can be a key-value object with thousands of individual keys. Baselime indexes every single one of the keys and enables you to query against every one of them.

From day 0, everything is queriable and searchable, and correlation between data sources is possible. Baselime does not perform any pre-aggregation of data before ingestion; this means you can run arbitrary queries on your telemetry data, and get answers about the state of your application.

### Query speed

Baselime is built on top of ClickHouse, the fastest analytics database in the world. When debugging real production outages, the ability to ask questions and get answers fast is most important.

### Real-time data ingestion

Baselime ingests data from your application in real-time. Telemetry data is available for you to query or for the real-time alerting within seconds of it being generated by your applications.

### Metadata annotations

Baselime automatically adds all the metadata necessary to contextualise your telemetry data: `hostname`, `hostID`, serverless function name, service name, cloud account and region, etc. All this data is automatically captured by Baselime. It enables you to efficiently identify patterns based on those parameters automatically.

Moreover, Baselime gives you control over the residency of your data. Either using our backend or a **Bring Your Own Backend** solution where all the data is stored on your cloud account.

---

## Why Baselime?

### Find and solve issues faster 
Troubleshoot infrastructure and application issues with high cardinality data and a fast query engine.

### Search anything, anywhere. It's all indexed
Query against any nested field and automatically surface anomalies fast; regardless of how unusual or unique this state of your application is.

### Take control of your data and costs
Use our backend or **Bring Your Own Backend**. Up to 6x more value than incumbents. No per-function pricing, no per-seat pricing, no per-alert pricing. Start at $0 and scale up as your applications grow, with no hidden fees.
