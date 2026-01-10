---
layout: with_mermaid
title: "Cyber Security Components"
author: "Stratoclo"
---
### Cyber Security Landscape

<div class="mermaid">
graph LR

  %% Styles
  classDef note fill:#FFF3B0,stroke:#D4A72C,stroke-width:1px,color:#111,font-size:10px;
  classDef cloudPanel fill:#F7FAFF,stroke:#C7D2E8,stroke-width:1px;

  %% CLIENT
  subgraph client["client"]
      PC[PC win/mac]
      MO[Mobile]

      N_PC["Security monitoring"] -.-> PC
      N_MO["Security monitoring"] -.-> MO

      class N_PC note
      class N_MO note
  end

  %% AWS
  subgraph cloudAws["cloud-aws"]
    subgraph firewall["firewall"]
      FW[Firewall]
      N_FW["Security monitoring"] -.-> FW
      class N_FW note
    end

    subgraph vpc["VPC"]
      WS[Webserver]
      AS[Application Server]
      DB[(DataBase Postgres)]

      N_WS["Security monitoring"] -.-> WS
      N_AS["Security monitoring"] -.-> AS
      N_DB["Security monitoring"] -.-> DB

      class N_WS note
      class N_AS note
      class N_DB note
    end
  end

  %% AZURE AD
  subgraph azureAd["Azure AD"]
    IAM[Identity Access Management]
    N_IAM["Monitoring / sign-in logs"] -.-> IAM
    class N_IAM note
  end

  %% Apply panel tint (works because cloudAws is a real ID)
  class cloudAws cloudPanel

  %% Traffic path (connect from actual nodes)
  PC -.-> FW
  MO -.-> FW
  FW -.-> WS
  WS --> AS
  AS --> DB

  %% Auth path (connect from actual nodes)
  PC -.-> IAM
  MO -.-> IAM
  AS -.-> IAM

</div>
