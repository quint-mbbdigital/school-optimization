graph TD
    A[User Logs In] --> B[View Main Dashboard]
    B --> C{Choose Action}
    C --> D[Explore Performance Timeline]
    C --> E[Compare Schools]
    C --> F[Analyze Resource Allocation]
    C --> G[View Predictive Insights]

    D --> H[Select Time Period]
    H --> I[View Performance Trends]
    I --> J[Explore Significant Events]
    J --> K[Analyze Event Impact]

    E --> L[Select Schools to Compare]
    L --> M[View Comparison Metrics]
    M --> N[Analyze Differences]

    F --> O[View Current Allocation]
    O --> P[Simulate Reallocation]
    P --> Q[Review Projected Impact]

    G --> R[Select Metrics for Prediction]
    R --> S[View Future Projections]
    S --> T[Explore 'What-If' Scenarios]

    K --> U[Make Data-Driven Decision]
    N --> U
    Q --> U
    T --> U

    U --> V[Implement Changes]
    V --> W[Monitor Results]
    W --> B