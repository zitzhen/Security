# ZIT Studio Security Policy

**Effective date:** October 24, 2026  
**Maintained by:** ZIT Studio  
**Policy scope:** Open-source projects maintained by ZIT Studio and related official services

**Language / 语言:** [English](Security.md) | [简体中文](Security-zh-cn.md)

## 1. Security Commitment

ZIT Studio is committed to maintaining a secure, reliable, and transparent open-source software ecosystem. We value feedback about security issues from security researchers, users, and community members, and encourage the responsible discovery, reporting, and remediation of vulnerabilities.

This policy describes how to report security vulnerabilities, how we handle reports, our coordinated disclosure principles, and our commitments to security researchers.

We will make reasonable efforts to respond to security reports promptly, assess potential risks, remediate confirmed issues, and publish security advisories when appropriate.

## 2. Scope

This policy applies to projects that ZIT Studio maintains or controls, including but not limited to:

- The official ZIT Studio GitHub organization and repositories maintained by ZIT Studio.
- Software, packages, installers, and official distribution channels published by ZIT Studio.
- Official websites and related online services operated or managed by ZIT Studio.
- Other projects or components that ZIT Studio explicitly includes in its security maintenance scope.

For third-party dependencies, external services, upstream projects, and other systems that ZIT Studio does not control, we may report issues to the relevant maintainers or service providers and assist with coordination where reasonable.

**Please note:** Finding a vulnerability in one project does not mean that all of its upstream dependencies, third-party services, or related systems are authorized for testing under this policy.

## 3. How to Report a Security Vulnerability

If you believe you have found a security issue affecting a ZIT Studio project or service, please report it privately through one of the following channels:

1. **GitHub Private Vulnerability Reporting:** If enabled for the affected repository, submit a private vulnerability report from the repository's Security page.
2. **GitHub Security Advisories:** If supported by the repository, use the private security advisory process to contact the maintainers.
3. **Official project contact information:** If neither option is available, contact the team using the information in the relevant repository's README, on the official website, or through another public maintainer contact. Clearly identify your message as a security vulnerability report.

Please do not disclose details of an unpatched vulnerability that may affect users in a public issue, discussion, or other public channel.

### Recommended Report Information

To help us reproduce and assess the issue, please include, where possible:

- The affected project name, repository URL, and version.
- The vulnerability type and its potential impact.
- Reproduction steps and necessary technical details.
- Logs, screenshots, or minimal validation materials obtained safely and lawfully.
- Suggested fixes or mitigations, if any.
- Contact information so maintainers can follow up.

You do not need to provide your legal name, identity documents, or other personal information unrelated to validating the vulnerability.

## 4. Vulnerability Handling Process

After receiving a security report, ZIT Studio will make reasonable efforts to follow this process:

1. **Receipt and acknowledgment:** Confirm receipt of the report and establish any necessary communication with the reporter.
2. **Reproduction and assessment:** Attempt to reproduce the vulnerability and identify affected components and versions, exploitation conditions, and potential impact.
3. **Risk classification:** Set a handling priority based on factors such as actual impact, exploitability, and scope.
4. **Remediation and mitigation:** Develop, test, and release a fix, or provide an appropriate mitigation if a complete fix is not immediately possible.
5. **Coordinated disclosure:** Coordinate the disclosure schedule and advisory content with the reporter and any necessary upstream maintainers.
6. **Public advisory:** When appropriate, publish an advisory describing the affected scope, fixed versions, and actions users should take.

We will prioritize reports based on severity, actual impact, maintenance resources, and remediation complexity. Issues that are being exploited or could have a significant impact will receive priority assessment and handling.

## 5. Response Time Targets

To make our security handling process more transparent, ZIT Studio uses the following target time frames:

| Handling stage | Target |
| --- | --- |
| Acknowledge receipt of a report | Within 3 business days |
| Initial assessment | Within 7 business days |
| Progress updates | Generally every 7 business days |
| Remediation and public disclosure | Determined by risk, remediation complexity, and coordination needs |

These are target time frames, not unconditional service guarantees. Complex vulnerabilities, upstream dependency issues, maintainer availability, or the need to coordinate with third parties may extend the handling time.

If we expect to miss a target, we will make reasonable efforts to tell the reporter why and explain the next steps.

## 6. Coordinated Vulnerability Disclosure

ZIT Studio supports Coordinated Vulnerability Disclosure (CVD).

While a vulnerability is being remediated and an advisory is being prepared, we will generally work with the reporter to agree on a reasonable disclosure schedule so affected users have an opportunity to protect themselves.

Absent special risks or other necessary circumstances, the parties may use 90 days after the first valid report as a reference for discussing coordinated disclosure. This is not a mandatory waiting period or an absolute deadline.

If a vulnerability is being exploited publicly, presents a significant risk, or requires an earlier advisory, we may disclose necessary information sooner where reasonable. We will assess requests to delay disclosure based on remediation progress, user risk, and the relevant facts.

A security advisory may include:

- A brief description of the vulnerability and its scope of impact.
- Affected and fixed versions.
- Available upgrade, remediation, or mitigation steps.
- Appropriate acknowledgments.
- A CVE identifier or other advisory identifier, where applicable.

Without an appropriate assessment, we will not publish sensitive technical details that could directly help attackers exploit an unpatched vulnerability merely to meet a disclosure time frame.

## 7. CVEs and Vulnerability Identifiers

Subject to applicable rules and authorization, ZIT Studio will consider requesting or coordinating the assignment of a CVE identifier based on the nature and impact of a vulnerability.

For eligible vulnerabilities within the team's authorized scope, we may coordinate through an appropriate CVE assignment channel, a relevant CVE Numbering Authority (CNA), or an upstream project.

Receiving a CVE identifier does not mean that a vulnerability has been fixed, nor does it automatically mean that all affected projects have been addressed.

If a vulnerability involves third-party software or an upstream project, we will coordinate with the relevant maintainers where possible to avoid duplicate identifiers and unnecessary disclosure conflicts.

## 8. Security Researcher Protections

To the extent permitted by law, and provided that researchers follow this policy and conduct research in good faith, ZIT Studio:

- Will not initiate legal action against a researcher solely because they submitted a vulnerability report in accordance with this policy.
- Will not hold a researcher responsible solely for submitting a good-faith vulnerability report for conduct unrelated to normal reporting.
- Respects reasonable requests for attribution or anonymity when a researcher makes a public disclosure.
- Encourages appropriate acknowledgment of researchers who make a substantive contribution in reports and advisories.
- Does not require researchers to access, modify, delete, or disclose unrelated user data to demonstrate a vulnerability.

These principles do not constitute legal immunity, legal representation, or a guarantee regarding the actions of third parties. They also do not authorize activity that violates applicable law, third-party rules, or other explicit authorization boundaries.

## 9. Security Research Rules of Conduct

We encourage researchers to validate issues without increasing risk and to follow these principles:

- Perform only the minimum testing necessary to validate the vulnerability.
- Do not access, collect, modify, or disclose data unrelated to validating the vulnerability.
- Do not conduct unauthorized denial-of-service testing, destructive actions, or large-scale automated attacks.
- Do not use a vulnerability to steal credentials, access unrelated systems, or affect other users.
- If you unexpectedly obtain sensitive data, stop accessing it and describe the situation in your report.
- If an issue may cause ongoing real-world harm, stop testing first and notify the maintainers promptly.

For systems outside this policy's scope, obtain explicit authorization from the relevant system owner before testing.

## 10. Supported Versions and Security Maintenance

ZIT Studio determines security support based on each project's maintenance status, release policy, and available maintenance capacity.

For versions that are still maintained, we will make reasonable efforts to assess confirmed security issues and, where necessary, release fixes or security advisories.

We may be unable to provide fixes for projects or versions that are no longer maintained, have been archived, or are otherwise unsupported. Users should follow project announcements and upgrade to a supported version when possible.

When a dependency has a security issue, we will assess the actual impact and decide whether to upgrade the dependency, apply a patch, adjust configuration, or use another mitigation.

## 11. Policy Updates

ZIT Studio may update this policy as projects evolve, based on vulnerability handling experience, applicable laws, and security industry practices.

Updates will be published on the official website or in the relevant project repository. Unless explicitly stated otherwise, a policy update should not be interpreted as retroactive authorization for past activity.

If you have questions about this policy, the vulnerability reporting process, or security advisories, contact the team using the contact information on the official ZIT Studio website or in the relevant project repository.

---

**ZIT Studio Security Team**

We thank all researchers, contributors, and community members who help improve open-source software security responsibly.

Security is an ongoing shared effort. We welcome constructive security reports and will make reasonable efforts to work with reporters to help protect users and the open-source community.
