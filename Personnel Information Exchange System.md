## Data Flow
```mermaid
sequenceDiagram
    Participant VBMS
    Participant PIES
    Participant Tuxedo
    Participant BDN

    VBMS ->> PIES:  Benfit information
    PIES -->> VBMS: Process Benefits
    Tuxedo ->> PIES: Develop Claim
    PIES->> Tuxedo : retrieves information
    BDN->> PIES : Examinations 
    PIES -->> BDN   : Examinations 
