---
layout: post
title: "Patch Advisory – Token Leak via Console"
---

**Summary:**  
Discovered a token exposed in client-side logs under debug mode. No exploitation attempted. Admin was notified 2025-04-28.

**Steps to Reproduce:**  
1. Enable verbose debug on version `1.2.3`  
2. View browser console after login  
3. Find JWT token in plain text

**Resolution:**  
Patch released in `v1.2.4`, removing console output.

**Disclosure Status:**  
Vendor acknowledged, fixed within 48h.
