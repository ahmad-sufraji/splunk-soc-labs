# Incident Investigation Report
## Automated Web Path Enumeration

**Incident Category:** Web Reconnaissance  
**Severity:** High (Simulated Alert)  
**Investigation Status:** Completed – No Confirmed Compromise

### 1. Incident Summary

A simulated SIEM alert detected an unusual volume of HTTP GET requests targeting multiple PHP and administrative paths on a web application.

The activity pattern was consistent with automated web path enumeration.

### 2. Key Findings

- Multiple unique web paths were requested within a short period.
- Requests targeted PHP files and administrative endpoints.
- HTTP 404 responses were observed.
- User-Agent information was unavailable in the simulated events.
- No successful exploitation was established.

### 3. Technical Analysis

The repeated requests to different PHP endpoints suggest automated reconnaissance intended to discover accessible files or administrative interfaces.

The observed HTTP 404 responses indicate that the requested resources were not found.

### 4. MITRE ATT&CK Mapping

- **T1595 – Active Scanning:** Consistent with the observed reconnaissance behavior.
- **T1595.003 – Wordlist Scanning:** Potential mapping for automated path discovery.

### 5. Conclusion

The activity is classified as suspicious automated web reconnaissance.

No confirmed compromise or data exfiltration was identified within the simulated investigation scope.

### 6. Recommendations

1. Monitor repeated requests to unusual web paths.
2. Apply appropriate rate limiting and WAF protections.
3. Review web application and server logs.
4. Investigate unexpected PHP files and administrative endpoints.
5. Monitor for subsequent exploitation attempts.

---

**Project Type:** Educational SOC Investigation  
**Data Classification:** Synthetic / Fictional  
**Environment:** Independent Splunk Lab
