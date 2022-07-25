## Data Flow
```mermaid
sequenceDiagram
    Participant VBMS
    Participant Caseflow
    Participant BGS
    Participant VACOLS
    Participant VVA
    VBMS ->> Caseflow: ClaimService(V5, API) 
    Caseflow -->> VBMS: eFolderUploadService API
    BGS ->> Caseflow: DocumentList
    VACOLS->> Caseflow : Verans Appeals Control and Locator System(cases before 2019)
    VVA->> Caseflow : Legacy content management (Virtual VA)
    Caseflow -->> Notification   : Sends email and text messages

```
