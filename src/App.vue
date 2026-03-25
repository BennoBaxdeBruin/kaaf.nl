<script setup>
import { ref } from 'vue'

const showAllExperience = ref(false)
const showAllAssignments = ref(false)
</script>

<template>
  <div class="header">
    <div class="header-top">
      <div class="header-info">
        <h1>Rob van Roessel</h1>
        <p class="subtitle">Project &amp; Program Manager, Digital Transformation</p>
        <p class="meta">Naarden, Netherlands &middot; Dutch (native), English (fluent)</p>
      </div>
      <img src="/robvanroessel.png" alt="Rob van Roessel" class="avatar" />
    </div>
    <div class="contact-links">
      <a href="mailto:rob.vanroessel@kaaf.nl" title="Email">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect width="20" height="16" x="2" y="4" rx="2"/><path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"/></svg>
      </a>
      <a href="tel:+31628227646" title="Phone">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"/></svg>
      </a>
      <a href="https://www.linkedin.com/in/robvanroessel/" target="_blank" title="LinkedIn">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect width="4" height="12" x="2" y="9"/><circle cx="4" cy="4" r="2"/></svg>
      </a>
    </div>
  </div>

  <div class="section">
    <h2>About</h2>
    <p>
      A driven, open and analytical professional who works in a structured and cooperative manner, based on trust, clarity and mutual respect. Approaches ICT primarily from a process and change perspective, with a solid foundation in core IT and deep expertise in supporting and mission-critical operational processes and systems.
    </p>
    <br>
    <p>
      Extensive experience in environments where ICT directly underpins operational continuity, safety and availability, particularly within supply-chain-driven domains in Utility, Retail, Consumer Goods, Banking and ICT Services. Significant international experience in process and organizational transformation, at the intersection of data, technology and interconnected ecosystems.
    </p>
  </div>

  <div class="section">
    <h2>Work Experience</h2>

    <div class="experience-item">
      <div class="experience-header">
        <h3>Independent</h3>
        <span class="period">2008 &ndash; present</span>
      </div>
      <div class="role">Project/Program Manager, Digital Transformation</div>
      <p>Independent consultant specializing in large-scale digital transformation programmes. Leading complex integration, migration and platform modernization projects for major organizations across the Netherlands and Europe.</p>
      <div class="tags">
        <span class="tag">Digital Transformation</span>
        <span class="tag">Integration</span>
        <span class="tag">Cloud Migration</span>
        <span class="tag">SAFe</span>
        <span class="tag">PRINCE2</span>
      </div>
    </div>

    <div class="experience-item">
      <div class="experience-header">
        <h3>Bakkenist</h3>
        <span class="period">2009 &ndash; 2017</span>
      </div>
      <div class="role">Managing Partner (2014&ndash;2017) &middot; Partner (2009&ndash;2013)</div>
      <p>Management consulting firm. Progressed from Partner to Managing Partner, leading strategic consulting engagements and growing the firm's revenue and client base.</p>
      <div class="tags">
        <span class="tag">Management Consulting</span>
        <span class="tag">Strategy</span>
        <span class="tag">Leadership</span>
      </div>
    </div>

    <div class="experience-item">
      <div class="experience-header">
        <h3>Arengo Advies en Management</h3>
        <span class="period">2008 &ndash; 2009</span>
      </div>
      <div class="role">Associate</div>
      <p>Advisory and management consultancy focused on organizational and ICT transformation.</p>
    </div>

    <template v-if="showAllExperience">
      <div class="experience-item">
        <div class="experience-header">
          <h3>Maxeda</h3>
          <span class="period">2003 &ndash; 2007</span>
        </div>
        <div class="role">Management Consultant / Project Manager / Architect</div>
        <p>Advised business units at CxO level on IT investment rationalization. Managed SAP application teams (~35 FTE) supporting retail back-office processes for HEMA, De Bijenkorf, V&amp;D and other brands.</p>
        <div class="tags">
          <span class="tag">SAP</span>
          <span class="tag">Retail</span>
          <span class="tag">IT Management</span>
        </div>
      </div>

      <div class="experience-item">
        <div class="experience-header">
          <h3>Deloitte Consulting Germany</h3>
          <span class="period">1996 &ndash; 2001</span>
        </div>
        <div class="role">Project Manager / Senior SAP Consultant</div>
        <p>SAP implementations across Europe for Bayer AG, Colgate Palmolive, SAP AG and SEB Group. Specialized in financial processes, controlling and profitability accounting across multi-country rollouts.</p>
        <div class="tags">
          <span class="tag">SAP FI/CO</span>
          <span class="tag">European Rollouts</span>
          <span class="tag">FMCG</span>
        </div>
      </div>
    </template>

    <button class="show-more" :class="{ expanded: showAllExperience }" @click="showAllExperience = !showAllExperience">
      {{ showAllExperience ? 'Show less' : 'Show 2 more' }}
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m6 9 6 6 6-6"/></svg>
    </button>
  </div>

  <div class="section">
    <h2>Key Assignments</h2>

    <div class="experience-item">
      <div class="experience-header">
        <h3>Schuberg Philis</h3>
        <span class="period">Oct 2024 &ndash; Mar 2025</span>
      </div>
      <div class="role">Project Manager</div>
      <p>Prepared a proposal for a Dutch pension administrator for the carve-out of a business unit from the existing ICT organization. Focused on migrating core applications to a new cloud platform, ensuring continuity, security and compliance.</p>
      <div class="tags">
        <span class="tag">Cloud Migration</span>
        <span class="tag">Carve-out</span>
        <span class="tag">Compliance</span>
      </div>
    </div>

    <div class="experience-item">
      <div class="experience-header">
        <h3>Schiphol Group</h3>
        <span class="period">Nov 2019 &ndash; Sep 2025</span>
      </div>
      <div class="role">Project Manager, Data Integration</div>
      <p>Part of Schiphol's End-of-Life strategic renewal programme. Led the replacement of the Airport Service Bus integration platform and the migration of ~400 internal and external integrations across all business units.</p>
      <div class="tags">
        <span class="tag">Integration Platform</span>
        <span class="tag">Mission-Critical</span>
        <span class="tag">Data Migration</span>
      </div>
    </div>

    <div class="experience-item">
      <div class="experience-header">
        <h3>PostNL</h3>
        <span class="period">Mar 2015 &ndash; Jan 2019</span>
      </div>
      <div class="role">Project Manager, Digital Integration &amp; Transformation</div>
      <p>Led a PostNL-wide strategic transformation to route all logistics and customer processes through a central LSP platform. Implemented organization-wide SAFe adoption and migrated the integration platform to AWS.</p>
      <div class="tags">
        <span class="tag">SAFe</span>
        <span class="tag">AWS</span>
        <span class="tag">Logistics</span>
      </div>
    </div>

    <template v-if="showAllAssignments">
      <div class="experience-item">
        <div class="experience-header">
          <h3>Eneco</h3>
          <span class="period">Apr 2019 &ndash; Aug 2019</span>
        </div>
        <div class="role">Program Manager</div>
        <p>Led an organization-wide strategic transformation programme to integrate all customer interactions within a single CRM/ERP platform (Microsoft BASE), enabling data-driven cross-selling.</p>
        <div class="tags">
          <span class="tag">CRM/ERP</span>
          <span class="tag">Microsoft</span>
          <span class="tag">Customer Data</span>
        </div>
      </div>

      <div class="experience-item">
        <div class="experience-header">
          <h3>Vodafone Germany</h3>
          <span class="period">2014 &ndash; Jan 2015</span>
        </div>
        <div class="role">Sub-Project Manager, Integration &amp; Transformation</div>
        <p>Part of a national programme across eight regions in Germany, responsible for completing the mobile telecommunications modernisation programme. Led improvement of production processes and P2P optimization.</p>
        <div class="tags">
          <span class="tag">Telecom</span>
          <span class="tag">Process Redesign</span>
        </div>
      </div>

      <div class="experience-item">
        <div class="experience-header">
          <h3>KPN</h3>
          <span class="period">Feb 2012 &ndash; Jan 2014</span>
        </div>
        <div class="role">Project Manager</div>
        <p>Implemented an Integrated Customer View for both business and consumer markets, focused on cleansing and maintaining high-quality customer data.</p>
        <div class="tags">
          <span class="tag">Customer Data</span>
          <span class="tag">Data Quality</span>
        </div>
      </div>

      <div class="experience-item">
        <div class="experience-header">
          <h3>Gemeente Amsterdam</h3>
          <span class="period">2011 &ndash; Sep 2012</span>
        </div>
        <div class="role">Advisor &amp; Project Manager</div>
        <p>Designed and implemented an integrated Business Plan for the ICT Services organisation of the Municipality of Amsterdam, including Demand Management processes and a new ICT job framework.</p>
        <div class="tags">
          <span class="tag">Government</span>
          <span class="tag">ICT Services</span>
        </div>
      </div>

      <div class="experience-item">
        <div class="experience-header">
          <h3>ProRail</h3>
          <span class="period">2009 &ndash; Sep 2011</span>
        </div>
        <div class="role">Project Manager</div>
        <p>Established and led an Integration Competence Center (25 FTE). Implemented the TIBCO integration platform as the enterprise backbone and led the "Information Integration" transformation programme.</p>
        <div class="tags">
          <span class="tag">SOA/ESB</span>
          <span class="tag">TIBCO</span>
          <span class="tag">Rail Infrastructure</span>
        </div>
      </div>

      <div class="experience-item">
        <div class="experience-header">
          <h3>ING</h3>
          <span class="period">2008 &ndash; 2009</span>
        </div>
        <div class="role">Project Manager</div>
        <p>Implemented redesigned ING Workplace Services and ITIL processes as part of the outsourcing of all Workplace Services to an external provider.</p>
        <div class="tags">
          <span class="tag">ITIL</span>
          <span class="tag">Banking</span>
          <span class="tag">Outsourcing</span>
        </div>
      </div>
    </template>

    <button class="show-more" :class="{ expanded: showAllAssignments }" @click="showAllAssignments = !showAllAssignments">
      {{ showAllAssignments ? 'Show less' : 'Show 6 more' }}
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m6 9 6 6 6-6"/></svg>
    </button>
  </div>

  <div class="section">
    <h2>Education</h2>

    <div class="education-item">
      <h3>Organisation and Policy</h3>
      <span class="institution">University of Amsterdam</span>
    </div>

    <div class="education-item">
      <h3>Hotelschool The Hague</h3>
      <span class="institution">Diploma</span>
    </div>

    <div class="education-item">
      <h3>Postgraduate Programme in Executive Team Coaching</h3>
      <span class="institution">Vrije Universiteit Amsterdam</span>
    </div>

    <div class="education-item">
      <h3>Design Thinking</h3>
      <span class="institution">Hasso Plattner Institute, Berlin</span>
    </div>

    <div class="education-item">
      <h3>SAFe 4.0 Practitioner</h3>
      <span class="institution">Scaled Agile Framework</span>
    </div>

    <div class="education-item">
      <h3>Real World Risk (Taking)</h3>
      <span class="institution">Nassim Nicholas Taleb</span>
    </div>

    <div class="education-item">
      <h3>PRINCE2, IPMA &amp; MSP</h3>
      <span class="institution">Project &amp; Programme Management</span>
    </div>
  </div>
</template>
