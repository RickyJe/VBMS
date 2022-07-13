## Data Flow
```mermaid
sequenceDiagram
    Participant VBMS
    Participant PCGL
    PCGL ->> VBMS :  Retrieve data for letter
    VBMS -->> PCGL : Get data for letters
```
