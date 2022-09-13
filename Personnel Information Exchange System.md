## Data Flow
```mermaid
sequenceDiagram
    Participant PIES
    Participant NATIONAL ARCHIVES
    Participant VBMS
    Participant Tuxedo
    Participant BDN

    PIES ->> NATIONAL ARCHIVES: Interface
    PIES  ->> VBMS:  Benfit information
    VBMS -->> PIES: Process Benefits
    Tuxedo ->> PIES: Develop Claim
    PIES->> Tuxedo : retrieves information
    BDN->> PIES : Examinations 
    PIES -->> BDN   : Examinations 
