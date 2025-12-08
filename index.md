---
layout: default
title: "Stratoclo"
permalink: /
---

<style>
  .ai-hero {
    background: radial-gradient(circle at 12% 25%, rgba(162, 197, 255, 0.75), transparent 70%), radial-gradient(circle at 78% 5%, rgba(66, 221, 195, 0.45), transparent 55%), linear-gradient(135deg, #253f78, #0b1430 45%, #122345);
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

  .ai-hero .hero-cta {
    gap: 1.5rem;
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
    margin: -1.25rem;
  }

  .ai-capabilities-grid > [class*="col-"] {
    padding: 1.25rem;
  }

  .ai-feature-card {
    border-radius: 24px;
    border: 1px solid rgba(255, 255, 255, 0.07);
    background: rgba(6, 12, 32, 0.75);
    box-shadow: 0 20px 50px rgba(5, 9, 26, 0.35);
    color: #f5f7ff;
    height: 100%;
    margin-bottom: 1.5rem;
  }

  .ai-feature-card .feature-meta {
    gap: 1rem;
  }

  .feature-icon {
    width: 68px;
    height: 68px;
    border-radius: 18px;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-shrink: 0;
    box-shadow: 0 12px 28px rgba(10, 10, 10, 0.35);
    border: 1px solid rgba(255, 255, 255, 0.2);
  }

  .feature-icon svg {
    width: 34px;
    height: 34px;
  }

  .feature-icon[data-tone="cyan"] {
    background: linear-gradient(135deg, #2f6fff, #49f0c6);
    color: #e4fbff;
  }

  .feature-icon[data-tone="blue"] {
    background: linear-gradient(135deg, #2941c7, #1e7bf6);
    color: #dce5ff;
  }

  .feature-icon[data-tone="violet"] {
    background: linear-gradient(135deg, #5d1fb6, #9c3bff);
    color: #f4e7ff;
  }

  .feature-icon[data-tone="mint"] {
    background: linear-gradient(135deg, #0c6255, #24d1aa);
    color: #edfff9;
  }

  .feature-icon[data-tone="amber"] {
    background: linear-gradient(135deg, #7a4306, #ffb347);
    color: #fff8ee;
  }

  .feature-icon[data-tone="rose"] {
    background: linear-gradient(135deg, #6b1334, #ff5e8a);
    color: #ffeef5;
  }

  .ai-feature-card[data-accent="cyan"] {
    background: linear-gradient(140deg, rgba(40, 104, 206, 0.92), rgba(69, 212, 215, 0.9));
  }

  .ai-feature-card[data-accent="violet"] {
    background: linear-gradient(140deg, rgba(73, 51, 140, 0.94), rgba(151, 92, 219, 0.88));
  }

  .ai-feature-card[data-accent="amber"] {
    background: linear-gradient(140deg, rgba(143, 93, 18, 0.92), rgba(242, 177, 73, 0.88));
  }

  .ai-feature-card[data-accent="mint"] {
    background: linear-gradient(140deg, rgba(28, 92, 80, 0.92), rgba(62, 198, 166, 0.88));
  }

  .ai-feature-card[data-accent="blue"] {
    background: linear-gradient(140deg, rgba(34, 66, 158, 0.94), rgba(64, 134, 236, 0.88));
  }

  .ai-feature-card[data-accent="rose"] {
    background: linear-gradient(140deg, rgba(128, 34, 63, 0.94), rgba(219, 91, 132, 0.88));
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
        <div class="d-flex flex-column flex-sm-row hero-cta">
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
          <div class="d-flex align-items-center mb-3 feature-meta">
            <div class="feature-icon" data-tone="cyan">
              <svg viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
                <rect x="9" y="10" width="22" height="6" rx="3" stroke="currentColor" stroke-width="2"/>
                <path d="M20 16v12" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
                <path d="M15 22l5 5 5-5" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M12 30h16" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
                <path d="M10 34h20" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
              </svg>
            </div>
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
          <div class="d-flex align-items-center mb-3 feature-meta">
            <div class="feature-icon" data-tone="blue">
              <svg viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
                <circle cx="18" cy="18" r="8" stroke="currentColor" stroke-width="2"/>
                <path d="M24 24l6 6" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
                <path d="M18 12v-2" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
                <path d="M12 18h-2" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
                <path d="M18 24v2" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
                <path d="M24 18h2" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
              </svg>
            </div>
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
          <div class="d-flex align-items-center mb-3 feature-meta">
            <div class="feature-icon" data-tone="violet">
              <svg viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
                <rect x="10" y="10" width="8" height="8" rx="2" stroke="currentColor" stroke-width="2"/>
                <rect x="22" y="10" width="8" height="8" rx="2" stroke="currentColor" stroke-width="2"/>
                <rect x="10" y="22" width="8" height="8" rx="2" stroke="currentColor" stroke-width="2"/>
                <path d="M22 18v10a2 2 0 0 0 2 2h6" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
                <path d="M14 18v4a2 2 0 0 0 2 2h4" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
              </svg>
            </div>
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
          <div class="d-flex align-items-center mb-3 feature-meta">
            <div class="feature-icon" data-tone="mint">
              <svg viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M20 8l12 6v8c0 8-6 12-12 14-6-2-12-6-12-14v-8l12-6z" stroke="currentColor" stroke-width="2" stroke-linejoin="round"/>
                <path d="M14 21l4 4 8-8" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </div>
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
          <div class="d-flex align-items-center mb-3 feature-meta">
            <div class="feature-icon" data-tone="amber">
              <svg viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M14 8h12l6 6v18a2 2 0 0 1-2 2H14a2 2 0 0 1-2-2V10a2 2 0 0 1 2-2z" stroke="currentColor" stroke-width="2" stroke-linejoin="round"/>
                <path d="M26 8v6h6" stroke="currentColor" stroke-width="2" stroke-linejoin="round"/>
                <path d="M16 22h12" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
                <path d="M16 26h12" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
                <path d="M16 18h6" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
              </svg>
            </div>
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
          <div class="d-flex align-items-center mb-3 feature-meta">
            <div class="feature-icon" data-tone="rose">
              <svg viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
                <rect x="8" y="12" width="24" height="18" rx="3" stroke="currentColor" stroke-width="2"/>
                <path d="M12 16h8" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
                <path d="M12 22h6" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
                <path d="M22 24l4 4 6-8" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </div>
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
