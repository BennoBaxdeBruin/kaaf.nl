<script setup>
import { TriangleAlert, CloudOff, Unplug } from 'lucide-vue-next'

const whatsappLink = 'https://wa.me/+31628227646'
</script>

<template>
  <!-- Navigation -->
  <nav class="nav">
    <span class="nav-logo">KAAF</span>
    <a :href="whatsappLink" target="_blank" class="nav-cta">Get in Touch</a>
  </nav>

  <!-- Hero -->
  <section class="hero">
    <div class="hero-content">
      <span class="hero-badge">KAAF · MISSION-CRITICAL IT/OT INTEGRATION</span>
      <h1>Seamless IT/OT Integration<br>for Mission-Critical Operations.</h1>
      <p class="hero-sub">We modernize your digital infrastructure and migrate complex data interfaces without ever risking your operational continuity.</p>
      <a :href="whatsappLink" target="_blank" class="btn-primary">Get in Touch</a>
    </div>
    <div class="hero-image">
      <img src="/robvanroessel.jpg" alt="Rob van Roessel" />
    </div>
  </section>

  <!-- Problem -->
  <section class="problem">
    <div class="problem-header">
      <h2>Don't let digital transformation become an operational disaster.</h2>
      <p>In mission-critical environments, a single failed interface can halt a supply chain, delay a flight, or stop a train.</p>
    </div>
    <div class="problem-cards">
      <div class="problem-card">
        <TriangleAlert :size="24" />
        <h3>End-of-Life Risks</h3>
        <p>Legacy systems that threaten stability and leave your operations exposed to unexpected failures.</p>
      </div>
      <div class="problem-card">
        <CloudOff :size="24" />
        <h3>Migration Anxiety</h3>
        <p>Fear of downtime during complex cloud or platform shifts that could cripple your business.</p>
      </div>
      <div class="problem-card">
        <Unplug :size="24" />
        <h3>Technical Silos</h3>
        <p>A gap between core IT and the operational technology (OT) that actually runs your business.</p>
      </div>
    </div>
  </section>

  <!-- Guide -->
  <section class="guide">
    <div class="guide-header">
      <span class="guide-badge">THE GUIDE</span>
      <h2>Expertise forged in high-pressure environments.</h2>
      <p>At KAAF, we approach ICT from a business-process perspective. We don't just manage code; we manage the heartbeat of your operation. With over 20 years of experience in aviation, utilities, and logistics, we specialize in environments where operational impact is not an option.</p>
    </div>
    <div class="track-record">
      <div class="track-card">
        <img src="/schiphol_logo.png" alt="Schiphol Group" class="track-logo track-logo--schiphol" />
        <span class="track-label">Aviation</span>
        <h3>Schiphol Group</h3>
        <p>Migrated 400+ critical interfaces for the Airport Service Bus with zero operational disruption.</p>
      </div>
      <div class="track-card">
        <img src="/postnl_logo.svg" alt="PostNL" class="track-logo" />
        <span class="track-label">Logistics</span>
        <h3>PostNL</h3>
        <p>Led the digital transformation of the integration platform for all logistics processes to the cloud.</p>
      </div>
      <div class="track-card">
        <img src="/prorail_logo.svg" alt="ProRail" class="track-logo" />
        <span class="track-label">Rail</span>
        <h3>ProRail</h3>
        <p>Implemented the integration backbone for critical train control systems and positioning.</p>
      </div>
      <div class="track-card">
        <img src="/vodafone_logo.png" alt="Vodafone" class="track-logo" />
        <span class="track-label">Telecom</span>
        <h3>Vodafone</h3>
        <p>Managed 5G modernization and site installation across eight regions in Germany.</p>
      </div>
    </div>
  </section>

  <!-- Plan -->
  <section class="plan">
    <h2>Your Roadmap to a Future-Proof Operation</h2>
    <div class="plan-steps">
      <div class="plan-step">
        <div class="step-number">1</div>
        <h3>Strategic Assessment</h3>
        <p>We identify your risks and map your critical data dependencies across all systems.</p>
      </div>
      <div class="plan-step">
        <div class="step-number">2</div>
        <h3>Controlled Migration</h3>
        <p>Our team designs and builds your new platform using Agile (SAFe) methodologies at every step.</p>
      </div>
      <div class="plan-step">
        <div class="step-number">3</div>
        <h3>Sustainable Continuity</h3>
        <p>We deliver a modernized, stable environment that empowers your business to grow without technical debt.</p>
      </div>
    </div>
  </section>

  <!-- Transformation -->
  <section class="transformation">
    <div class="transformation-image"></div>
    <div class="transformation-text">
      <h2>From technical fires to operational harmony.</h2>
      <p>Imagine a digital ecosystem where your IT and OT systems work in perfect harmony. No more emergency rooms for failed deployments or fear of legacy system collapses. Whether it's connecting baggage drop-off points at an airport or algorithmic train positioning, KAAF provides the decisive, values-driven leadership needed to align complex stakeholders and technology.</p>
      <p class="highlight">Stop managing technical fires and start leading a resilient, data-driven organization.</p>
    </div>
  </section>

  <!-- Final CTA -->
  <section class="final-cta">
    <h2>Ready to secure your operational future?</h2>
    <p>Let's discuss how KAAF can modernize your infrastructure without risking what matters most.</p>
    <a :href="whatsappLink" target="_blank" class="btn-primary-dark">Get in Touch</a>
  </section>
</template>
