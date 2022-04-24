# Part 1: Remediate Security Review Findings

### Finding 1:
---
We can see that the when we run `kubectl get psp` to view the security policy, our container is running with full privileges which should not be allowed.

In order to remediate the finding, we run `kubectl edit `

![](./Artifacts/policy-1-1.png)