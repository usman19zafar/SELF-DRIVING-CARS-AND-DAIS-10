```mermaid
flowchart LR
    A[Sensors] --> B[Perception]
    B --> C[SIS‑10<br/>Semantic Interpretation]
    C --> D[SIF‑10<br/>Semantic Influence]
    D --> E[MCM‑10<br/>Meaning Classification]
    E --> F[TIER‑10<br/>Tier Assignment]
    F --> G[SICM‑10<br/>Semantic Intensity Scoring]
    G --> H[DIFS‑10<br/>Drift & Fading]
    H --> I[QFIM‑10<br/>Qualified Interpretation]
    I --> J[Fusion<br/>(Cross‑Sensor Meaning)]
    J --> K[Planning<br/>(Task + Motion)]
    K --> L[Control<br/>(Execution Layer)]
    L --> M[AMD‑10<br/>Meaning Diagnostics]
```
