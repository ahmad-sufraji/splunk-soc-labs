# Splunk SPL Investigation Queries

**Project:** Web Attack Detection & Investigation  
**Environment:** Educational Splunk Lab  
**Data:** Synthetic Nginx web logs

## 1. Detect HTTP Failure Responses

```spl
index=web_lab sourcetype=nginx:access
| where status>=400
| stats count AS failed_requests by src status
| sort - failed_requests
```

**Purpose:** Identify sources generating HTTP failure responses.

## 2. Identify Suspicious Path Enumeration

```spl
index=web_lab sourcetype=nginx:access
| stats count AS requests dc(uri_path) AS unique_paths values(uri_path) AS requested_paths by src
| where unique_paths > 20
| sort - unique_paths
```

**Purpose:** Identify sources requesting many unique web paths.

## 3. Analyze HTTP Response Codes

```spl
index=web_lab sourcetype=nginx:access
| stats count by src status
| sort - count
```

**Purpose:** Examine HTTP response patterns and identify unusual activity.

---

**Note:** These queries are designed for a synthetic Nginx dataset with the documented field names. Index and sourcetype values must match the local lab configuration before execution.
