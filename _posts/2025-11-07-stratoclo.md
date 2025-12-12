---
layout: with_mermaid
title: "Stratoclo Architecture"
author: "Stratoclo"
---


<div class="mermaid">

flowchart LR

  %% ========= Telemetry Sources =========
  subgraph S[Raw telemetry sources]
    IAM[IAM logs]
    NET[Network logs]
    CLOUD[Cloud logs]
    EDR[EDR logs]
  end

  %% ========= Platforms =========
  subgraph SIEM[SIEM]
    S1[Normalize and enrich logs]
    ST[(Storage)]    
    S2[Correlation alerts]
    S3[SIEM incidents]
  end

  subgraph XDR[XDR]
    X1[Cross domain detections]
    X2[Behavior analytics]
    X3[Attack path and causality]
  end

  subgraph SOAR[SOAR and XSOAR]
    R1[Incidents and cases]
    R2[Playbook runs]
    R3[Analyst notes and actions]
    R4[Threat intel artifacts]
  end

  %% ========= Stratoclo Core =========
  subgraph STRATO[Stratoclo]
    A1[Ingestion and normalization]
    A2[Agent reasoning engine]
    A3[Dedup and correlation across tools]
    A4[Risk scoring and prioritization]
    A5[Explainable summaries for analysts]
  end

  %% ========= Output =========
  SOC[MSSP SOC analysts]
  TICKETS[Ticketing and ITSM]
  ACTIONS[Response actions in customer tools]

  %% ========= Edges from raw logs =========
  IAM --> S
  NET --> S
  CLOUD --> S
  EDR --> S

  S --> S1
  S1 --> ST
  S1 --> S2
  S2 --> S3

  %% Raw logs also feed XDR directly
  S --> XDR

  %% SIEM and XDR into SOAR
  S3 --> SOAR
  XDR --> SOAR

  %% All platform outputs into Stratoclo
  S3 --> A1
  X1 --> A1
  X2 --> A1
  X3 --> A1
  R1 --> A1
  R2 --> A1
  R3 --> A1
  R4 --> A1

  %% Internal Stratoclo flow
  A1 --> A2
  A2 --> A3
  A3 --> A4
  A4 --> A5

  %% Stratoclo outputs
  A5 --> SOC
  A4 --> TICKETS
  A4 --> ACTIONS
</div>