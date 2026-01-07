```text
+----------------------------------------+-------------+-------------------------------+-------------+
|                Dimension               | ISO 26262   |            SOTIF              |   DAIS‑10   |
+----------------------------------------+-------------+-------------------------------+-------------+
| Focus                                  | Functional  | Safety of Intended            | Semantic    |
|                                        | Safety      | Functionality                 | Safety      |
+----------------------------------------+-------------+-------------------------------+-------------+
| Governs meaning                        | No          | No                            | Yes         |
+----------------------------------------+-------------+-------------------------------+-------------+
| Governs drift                          | No          | Partial                       | Yes         |
+----------------------------------------+-------------+-------------------------------+-------------+
| Governs semantic lifecycle             | No          | No                            | Yes         |
+----------------------------------------+-------------+-------------------------------+-------------+
| Handles occlusion meaning              | No          | Partial                       | Yes         |
+----------------------------------------+-------------+-------------------------------+-------------+
| Handles cross‑model contradictions     | No          | No                            | Yes         |
+----------------------------------------+-------------+-------------------------------+-------------+
| Provides semantic scoring              | No          | No                            | Yes         |
+----------------------------------------+-------------+-------------------------------+-------------+
| Provides tiering                       | No          | No                            | Yes         |
+----------------------------------------+-------------+-------------------------------+-------------+
| Provides fading logic                  | No          | No                            | Yes         |
+----------------------------------------+-------------+-------------------------------+-------------+
| Provides semantic diagnostics          | No          | No                            | Yes         |
+----------------------------------------+-------------+-------------------------------+-------------+
| Handles SSCEs                          | No          | No                            | Yes         |
+----------------------------------------+-------------+-------------------------------+-------------+
| Complements AV stack                   | Yes         | Yes                           | Yes         |
+----------------------------------------+-------------+-------------------------------+-------------+
```

```mermaid
flowchart LR

    A[ISO 26262<br/>Functional Safety] --> D[Complete AV Safety Stack]
    B[SOTIF<br/>Safety of Intended Functionality] --> D
    C[DAIS‑10<br/>Semantic Safety] --> D

    subgraph A1[ISO 26262 Capabilities]
        A2[No meaning governance]
        A3[No drift governance]
        A4[No semantic lifecycle]
        A5[No occlusion meaning]
        A6[No semantic diagnostics]
    end

    subgraph B1[SOTIF Capabilities]
        B2[No meaning governance]
        B3[Partial drift handling]
        B4[No semantic lifecycle]
        B5[Partial occlusion handling]
        B6[No semantic diagnostics]
    end

    subgraph C1[DAIS‑10 Capabilities]
        C2[Governs meaning]
        C3[Governs drift]
        C4[Governs semantic lifecycle]
        C5[Handles occlusion meaning]
        C6[Resolves cross‑model contradictions]
        C7[Semantic scoring]
        C8[Tiering]
        C9[Fading logic]
        C10[Semantic diagnostics]
        C11[Handles SSCEs]
    end
```
