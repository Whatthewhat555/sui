```mermaid
flowchart TD
    A[Decision: Is the person 18 years old or older?] -->|Yes| B[Is the person medically fit?]
    A -->|No| X[Not eligible]
    B -->|Yes| C[Is the person a Singapore Citizen, PR, or Long Term Pass holder?]
    B -->|No| X
    C -->|Yes| D[Eligible to continue]
    C -->|No| X

    D --> E[Action: Register at Center]
    E --> F{Which Center?}
    F -->|ComfortDelGro| G[Action: Book the Test]
    F -->|Bukit Batok| G
    F -->|Singapore Safety Driving Center| G

    G --> H[Action: Study]
    H --> I[Action: Take Test]
    I --> J{Did you pass?}
    J -->|No| G
    J -->|Yes| K[Move on to Provisional Driving License (valid 2 years, needed for driving lessons)]

