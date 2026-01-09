---
layout: with_mermaid
title: "Cyber Security Landscape"
author: "Stratoclo"
---
### Cyber Security Landscape
<div class="mermaid">
graph LR

  %% Styles
  classDef note fill:#FFF3B0,stroke:#D4A72C,stroke-width:1px,color:#111,font-size:10px;
  classDef cloudPanel fill:#F7FAFF,stroke:#C7D2E8,stroke-width:1px;

  subgraph client
      PC[PC win/mac]
      N_PC["Security monitoring"]
      N_PC -.->  PC 
      class N_PC note
      MO[Mobile]
      N_MO["Security monitoring"]
      N_MO -.-> MO
      class N_MO note      
  end

  subgraph "cloud-aws"
    subgraph firewall
      FW[Firewall]
      N_FW["Security monitoring"]
      N_FW -.-> FW
      class N_FW note      
    end

    subgraph VPC
      WS[Webserver]
      N_WS["Security monitoring"]
      N_WS -.-> WS
      class N_WS note

      AS[Application Server]
      N_AS["Security monitoring"]
      N_AS -.-> AS
      class N_AS note

      DB[(DataBase Postgres)]
      N_DB["Security monitoring"]
      N_DB -.-> DB
      class N_DB note
    end
  end

  subgraph "Azure AD"
    IAM[Identity Access Management]
    N_IAM["Monitoring / sign-in logs"]
    N_IAM -.-> IAM
    class N_IAM note
  end

  %% Apply panel tint
  class cloudPanel cloud-aws

  %% Traffic path
  client -.-> FW
  FW -.-> WS
  WS --> AS
  AS --> DB

  %% Auth path
  client -.-> IAM
  AS -.-> IAM

</div>
