## Data Flow
```mermaid
sequenceDiagram
    Participant VBMS
    Participant PIES
    Participant NATIONAL ARCHIVES
   
    Participant BDN

    PIES ->> NATIONAL ARCHIVES: Interface(Service Records)
    NATIONAL ARCHIVES ->> PIES: Interface
    PIES  ->> VBMS:  Benfits Information
    VBMS ->> PIES: Process Benefits
    PIES ->> BDN : Examinations (verify SSN)
    BDN ->> PIES   : Examinations 
