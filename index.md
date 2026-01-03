---
layout: default
title: Home
---

**GOTT Labs** is an independent cybersecurity research project focused on studying how threats operate in practice, how defensive systems respond under real conditions, and where theory quietly diverges from reality.

This site exists to publish research. Any resemblance to marketing is coincidental.

### Research/Write-ups

<div class="filter-controls">
  <div class="filter-header">
    <span class="filter-label">Filter by Research Area:</span>
    <button class="clear-filter" onclick="clearFilter()">Reset View</button>
  </div>
  <div class="filter-grid">
    <button class="filter-tag" onclick="filterByTag('forensics')">forensics</button>
    <button class="filter-tag" onclick="filterByTag('mongodb')">mongodb</button>
    <button class="filter-tag" onclick="filterByTag('oracle_ebs')">oracle_ebs</button>
    <button class="filter-tag" onclick="filterByTag('sap_netweaver')">sap_netweaver</button>
    <button class="filter-tag" onclick="filterByTag('fortigate')">fortigate</button>
    <button class="filter-tag" onclick="filterByTag('panos')">panos</button>
    <button class="filter-tag" onclick="filterByTag('threat_groups')">threat_groups</button>
  </div>
</div>

<div id="research-posts">

<div class="research-post" data-tags="CVE-2025-14847,mongodb,forensics">
  <a href="{{ site.baseurl }}/2025/12/26/mongobleed_forensics_cve2025-14847" class="main-post-link" aria-label="MongoBleed Forensics"></a>
  <div class="post-content">
    <h4>MongoBleed Forensics (CVE-2025-14847)</h4>
    <span class="post-date">CVE Date: December 26, 2025</span>
    <p>MongoBleed, a discussion of forensics and considerations</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('CVE-2025-14847')">CVE-2025-14847</span>
      <span class="tag" onclick="filterByTag('mongodb')">mongodb</span>
      <span class="tag" onclick="filterByTag('forensics')">forensics</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/CVE-2025-14847.png" alt="MongoBleed">
  </div>
</div>

<div class="research-post" data-tags="CVE-2025-61882,oracle_ebs,forensics">
  <a href="{{ site.baseurl }}/2025/10/07/oracle_ebs_cve2025-61882" class="main-post-link" aria-label="Oracle EBS Research"></a>
  <div class="post-content">
    <h4>Oracle EBS (CVE-2025-61882)</h4>
    <span class="post-date">CVE Date: October 7, 2025</span>
    <p>The Zero-Day That Reminded Everyone Why ERP Means "Everyone's Really Pwned"</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('CVE-2025-61882')">CVE-2025-61882</span>
      <span class="tag" onclick="filterByTag('oracle_ebs')">oracle_ebs</span>
      <span class="tag" onclick="filterByTag('forensics')">forensics</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/CVE-2025-61882.png" alt="oracle_ebs">
  </div>
</div>

<div class="research-post" data-tags="CVE-2025-31324,sap_netweaver,forensics">
  <a href="{{ site.baseurl }}/2025/04/26/sap_netweaver_cve2025-31324" class="main-post-link" aria-label="SAP NetWeaver Research"></a>
  <div class="post-content">
    <h4>SAP NetWeaver VC (CVE-2025-31324)</h4>
    <span class="post-date">CVE Date: April 26, 2025</span>
    <p>How an obscure endpoint turned SAP NetWeaver into a webshell wonderland</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('CVE-2025-31324')">CVE-2025-31324</span>
      <span class="tag" onclick="filterByTag('sap_netweaver')">sap_netweaver</span>
      <span class="tag" onclick="filterByTag('forensics')">forensics</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/CVE-2025-31324.png" alt="sap_netweaver">
  </div>
</div>

<div class="research-post" data-tags="CVE-2024-55591,fortigate,forensics">
  <a href="{{ site.baseurl }}/2025/01/14/fortigate_cve2024-55591" class="main-post-link" aria-label="FortiGate Research"></a>
  <div class="post-content">
    <h4>The FortiGate Backdoor That Wasn't A Backdoor (CVE-2024-55591)</h4>
    <span class="post-date">CVE Date: January 14, 2025</span>
    <p>When authentication is just a really aggressive suggestion</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('CVE-2024-55591')">CVE-2024-55591</span>
      <span class="tag" onclick="filterByTag('fortigate')">fortigate</span>
      <span class="tag" onclick="filterByTag('forensics')">forensics</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/CVE-2024-55591.png" alt="fortigate_cve">
  </div>
</div>

<div class="research-post" data-tags="CVE-2024-0012,CVE-2024-9474,panos,forensics">
  <a href="{{ site.baseurl }}/2024/11/18/panos_cve2024-0012" class="main-post-link" aria-label="PAN-OS Research"></a>
  <div class="post-content">
    <h4>PAN-OS (CVE-2024-0012 and CVE-2024-9474)</h4>
    <span class="post-date">CVE Date: November 18, 2024</span>
    <p>When Your Security Appliance Becomes the Vulnerability</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('CVE-2024-0012')">CVE-2024-0012</span>
      <span class="tag" onclick="filterByTag('CVE-2024-9474')">CVE-2024-9474</span>
      <span class="tag" onclick="filterByTag('panos')">panos</span>
      <span class="tag" onclick="filterByTag('forensics')">forensics</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/CVE-2024-0012.png" alt="panos_cve">
  </div>
</div>

<div class="research-post" data-tags="CVE-2024-47575,fortigate,forensics">
  <a href="{{ site.baseurl }}/2024/10/23/fortijump_cve2024-47575" class="main-post-link" aria-label="FortiJump Research"></a>
  <div class="post-content">
    <h4>FortiJump Diving board (CVE-2024-47575)</h4>
    <span class="post-date">CVE Date: October 23, 2024</span>
    <p>How Missing Auth in FortiManager Let UNC5820 Play Musical Chairs with Enterprise Networks</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('CVE-2024-47575')">CVE-2024-47575</span>
      <span class="tag" onclick="filterByTag('fortigate')">fortigate</span>
      <span class="tag" onclick="filterByTag('forensics')">forensics</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/CVE-2024-47575.png" alt="fortijump">
  </div>
</div>

<div class="research-post" data-tags="luna_moth,threat_groups,forensics">
  <a href="{{ site.baseurl }}/2026/01/02/luna_moth" class="main-post-link" aria-label="Luna Moth Research"></a>
  <div class="post-content">
    <h4>Luna Moth: When Social Engineering Beats Malware</h4>
    <span class="post-date">Post Date: January 02, 2026</span>
    <p>How ex-Conti operators are extorting millions without writing a single line of malicious code</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('luna_moth')">luna_moth</span>
      <span class="tag" onclick="filterByTag('threat_groups')">threat_groups</span>
      <span class="tag" onclick="filterByTag('forensics')">forensics</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/luna_moth.png" alt="luna_moth">
  </div>
</div>

</div>

<script>
let currentFilter = null;

function filterByTag(tag) {
  currentFilter = tag;
  const posts = document.querySelectorAll('.research-post');
  const filterTags = document.querySelectorAll('.filter-tag');
  const postTags = document.querySelectorAll('.tag');
  
  // Update filter button states
  filterTags.forEach(ft => {
    if (ft.textContent === tag) {
      ft.classList.add('active');
    } else {
      ft.classList.remove('active');
    }
  });
  
  // Update post tag states
  postTags.forEach(pt => {
    if (pt.textContent === tag) {
      pt.classList.add('active');
    } else {
      pt.classList.remove('active');
    }
  });
  
  // Filter posts
  posts.forEach(post => {
    const tags = post.getAttribute('data-tags').toLowerCase();
    if (tags.includes(tag.toLowerCase())) {
      post.style.display = 'flex';
    } else {
      post.style.display = 'none';
    }
  });
}

function clearFilter() {
  currentFilter = null;
  const posts = document.querySelectorAll('.research-post');
  const filterTags = document.querySelectorAll('.filter-tag');
  const postTags = document.querySelectorAll('.tag');
  
  // Clear all active states
  filterTags.forEach(ft => ft.classList.remove('active'));
  postTags.forEach(pt => pt.classList.remove('active'));
  
  // Show all posts
  posts.forEach(post => {
    post.style.display = 'flex';
  });
}
</script>

### Research Disclaimer
<span class="disclaimer">
Research published is provided for educational purposes. Findings reflect observed behavior in specific environments and should not be interpreted as universal truth, vendor endorsement, or operational guidance. Techniques discussed may be incomplete, ineffective, or rendered obsolete without notice. Readers are expected to apply judgment, skepticism, and basic security hygiene.
</span>
