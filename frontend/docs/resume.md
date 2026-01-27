---
outline: false
prev: false
next: false
title: "Resume"
description: "Download Gwendolin Tan's professional resume. Senior Product Manager at FWD Insurance with 10+ years of experience in product management, digital platforms, and strategic delivery."
keywords: "Gwendolin Tan resume, product manager resume, FWD, Lazada, Amadeus, B2B SaaS, Singapore, SMU, Chatbot, AI, CX, e-commerce"
author: "Gwendolin Tan"
head:
  - - meta
    - property: og:title
      content: "Resume"
  - - meta
    - property: og:description
      content: "Download Gwendolin Tan's professional resume. Senior Product Manager at FWD Insurance with 10+ years of experience in product management, digital platforms, and strategic delivery."
  - - meta
    - property: og:type
      content: profile
  - - meta
    - property: og:url
      content: https://gwendolintan.com/resume
  - - link
    - rel: canonical
      href: https://gwendolintan.com/resume
---

<script setup lang="ts">
import { defineAsyncComponent, ref, onMounted, nextTick } from 'vue'

const isClient = ref(false)
const downloadButtonRef = ref(null)

onMounted(async () => {
  isClient.value = true

  // Check if we should auto-trigger download (from navigation)
  const urlParams = new URLSearchParams(window.location.search)
  const autoDownload = urlParams.get('auto') === 'true'
  
  if (autoDownload) {
    // Wait for the component to be fully mounted
    await nextTick()
    
    // Try multiple approaches with increasing delays
    const attemptDownload = (attempt = 1) => {      
      // Method 1: Try DOM query
      const downloadBtn = document.querySelector('button[data-download-resume]')
      if (downloadBtn) {
        downloadBtn.click()
        return
      }
      
      // Method 2: Retry if component hasn't loaded yet (max 5 attempts)
      if (attempt < 5) {
        setTimeout(() => attemptDownload(attempt + 1), 300 * attempt)
      } else {
        console.warn('Could not trigger auto-download - component not ready')
      }
    }
    
    // Start the first attempt after a small delay
    setTimeout(() => attemptDownload(), 200)
  }
})

const DownloadResumeButton = defineAsyncComponent({
  loader: () => import('./components/DownloadResume.vue'),
  loadingComponent: {
    template: `<button class="!border-none !py-2.5 !px-6 !text-center !no-underline !inline-block !text-base !m-1 !cursor-wait !rounded-full !font-medium !transition-all !duration-300 !shadow-sm !font-sans !tracking-wide !bg-gray-400 !text-white">Loading...</button>`
  },
  delay: 0,
  timeout: 10000
})
</script>

<div style="text-align: right; margin-bottom: 20px;">
  <ClientOnly>
    <DownloadResumeButton ref="downloadComponentRef" filename="Gwendolin Tan.pdf" />
  </ClientOnly>
</div>

# Gwendolin Tan

[LinkedIn](https://www.linkedin.com/in/gwendolintan) | [gwendolin.tan@gmail.com](mailto:gwendolin.tan@gmail.com) | (65) 9220 8692 | [www.gwendolintan.com](https://www.gwendolintan.com)

## Personal Profile

Product Manager with 10+ years of experience in requirements and data analysis, strategy, solutions design, product feature development, and end-to-end project delivery. A self-starter who has implemented proofs-of-concept, conducted competitor analysis, and shaped the customer experience through data-driven features and UX. Skill set encompasses features built for diverse product categories, including SaaS, B2C, e-commerce, AI/ML and GenAI. Fluent in both English and fair in Business Chinese.

## Core Competencies

GenAI • Arize AI • ML Lifecycle • Agile • Scrum • Product backlog management • Design thinking • Project management • JIRA • Confluence • SQL • Figma • Python • Excel • Microsoft Office

## Work Experience

### FWD Insurance Pte. Ltd.

**Senior Product Manager, Group Digital Platforms** | Singapore | July 2025 – Present  
**Product Manager, Group Digital Platforms** | Singapore | June 2024 – June 2025

- Drove agent assistant adoption, with high adopters achieving 12% higher APE and 40% more cases than low adopters.
- Spearheaded automation of data and tagging workflows, reducing manual effort by 1 day per request and accelerating insights by up to 2 days through GPT-powered analysis.
- Improved the company’s agentic generative AI chatbot accuracy by 20% through new features and performance optimisations.
- Drove 2% increase in adoption via agent interviews, iterative improvements, and promotions.
- Improved avatar UX for a C-level event by refining prompts and testing scenarios, leading to positive stakeholder feedback.
- Scaled adoption of GenAI agent assistants in 4 strategic markets, delivering all go-lives on time.
- Partnered with engineering team to monitor and troubleshoot AI models using Arize AI.

### Lazada

**Manager, Product Management** | Singapore | October 2023 – January 2024  
**Manager, Project / Program Management** | Singapore | May 2023 – October 2023  
**Senior Associate, Regional AI Business Product Owner** | Singapore | June 2021 – April 2023

- Led cross-functional product strategy, propelling chatbot utilization by 7%, resolution rate by 20%, and response rate by 10%.
- Boosted case management usage by 300% (buyer) and 1600% (seller) through key feature launches.
- Launched 2 GenAI features and crafted the prompts, resulting in 20% less dissatisfaction in the replies.
- Championed the adoption of 3rd party automation tool boosting automatic review reply rate by 50%.
- Launched inaugural internal dashboards to enable data-driven impact analysis, monitoring key metrics, and derive insights.
- Coordinated with data science and engineering teams on the model training, tuning and deployment of ML models.

### Amadeus GDS Singapore Pte. Ltd.

**Technical Product Owner** | Singapore | August 2019 – May 2021

- Designed key features and UI enhancements for 3 modules of our SaaS-based Airport Management Suite (AMS).
- Convinced the global senior management team on the merits of the above-mentioned redesign.
- Spearheaded functional integration between AMS and our firm’s best-selling solution.
- Championed for consistency in UI and technical implementations across the 3 modules.
- Expedited the design, implementation, and testing of a new requirement to production within 2 weeks.

### Atos Information Technology (Singapore) Pte. Ltd.

**Business Analyst** | Singapore | June 2015 – July 2019

- Delivered cross-functional full life cycle content management applications for 2 government agencies, one 3 months ahead.
- Owned execution of above-mentioned projects from design, implementation, build, testing, and training.
- Analyzed and generated reports from SQL database to troubleshoot issues.
- Communicated and delivered key enhancements to deliveries based on user feedback within 1-2 weeks.

## Education

### Singapore Management University

**Bachelor of Science (Information Systems Management)** | August 2012 - May 2015

Second Major in Operations Management

## Awards and Certifications

- HFI UX 1 – Usability Engineering Course | February 2021
- Certified Scrum Product Owner (CSPO) | December 2020
- ICAgile Certified Professional – Agile Team Facilitation | December 2020
- Certified Scrum Master (CSM) | May 2019
- NICF – Data Storytelling (SF) | April 2019
- DS102: Data Analytics with Python | April 2019
- Tableau Desktop I & II: Fundamentals | July 2018
- NICF Predictive Analytics – Insights of Trends and Irregularities | September 2018
