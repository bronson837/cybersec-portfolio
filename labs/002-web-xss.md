# 002 — Web: Reflected XSS (PortSwigger / Lab)

**Date:** 2025-10-17  
**Time spent:** 2.0 hrs  
**Tools used:** Burp Suite, Firefox, PortSwigger Web Security Academy

## Objective
Understand how reflected XSS works by completing a PortSwigger lab.

## Steps taken
1. Completed the PortSwigger “Reflected XSS” lab.
2. Intercepted the request in Burp and modified the parameter payload to confirm output reflection.
3. Verified the payload rendered in the browser (lab environment only).

## Findings
- Demonstrated a reflected XSS vector in a controlled lab.
- Verified mitigation steps: properly escape/encode user-supplied input and implement Content Security Policy (CSP).

## Remediation / Notes
- Sanitize untrusted input on both server and client sides.
- Recommend CSP + HTTPOnly cookies where applicable.

## Evidence
- Burp Proxy screenshot and sanitized request/response saved locally (not published).
