---
layout: with_mermaid
title: "Cyber Security Landscape"
author: "Stratoclo"
---


<div class="mermaid">
architecture-beta
    group api(cloud)[API]

    service db(database)[Database] in api
    service disk1(disk)[Storage] in api
    service disk2(disk)[Storage] in api
    service server(server)[Server] in api

    db:L -- R:server
    disk1:T -- B:server
    disk2:T -- B:db
</div>

<div class="mermaid">
architecture-beta
    group api(logos:aws-lambda)[API]

    service db(logos:aws-aurora)[Database] in api
    service disk1(logos:aws-glacier)[Storage] in api
    service disk2(logos:aws-s3)[Storage] in api
    service server(logos:aws-ec2)[Server] in api

    db:L -- R:server
    disk1:T -- B:server
    disk2:T -- B:db
</div>

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

