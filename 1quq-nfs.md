---
title: #[[2ntn-exploit|Exploiting]] NFS
created: 2022-09-28
keywords: [Programming, Hacking]
---

- Can exploit if root-squash is misconfigured, via setting SUID permissions, which allows root access for specific files. Therefore, if we can download a bash executable on the machine, and give it SUID access, we have a root shell.
