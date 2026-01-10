---
layout: default
title: Home
---

**GOTT Labs** is an independent cybersecurity research project focused on studying how threats operate in practice, how defensive systems respond under real conditions, and where theory quietly diverges from reality.

This site exists to publish research. Any resemblance to marketing is coincidental.

<script>
let currentFilter = null;
function filterByTag(tag) {
  currentFilter = tag;
  const posts = document.querySelectorAll('.research-post');
  const filterTags = document.querySelectorAll('.filter-tag');
  const postTags = document.querySelectorAll('.tag');
    filterTags.forEach(ft => {
    if (ft.textContent === tag) {
      ft.classList.add('active');
    } else {
      ft.classList.remove('active');
    }
  });
    postTags.forEach(pt => {
    if (pt.textContent === tag) {
      pt.classList.add('active');
    } else {
      pt.classList.remove('active');
    }
  });
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
  filterTags.forEach(ft => ft.classList.remove('active'));
  postTags.forEach(pt => pt.classList.remove('active'));
  posts.forEach(post => {
    post.style.display = 'flex';
  });
}
</script>

### Research/Write-ups

<div class="filter-controls">
  <div class="filter-header">
    <span class="filter-label">Filter by Research Area:</span>
    <button class="clear-filter" onclick="clearFilter()">Reset View</button>
  </div>
  <div class="filter-grid">
    <button class="filter-tag" onclick="filterByTag('forensics')">forensics</button>
    <button class="filter-tag" onclick="filterByTag('vulnerability')">vulnerability</button>
    <button class="filter-tag" onclick="filterByTag('threat_groups')">threat_groups</button>
    <button class="filter-tag" onclick="filterByTag('research')">research</button>
    <button class="filter-tag" onclick="filterByTag('mongodb')">mongodb</button>
    <button class="filter-tag" onclick="filterByTag('oracle_ebs')">oracle_ebs</button>
    <button class="filter-tag" onclick="filterByTag('sap_netweaver')">sap_netweaver</button>
    <button class="filter-tag" onclick="filterByTag('fortinet')">fortinet</button>
    <button class="filter-tag" onclick="filterByTag('panos')">panos</button>
    <button class="filter-tag" onclick="filterByTag('sonicwall')">sonicwall</button>
  </div>
</div>

<div id="research-posts">

<div class="research-post" data-tags="research,threat_groups">
  <div class="post-content">
    <h4><a href="{{ site.baseurl }}/2026/01/10/tds_part1">Internet Traffic Brokers: TDS and the VexTrio Criminal Enterprise</a></h4>
    <span class="post-date">Published: January 10, 2026</span>
    <p>How a Billion-Dollar Cybercrime Operation Hides Behind Legitimate AdTech (Part 1)</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('research')">research</span>
      <span class="tag" onclick="filterByTag('threat_groups')">threat_groups</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/vextrio_tds_part1.png" alt="vextrio_tds_part1">
  </div>
</div>

<div class="research-post" data-tags="CVE-2025-14847,mongodb,forensics,vulnerability">
  <div class="post-content">
    <h4><a href="{{ site.baseurl }}/2025/12/26/mongobleed_forensics_cve2025-14847">MongoBleed Forensics (CVE-2025-14847)</a></h4>
    <span class="post-date">CVE Date: December 26, 2025</span>
    <p>MongoBleed, a discussion of forensics and considerations</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('CVE-2025-14847')">CVE-2025-14847</span>
      <span class="tag" onclick="filterByTag('mongodb')">mongodb</span>
      <span class="tag" onclick="filterByTag('forensics')">forensics</span>
      <span class="tag" onclick="filterByTag('vulnerability')">vulnerability</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/CVE-2025-14847.png" alt="MongoBleed">
  </div>
</div>

<div class="research-post" data-tags="CVE-2025-59718,fortinet,forensics,vulnerability">
  <div class="post-content">
    <h4><a href="{{ site.baseurl }}/2026/01/06/forti_cve2025-59718">Trust But Don't Verify (Forti CVE-2025-59718)</a></h4>
    <span class="post-date">CVE Date: November 9, 2025</span>
    <p>CVE-2025-59718 & CVE-2025-59719 - Who Needs Signature Verification Anyway?</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('CVE-2025-59718')">CVE-2025-59718</span>
      <span class="tag" onclick="filterByTag('fortinet')">fortinet</span>
      <span class="tag" onclick="filterByTag('forensics')">forensics</span>
      <span class="tag" onclick="filterByTag('vulnerability')">vulnerability</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/CVE-2025-59718.png" alt="forti_vuln2">
  </div>
</div>

<div class="research-post" data-tags="CVE-2025-59287,WSUS,forensics,vulnerability">
  <div class="post-content">
    <h4><a href="{{ site.baseurl }}/2026/01/07/wsus_cve2025-59287">CVE-2025-59287 and the WSUS Deserialization Nightmare</a></h4>
    <span class="post-date">CVE Date: October 10, 2025</span>
    <p>A critical unauthenticated RCE vulnerability that turned Microsoft's patch delivery system into an attacker's dream"</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('CVE-2025-61882')">CVE-2025-59287</span>
      <span class="tag" onclick="filterByTag('forensics')">forensics</span>
      <span class="tag" onclick="filterByTag('vulnerability')">vulnerability</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/CVE-2025-59287.png" alt="wsus_windows">
  </div>
</div>

<div class="research-post" data-tags="CVE-2025-61882,oracle_ebs,forensics,vulnerability">
  <div class="post-content">
    <h4><a href="{{ site.baseurl }}/2025/10/07/oracle_ebs_cve2025-61882">Oracle EBS (CVE-2025-61882)</a></h4>
    <span class="post-date">CVE Date: October 7, 2025</span>
    <p>The Zero-Day That Reminded Everyone Why ERP Means "Everyone's Really Pwned"</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('CVE-2025-61882')">CVE-2025-61882</span>
      <span class="tag" onclick="filterByTag('oracle_ebs')">oracle_ebs</span>
      <span class="tag" onclick="filterByTag('forensics')">forensics</span>
      <span class="tag" onclick="filterByTag('vulnerability')">vulnerability</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/CVE-2025-61882.png" alt="oracle_ebs">
  </div>
</div>

<div class="research-post" data-tags="CVE-2025-31324,sap_netweaver,forensics,vulnerability">
  <div class="post-content">
    <h4><a href="{{ site.baseurl }}/2025/04/26/sap_netweaver_cve2025-31324">SAP NetWeaver VC (CVE-2025-31324)</a></h4>
    <span class="post-date">CVE Date: April 26, 2025</span>
    <p>How an obscure endpoint turned SAP NetWeaver into a webshell wonderland</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('CVE-2025-31324')">CVE-2025-31324</span>
      <span class="tag" onclick="filterByTag('sap_netweaver')">sap_netweaver</span>
      <span class="tag" onclick="filterByTag('forensics')">forensics</span>
      <span class="tag" onclick="filterByTag('vulnerability')">vulnerability</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/CVE-2025-31324.png" alt="sap_netweaver">
  </div>
</div>

<div class="research-post" data-tags="CVE-2024-55591,fortinet,forensics,vulnerability">
  <div class="post-content">
    <h4><a href="{{ site.baseurl }}/2025/01/14/fortigate_cve2024-55591">The FortiGate Backdoor That Wasn't A Backdoor (CVE-2024-55591)</a></h4>
    <span class="post-date">CVE Date: January 14, 2025</span>
    <p>When authentication is just a really aggressive suggestion</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('CVE-2024-55591')">CVE-2024-55591</span>
      <span class="tag" onclick="filterByTag('fortinet')">fortinet</span>
      <span class="tag" onclick="filterByTag('forensics')">forensics</span>
      <span class="tag" onclick="filterByTag('vulnerability')">vulnerability</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/CVE-2024-55591.png" alt="forti_cve1">
  </div>
</div>

<div class="research-post" data-tags="CVE-2024-0012,CVE-2024-9474,panos,forensics,vulnerability">
  <div class="post-content">
    <h4><a href="{{ site.baseurl }}/2024/11/18/panos_cve2024-0012">PAN-OS (CVE-2024-0012 and CVE-2024-9474)</a></h4>
    <span class="post-date">CVE Date: November 18, 2024</span>
    <p>When Your Security Appliance Becomes the Vulnerability</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('CVE-2024-0012')">CVE-2024-0012</span>
      <span class="tag" onclick="filterByTag('CVE-2024-9474')">CVE-2024-9474</span>
      <span class="tag" onclick="filterByTag('panos')">panos</span>
      <span class="tag" onclick="filterByTag('forensics')">forensics</span>
      <span class="tag" onclick="filterByTag('vulnerability')">vulnerability</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/CVE-2024-0012.png" alt="panos_cve">
  </div>
</div>

<div class="research-post" data-tags="CVE-2024-47575,fortinet,forensics,vulnerability">
  <div class="post-content">
    <h4><a href="{{ site.baseurl }}/2024/10/23/fortijump_cve2024-47575">FortiJump Diving board (CVE-2024-47575)</a></h4>
    <span class="post-date">CVE Date: October 23, 2024</span>
    <p>How Missing Auth in FortiManager Let UNC5820 Play Musical Chairs with Enterprise Networks</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('CVE-2024-47575')">CVE-2024-47575</span>
      <span class="tag" onclick="filterByTag('fortinet')">fortinet</span>
      <span class="tag" onclick="filterByTag('forensics')">forensics</span>
      <span class="tag" onclick="filterByTag('vulnerability')">vulnerability</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/CVE-2024-47575.png" alt="fortijump">
  </div>
</div>

<div class="research-post" data-tags="luna_moth,threat_groups,forensics">
  <div class="post-content">
    <h4><a href="{{ site.baseurl }}/2026/01/02/luna_moth">Luna Moth: When Social Engineering Beats Malware</a></h4>
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

<div class="research-post" data-tags="CVE-2024-53704,sonicwall,forensics,vulnerability">
  <div class="post-content">
    <h4><a href="{{ site.baseurl }}/2026/01/05/sonicwall_cve2024-53704">CVE-2024-53704: SonicWall Session Hijack</a></h4>
    <span class="post-date">CVE Date: November 05, 2024</span>
    <p>When 32 Null Bytes Break Authentication and SIEM Logs Miss Everything That Matters</p>
    <div class="post-tags">
      <span class="tag" onclick="filterByTag('CVE-2024-53704')">CVE-2024-53704</span>
      <span class="tag" onclick="filterByTag('sonicwall')">sonicwall</span>
      <span class="tag" onclick="filterByTag('forensics')">forensics</span>
      <span class="tag" onclick="filterByTag('vulnerability')">vulnerability</span>
    </div>
  </div>
  <div class="post-image">
    <img src="{{ site.baseurl }}/assets/images/CVE-2024-53704.png" alt="sonicwall">
  </div>
</div>

</div>

### Research Disclaimer
<span class="disclaimer">
Research published is provided for educational purposes. Findings reflect observed behavior in specific environments and should not be interpreted as universal truth, vendor endorsement, or operational guidance. Techniques discussed may be incomplete, ineffective, or rendered obsolete without notice. Readers are expected to apply judgment, skepticism, and basic security hygiene.
</span>
