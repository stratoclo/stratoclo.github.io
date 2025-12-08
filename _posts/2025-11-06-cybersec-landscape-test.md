---
layout: with_mermaid
title: "Cyber security landscape test"
author: "Stratoclo"
---


<div class="mermaid">
graph LR

  subgraph client
    subgraph pc
    BR[Browser]
    end
    subgraph mobile
    MO[Mobile]
    end
  end

  subgraph cloud
    subgraph firewall
    FW[Firewall]
    end
    subgraph VPC
    WS[Webserver]
    end
    subgraph cloud_services
    IAM[Identity Access Management]
    end    
  end

  client -.-> firewall
  FW -.-> WS
  client -.-> IAM
  
</div>

