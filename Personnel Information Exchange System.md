## Data Flow
```mermaid
sequenceDiagram
    Participant VBMS
    Participant PIES
    Participant NATIONAL ARCHIVES
   
    Participant BDN

    PIES ->> NATIONAL ARCHIVES: Interface(Service Records)
    NATIONAL ARCHIVES ->> PIES: Interface
    PIES  ->> VBMS:  Benfit information
    VBMS ->> PIES: Process Benefits
    BDN ->> PIES : Examinations (verify SSN)
    PIES ->> BDN   : Examinations 
