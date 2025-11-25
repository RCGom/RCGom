```mermaid
flowchart LR

%% PHASES
subgraph Envision [Envision]
E_BR[Business: Define business vision & TOM]
E_PR[Process: Define E2E process landscape]
E_SR[System: Assess technical landscape]
E_DR[Data: Define data migration strategy]
E_PM[PM: Define governance & scope]
E_CR[Compliance: Define regulatory scope]
end

subgraph Discover [Discover]
D_BR[Business: Mobilise teams & change plan]
D_PR[Process: Sandbox setup & config standards]
D_SR[System: Sandbox landscape setup]
D_DR[Data: Profile legacy data]
D_PM[PM: Establish PMO & roadmap]
D_CR[Compliance: Validation impact assessment]
end

subgraph Prepare [Prepare]
P_BR[Business: Fit-to-Standard workshops]
P_PR[Process: Fit-to-Standard outputs]
P_SR[System: Define config backlog]
P_DR[Data: Mapping & initial load design]
P_PM[PM: Detailed project plan & RAID]
P_CR[Compliance: Validation Master Plan]
end

subgraph Explore [Explore]
X_BR[Business: Training & UAT readiness]
X_PR[Process: Build scenarios & test design]
X_SR[System: Integration builds & tests]
X_DR[Data: Trial migration & validation]
X_PM[PM: Cross-stream integration mgmt]
X_CR[Compliance: URS + Functional Risk Assessment]
end

subgraph Realize [Realize]
R_BR[Business: Cutover planning]
R_PR[Process: Process documentation updates]
R_SR[System: Final deployment prep]
R_DR[Data: Final migration execution]
R_PM[PM: Quality gates & readiness checks]
R_CR[Compliance: IQ/OQ/PQ execution]
end

subgraph Deploy [Deploy]
DP_BR[Business: Business value review]
DP_PR[Process: Continuous improvement]
DP_SR[System: Operate & monitor]
DP_DR[Data: Data quality governance]
DP_PM[PM: Go-live & hypercare]
DP_CR[Compliance: Validation Summary Report]
end

%% (No arrows needed; it's a structured matrix)
