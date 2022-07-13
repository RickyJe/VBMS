## Data Flow
```mermaid
sequenceDiagram
    Participant VBMS
    Participant PCGL
    Participant BDN
    Participant VETSNET
    PCGL ->> VBMS :  Retrieve data for letter
    VBMS -->> PCGL : Get data for letters
    PCGL ->> BDN :  Retrieve data for letter
    BDN -->> PCGL  : Get data for letters
    VETSNET ->> PCGL:  Retrieve data for letter
    PCGL -->> VETSNET : Get data for letters
```
