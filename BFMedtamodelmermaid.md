```mermaid
flowchart TD

%% --- Core Meta Model ---

StreamOverview["Stream overview"]

StreamOverview --> FunctionalGroups["Functional process groups"]
StreamOverview --> ScenarioClusters["E2E scenario clusters"]

FunctionalGroups --> BusinessProcesses["Business Processes "]
ScenarioClusters --> E2E_Scenarios["E2E scenarios"]

BusinessProcesses --> BusinessRoles["Business Roles"]
E2E_Scenarios --> BusinessRoles

BusinessRoles --> TrainingDocs["Training needs / Training documents"]
BusinessRoles --> RoleMapping["Role mapping and system access"]

TrainingDocs --> TestDocuments["Test documents"]
E2E_Scenarios --> E2E_TestCases["E2E test cases"]

BusinessProcesses --> ChangeImpacts["Change impacts"]
ChangeImpacts --> BusinessRoles

BusinessProcesses --> SystemImpacts["System impacts"]
SystemImpacts --> BusinessRoles

BusinessRoles --> AuthorizationConcept["Authorization concept"]

%% --- GxP / CSV Extensions ---

BusinessProcesses --> CSV_Requirements["CSV Requirements"]
BusinessRoles --> URS["URS - User Requirement Specifications"]

E2E_Scenarios --> FRA["Functional Risk Assessments (FRA)"]

FRA --> TestProtocols["Validation Test Protocols (IQ / OQ / PQ)"]
TestProtocols --> Deviations["Deviation Reports"]
Deviations --> ValidationSummary["Validation Summary Report (VSR)"]

%% Add forward flow for readability
ValidationSummary --> FinalCompliance["Compliance Evidence Package"]
