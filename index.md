---
layout: default
title: "Stratoclo"
permalink: /
---

<style>
  .ai-hero {
    background: radial-gradient(circle at 15% 20%, rgba(58, 125, 243, 0.4), transparent 60%), radial-gradient(circle at 80% 0%, rgba(66, 221, 195, 0.45), transparent 55%), linear-gradient(135deg, #060a1b, #101b3a 55%, #122345);
    border: 1px solid rgba(255, 255, 255, 0.08);
    border-radius: 32px;
    color: #f7fbff;
  }

  .ai-hero .badge {
    background: rgba(255, 255, 255, 0.08);
    border: 1px solid rgba(255, 255, 255, 0.15);
    color: #c8d7ff;
    font-weight: 500;
    letter-spacing: 0.08em;
    text-transform: uppercase;
  }

  .ai-hero .btn-primary {
    background: linear-gradient(120deg, #5b7cfd, #49f0c6);
    border: none;
    box-shadow: 0 10px 40px rgba(72, 184, 255, 0.25);
  }

  .ai-hero .btn-outline-light {
    border-color: rgba(255, 255, 255, 0.4);
    color: #fff;
  }

  .ai-capabilities-grid {
    --bs-gutter-x: 2.5rem;
    --bs-gutter-y: 2.5rem;
  }

  .ai-feature-card {
    border-radius: 24px;
    border: 1px solid rgba(255, 255, 255, 0.07);
    background: rgba(3, 7, 23, 0.9);
    box-shadow: 0 15px 45px rgba(5, 9, 26, 0.4);
    color: #e7ecff;
    height: 100%;
    margin-bottom: 1.5rem;
  }

  .ai-feature-card img {
    border-radius: 16px;
    border: 1px solid rgba(255, 255, 255, 0.1);
  }

  .ai-feature-card[data-accent="cyan"] {
    background: linear-gradient(140deg, rgba(16, 53, 105, 0.9), rgba(22, 112, 138, 0.9));
  }

  .ai-feature-card[data-accent="violet"] {
    background: linear-gradient(140deg, rgba(30, 21, 56, 0.95), rgba(79, 54, 170, 0.85));
  }

  .ai-feature-card[data-accent="amber"] {
    background: linear-gradient(140deg, rgba(54, 36, 7, 0.95), rgba(160, 111, 10, 0.8));
  }

  .ai-feature-card[data-accent="mint"] {
    background: linear-gradient(140deg, rgba(11, 39, 35, 0.95), rgba(24, 109, 93, 0.85));
  }

  .ai-feature-card[data-accent="blue"] {
    background: linear-gradient(140deg, rgba(12, 35, 71, 0.95), rgba(20, 60, 135, 0.85));
  }

  .ai-feature-card[data-accent="rose"] {
    background: linear-gradient(140deg, rgba(52, 5, 21, 0.95), rgba(142, 37, 74, 0.85));
  }

  .ai-section-title {
    max-width: 680px;
  }

  .ai-section-title span {
    color: #5fe6ff;
    letter-spacing: 0.08em;
  }

  .ai-stats-card {
    background: rgba(3, 8, 28, 0.6);
    border: 1px solid rgba(255, 255, 255, 0.08);
    border-radius: 20px;
    color: #dfe8ff;
  }

  .ai-stats-card strong {
    font-size: 2rem;
  }

  .ai-surface {
    background: #050a1f;
    border-radius: 28px;
    border: 1px solid rgba(20, 32, 73, 0.6);
  }

  .ai-post-card {
    border-radius: 18px;
    border: 1px solid rgba(20, 32, 73, 0.8);
    box-shadow: none;
    margin-bottom: 1.5rem;
  }
</style>

<div class="py-5">
  <div class="ai-hero p-4 p-md-5 mb-5 shadow-lg">
    <div class="row align-items-center g-5">
      <div class="col-lg-7">
        <span class="badge rounded-pill px-3 py-2 mb-3">Enterprise AI Security</span>
        <h1 class="display-5 mb-3">AgentSOC — the professional AI Tier‑1 SOC analyst for modern teams</h1>
        <p class="lead mb-4">AgentSOC triages every alert, correlates across telemetry, and pushes remediation to the SecOps stack without leaving your workflow.</p>
        <div class="d-flex flex-column flex-sm-row gap-3">
          <a class="btn btn-primary btn-lg px-4" href="mailto:founder@stratoclo.com">Book a demo</a>
          <a class="btn btn-outline-light btn-lg px-4" href="/tech_notes">See the platform</a>
        </div>
      </div>
      <div class="col-lg-5 text-center">
        <div class="bg-dark bg-opacity-25 rounded-4 p-4 p-md-5 h-100 d-flex flex-column justify-content-center">
          <img src="/assets/images/intro.svg" alt="Incident workflow illustration" class="img-fluid mb-3" style="max-height:280px;">
          <p class="text-uppercase small text-white-50 mb-0">Signal → Evidence → Action</p>
        </div>
      </div>
    </div>
    <div class="row row-cols-1 row-cols-md-3 g-4 mt-4">
      <div class="col">
        <div class="ai-stats-card p-4 h-100">
          <strong>12 min</strong>
          <p class="mb-0 text-white-50">Average time from alert to containment</p>
        </div>
      </div>
      <div class="col">
        <div class="ai-stats-card p-4 h-100">
          <strong>40+</strong>
          <p class="mb-0 text-white-50">Native SIEM, SOAR, and ticketing integrations</p>
        </div>
      </div>
      <div class="col">
        <div class="ai-stats-card p-4 h-100">
          <strong>99.2%</strong>
          <p class="mb-0 text-white-50">Actions performed under human-approved guardrails</p>
        </div>
      </div>
    </div>
  </div>

  <div class="py-4 py-md-5">
    <div class="ai-section-title mb-5">
      <p class="text-uppercase small mb-2"><span>Capabilities</span></p>
      <h2 class="h1 mb-3">Purpose-built workflows for AI-driven SecOps</h2>
      <p class="text-muted">Each capability pairs deterministic playbooks with autonomous AI agents so analysts can operate faster without sacrificing trust.</p>
    </div>
    <div class="row g-4 ai-capabilities-grid">
      <div class="col-md-6 col-lg-4">
        <div class="ai-feature-card p-4" data-accent="cyan">
          <div class="d-flex align-items-center mb-3">
            <img src="/assets/images/1.jpg" alt="SIEM sources" style="width:68px;height:68px;object-fit:cover;">
            <div class="ms-3">
              <p class="text-uppercase small mb-1 text-white-50">Ingest</p>
              <h5 class="mb-0">Connect every telemetry stream</h5>
            </div>
          </div>
          <p>Pull alerts from Splunk, Sentinel, Cortex XDR, Cisco XDR, or any SIEM/XDR via webhook, API, or secure forwarder.</p>
        </div>
      </div>
      <div class="col-md-6 col-lg-4">
        <div class="ai-feature-card p-4" data-accent="blue">
          <div class="d-flex align-items-center mb-3">
            <img src="/assets/images/2.jpg" alt="AI investigations" style="width:68px;height:68px;object-fit:cover;">
            <div class="ms-3">
              <p class="text-uppercase small mb-1 text-white-50">Investigate</p>
              <h5 class="mb-0">Autonomous case building</h5>
            </div>
          </div>
          <p>Multiple AI agents enrich context, trace lateral movement, and correlate user, device, and IP behavior in real time.</p>
        </div>
      </div>
      <div class="col-md-6 col-lg-4">
        <div class="ai-feature-card p-4" data-accent="violet">
          <div class="d-flex align-items-center mb-3">
            <img src="/assets/images/3.jpg" alt="ATT&CK mapping" style="width:68px;height:68px;object-fit:cover;">
            <div class="ms-3">
              <p class="text-uppercase small mb-1 text-white-50">Reason</p>
              <h5 class="mb-0">MITRE ATT&CK narratives</h5>
            </div>
          </div>
          <p>Automatically map signals to ATT&CK techniques, calculate severity, and build an explainable timeline ready for audit.</p>
        </div>
      </div>
      <div class="col-md-6 col-lg-4">
        <div class="ai-feature-card p-4" data-accent="mint">
          <div class="d-flex align-items-center mb-3">
            <img src="/assets/images/4.jpg" alt="Remediation steps" style="width:68px;height:68px;object-fit:cover;">
            <div class="ms-3">
              <p class="text-uppercase small mb-1 text-white-50">Act</p>
              <h5 class="mb-0">Actionable remediation</h5>
            </div>
          </div>
          <p>Recommend or execute: block IPs, isolate endpoints, disable accounts, update firewalls, and open SOC tickets.</p>
        </div>
      </div>
      <div class="col-md-6 col-lg-4">
        <div class="ai-feature-card p-4" data-accent="amber">
          <div class="d-flex align-items-center mb-3">
            <img src="/assets/images/5.jpg" alt="Reporting" style="width:68px;height:68px;object-fit:cover;">
            <div class="ms-3">
              <p class="text-uppercase small mb-1 text-white-50">Report</p>
              <h5 class="mb-0">Executive-grade outputs</h5>
            </div>
          </div>
          <p>Produce ready-to-ship reports for PDF, Slack, Email, Jira, or ServiceNow with linked evidence and rationale.</p>
        </div>
      </div>
      <div class="col-md-6 col-lg-4">
        <div class="ai-feature-card p-4" data-accent="rose">
          <div class="d-flex align-items-center mb-3">
            <img src="/assets/images/6.jpg" alt="Human approvals" style="width:68px;height:68px;object-fit:cover;">
            <div class="ms-3">
              <p class="text-uppercase small mb-1 text-white-50">Assure</p>
              <h5 class="mb-0">Human-in-the-loop controls</h5>
            </div>
          </div>
          <p>Operate with approvals or auto-mode. Every action is justified, logged, and ready for compliance review.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="py-5">
  <div class="ai-surface p-4 p-md-5">
    <div class="d-flex flex-column flex-md-row justify-content-between align-items-start align-items-md-center mb-4">
      <div>
        <p class="text-uppercase text-secondary small mb-2">Insights</p>
        <h2 class="mb-0 text-white">Latest from the Stratoclo team</h2>
      </div>
      <a class="btn btn-outline-light btn-sm mt-3 mt-md-0" href="/blog/">View all</a>
    </div>
    <div class="row g-4">
      {% assign recent_posts = site.posts | slice: 0, 4 %}
      {% for post in recent_posts %}
      <div class="col-md-6 col-lg-3">
        <div class="card ai-post-card h-100 bg-transparent">
          <div class="card-body py-4">
            <p class="text-uppercase text-secondary small mb-2">{{ post.date | date: "%b %d, %Y" }}</p>
            <h5 class="card-title"><a class="text-light" href="{{ post.url }}">{{ post.title }}</a></h5>
            <p class="card-text text-secondary">{{ post.excerpt | strip_html | truncate: 110 }}</p>
            <a class="text-primary small" href="{{ post.url }}">Read more →</a>
          </div>
        </div>
      </div>
      {% endfor %}
    </div>
  </div>
</div>
