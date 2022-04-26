```
mermaid
graph TD
    A[Docker Compose, Node JS] --> B(Docker Compose, Reverse Proxy)
    A --> C(Docker Compose, Mongo DB)
    B -.-> C
    I[Express, Node JS] -.Strongly Recommended.-> E[Typescript Basics] -->|Required| F[Typescript Integration]
    F -.-> A
    C --> G[Caching, Homegrown LRU]
    G --> H[Caching, Redis]
    C --> J[Mongo DB, Replica Sets]
    F -.-> J
    J --> K[Mongo DB, Sharding]
    B --> L[Event Driven Architecture, NodeJS + Typescript]
    L --> M[Event Driven Architecture, Redis]
    F --> N[Unit Testing using Jest]
    N --> O[Unit Testing, Mocking with Substitute]
    F --> L
```


  
