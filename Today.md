# Update 2026-09-06
## CVE-2026-85769
 A flaw was found in libtpms, a library that provides software TPM 2.0 emulation. When restoring TPM 2.0 state (for example during a virtual machine's power-on or state/migration restore), a malformed state blob can supply an oversized skip-block length that is not validated against the remaining size of the input buffer. This can drive an internal size counter negative, which bypasses a subsequent bounds check due to an unsafe signed-to-unsigned conversion, causing the parser to read memory outside the bounds of the heap buffer holding the state data. Successful exploitation can crash the process hosting libtpms (such as swtpm), resulting in a denial of service of the emulated TPM device and the virtual machine that depends on it. No data corruption or information disclosure was confirmed.

- [https://github.com/isukasanuj/CVE-2026-85769](https://github.com/isukasanuj/CVE-2026-85769) :  ![starts](https://img.shields.io/github/stars/isukasanuj/CVE-2026-85769.svg) ![forks](https://img.shields.io/github/forks/isukasanuj/CVE-2026-85769.svg)


## CVE-2026-85649
 (Holloway) Chew, Kean Ho's Actualizer v1.2.0 and earlier contains a fail-open password validation vulnerability in the Alpha user and root user password loops of Shell/debian-minbase-install.sh. The installer invokes mkpasswd to generate yescrypt password hashes but does not check the command's return value and unconditionally accepts the result. If mkpasswd fails to generate a yescrypt hash, for example because an incompatible mkpasswd implementation or an environment without yescrypt support is used, the resulting password hash variable can be empty and the build proceeds. The resulting image can therefore contain empty password fields for the root and alpha accounts, potentially permitting passwordless authentication depending on the authentication configuration.

- [https://github.com/ChewKeanHo/research-cve-2026-85649](https://github.com/ChewKeanHo/research-cve-2026-85649) :  ![starts](https://img.shields.io/github/stars/ChewKeanHo/research-cve-2026-85649.svg) ![forks](https://img.shields.io/github/forks/ChewKeanHo/research-cve-2026-85649.svg)


## CVE-2026-85046
 Type confusion in V8 in Google Chrome prior to 152.0.7977.82 allowed a remote attacker to execute arbitrary code inside the sandbox via a crafted HTML page. (Chromium security severity: High)

- [https://github.com/HORKimhab/CVE-2026-85046](https://github.com/HORKimhab/CVE-2026-85046) :  ![starts](https://img.shields.io/github/stars/HORKimhab/CVE-2026-85046.svg) ![forks](https://img.shields.io/github/forks/HORKimhab/CVE-2026-85046.svg)
- [https://github.com/ubitquity/CVE-2026-85046-Patch-confusion-zero-day-vulnerability-in-Google-Chrome-s-V8-engine](https://github.com/ubitquity/CVE-2026-85046-Patch-confusion-zero-day-vulnerability-in-Google-Chrome-s-V8-engine) :  ![starts](https://img.shields.io/github/stars/ubitquity/CVE-2026-85046-Patch-confusion-zero-day-vulnerability-in-Google-Chrome-s-V8-engine.svg) ![forks](https://img.shields.io/github/forks/ubitquity/CVE-2026-85046-Patch-confusion-zero-day-vulnerability-in-Google-Chrome-s-V8-engine.svg)


## CVE-2026-83548
 A Pre-authentication SSRF vulnerability exists in the SMA1000 Appliance Work Place interface due to an unintended alternate access path. A remote unauthenticated attacker could potentially exploit this vulnerability to gain unauthorized access to sensitive functionality and perform unauthorized operations.

- [https://github.com/xcoy0te/CVE-2026-83548-checker](https://github.com/xcoy0te/CVE-2026-83548-checker) :  ![starts](https://img.shields.io/github/stars/xcoy0te/CVE-2026-83548-checker.svg) ![forks](https://img.shields.io/github/forks/xcoy0te/CVE-2026-83548-checker.svg)


## CVE-2026-82876
 Phison PS3111-S11 controller firmware verifies RSA signatures using a public modulus embedded within the firmware image itself rather than anchored in immutable storage. Attackers can generate arbitrary RSA key pairs, sign modified firmware with the private key, embed the matching modulus in the signature segment, and the controller accepts the tampered firmware as valid.

- [https://github.com/Hunt-Benito/the-key-ships-with-the-lock-cve-2026-82876-phison-s11-ssd-firmware-signature-bypass](https://github.com/Hunt-Benito/the-key-ships-with-the-lock-cve-2026-82876-phison-s11-ssd-firmware-signature-bypass) :  ![starts](https://img.shields.io/github/stars/Hunt-Benito/the-key-ships-with-the-lock-cve-2026-82876-phison-s11-ssd-firmware-signature-bypass.svg) ![forks](https://img.shields.io/github/forks/Hunt-Benito/the-key-ships-with-the-lock-cve-2026-82876-phison-s11-ssd-firmware-signature-bypass.svg)


## CVE-2026-82329
 JFrog Artifactory contains an authentication weakness that, under default configuration, may allow an unauthenticated attacker with network access to obtain administrative privileges.

- [https://github.com/gagaltotal/CVE-2026-82329-poc](https://github.com/gagaltotal/CVE-2026-82329-poc) :  ![starts](https://img.shields.io/github/stars/gagaltotal/CVE-2026-82329-poc.svg) ![forks](https://img.shields.io/github/forks/gagaltotal/CVE-2026-82329-poc.svg)


## CVE-2026-78839
 An arbitrary file upload vulnerability in AppNitro MachForm v30 allows attackers to execute arbitrary code via uploading a crafted .phar file.

- [https://github.com/nabeelmkhan/CVE-2026-78839](https://github.com/nabeelmkhan/CVE-2026-78839) :  ![starts](https://img.shields.io/github/stars/nabeelmkhan/CVE-2026-78839.svg) ![forks](https://img.shields.io/github/forks/nabeelmkhan/CVE-2026-78839.svg)


## CVE-2026-78745
 An issue in HiDPT/ Weyon HiDPTAndroid Hi3751V350 Hi3751V352E_DMO allows a remote attacker to execute arbitrary code via the Android Debug Bridge (ADB) daemon (adbd)

- [https://github.com/n0c71v3x/CVE-2026-78745](https://github.com/n0c71v3x/CVE-2026-78745) :  ![starts](https://img.shields.io/github/stars/n0c71v3x/CVE-2026-78745.svg) ![forks](https://img.shields.io/github/forks/n0c71v3x/CVE-2026-78745.svg)


## CVE-2026-77818
This issue affects Library Information and Document Automation Program: from v22.1 before v22.2.

- [https://github.com/alkimcoskun/Yordam-Kutuphane-Otomasyonunda-Coklu-HTML-Enjeksiyonu](https://github.com/alkimcoskun/Yordam-Kutuphane-Otomasyonunda-Coklu-HTML-Enjeksiyonu) :  ![starts](https://img.shields.io/github/stars/alkimcoskun/Yordam-Kutuphane-Otomasyonunda-Coklu-HTML-Enjeksiyonu.svg) ![forks](https://img.shields.io/github/forks/alkimcoskun/Yordam-Kutuphane-Otomasyonunda-Coklu-HTML-Enjeksiyonu.svg)


## CVE-2026-75431
 PowerJob Server version 5.1.2 (and likely earlier) uses a predictable JWT signing key for HS256-based authentication. This allows a remote attacker to execute arbitrary code.

- [https://github.com/unpredictable21/CVE-2026-75431_PowerJob_jwt_key_predictable](https://github.com/unpredictable21/CVE-2026-75431_PowerJob_jwt_key_predictable) :  ![starts](https://img.shields.io/github/stars/unpredictable21/CVE-2026-75431_PowerJob_jwt_key_predictable.svg) ![forks](https://img.shields.io/github/forks/unpredictable21/CVE-2026-75431_PowerJob_jwt_key_predictable.svg)


## CVE-2026-75430
 PowerJob Worker version 5.1.2 (and likely earlier versions) exposes the /worker/deployContainer HTTP endpoint without authentication on the default transport port. This allows a remote attacker to execute arbitrary code.

- [https://github.com/unpredictable21/CVE-2026-75430_PowerJob_worker_deployContainer_RCE](https://github.com/unpredictable21/CVE-2026-75430_PowerJob_worker_deployContainer_RCE) :  ![starts](https://img.shields.io/github/stars/unpredictable21/CVE-2026-75430_PowerJob_worker_deployContainer_RCE.svg) ![forks](https://img.shields.io/github/forks/unpredictable21/CVE-2026-75430_PowerJob_worker_deployContainer_RCE.svg)


## CVE-2026-75429
 PowerJob versions 4.x through 5.1.2 contain an unauthenticated remote code execution vulnerability in the /friend/process endpoint of the Server-Worker transport layer

- [https://github.com/unpredictable21/CVE-2026-75429_PowerJob_friend_process_RCE](https://github.com/unpredictable21/CVE-2026-75429_PowerJob_friend_process_RCE) :  ![starts](https://img.shields.io/github/stars/unpredictable21/CVE-2026-75429_PowerJob_friend_process_RCE.svg) ![forks](https://img.shields.io/github/forks/unpredictable21/CVE-2026-75429_PowerJob_friend_process_RCE.svg)


## CVE-2026-73570
 A remote code execution vulnerability exists in Zimbra Collaboration (ZCS) before 10.1.20 when the optional zimbra-snmp package is installed and SNMP notifications are enabled. Due to improper sanitization of untrusted input during SNMP notification processing, an unauthenticated attacker can send specially crafted SMTP requests that may result in execution of arbitrary operating system commands as the Zimbra user.

- [https://github.com/dahnutz/zimbra-cve-2026-73570-ir](https://github.com/dahnutz/zimbra-cve-2026-73570-ir) :  ![starts](https://img.shields.io/github/stars/dahnutz/zimbra-cve-2026-73570-ir.svg) ![forks](https://img.shields.io/github/forks/dahnutz/zimbra-cve-2026-73570-ir.svg)


## CVE-2026-64468
context in those paths.

- [https://github.com/aramosf/CVE-2026-64468](https://github.com/aramosf/CVE-2026-64468) :  ![starts](https://img.shields.io/github/stars/aramosf/CVE-2026-64468.svg) ![forks](https://img.shields.io/github/forks/aramosf/CVE-2026-64468.svg)


## CVE-2026-63077
 In JetBrains TeamCity before 2026.1.3, 2025.11.7 unauthenticated remote code execution was possible via the agent polling protocol

- [https://github.com/0xCyp1337/CVE-2026-63077](https://github.com/0xCyp1337/CVE-2026-63077) :  ![starts](https://img.shields.io/github/stars/0xCyp1337/CVE-2026-63077.svg) ![forks](https://img.shields.io/github/forks/0xCyp1337/CVE-2026-63077.svg)


## CVE-2026-48019
 Laravel is a web application framework. Prior to versions 12.60.0 and 13.10.0, a CRLF injection vulnerability in Laravel's email validation, in combination with how Symfony Mailer and Symfony Mime handle certain character sequences, may allow an unauthenticated attacker to interfere with outbound email processing in applications that send mail to user-supplied addresses. This issue has been patched in versions 12.60.0 and 13.10.0.

- [https://github.com/derrickschoen/laravel-framework](https://github.com/derrickschoen/laravel-framework) :  ![starts](https://img.shields.io/github/stars/derrickschoen/laravel-framework.svg) ![forks](https://img.shields.io/github/forks/derrickschoen/laravel-framework.svg)


## CVE-2026-44402
 Voltronic Power SNMP Web Pro 1.1 contains an unauthenticated remote code execution vulnerability in the upload.cgi firmware update endpoint that allows remote attackers to execute arbitrary commands as root by uploading a crafted tar archive without valid credentials. Attackers can supply a malicious tar archive containing arbitrary executable files that are extracted to a privileged directory and executed as root, achieving full system compromise.

- [https://github.com/Virgula0/CVE-2026-44402](https://github.com/Virgula0/CVE-2026-44402) :  ![starts](https://img.shields.io/github/stars/Virgula0/CVE-2026-44402.svg) ![forks](https://img.shields.io/github/forks/Virgula0/CVE-2026-44402.svg)


## CVE-2026-43499
  	changelog ]

- [https://github.com/rsyzee/ghostlock-infinix-hot70](https://github.com/rsyzee/ghostlock-infinix-hot70) :  ![starts](https://img.shields.io/github/stars/rsyzee/ghostlock-infinix-hot70.svg) ![forks](https://img.shields.io/github/forks/rsyzee/ghostlock-infinix-hot70.svg)


## CVE-2026-41901
 Thymeleaf is a server-side Java template engine for web and standalone environments. Prior to 3.1.5.RELEASE, a security bypass vulnerability exists in the expression execution mechanisms of Thymeleaf. Although the library provides mechanisms to avoid the execution of potentially dangerous expressions in some specific sandboxed (restricted) contexts, it fails to properly neutralize specific constructs that allow this kind of expressions to be executed. If an application developer passes to the template engine unsanitized variables that contain such expressions, and these values are used in sandboxed contexts inside the templates, these expressions can be executed achieving Server-Side Template Injection (SSTI). This vulnerability is fixed in 3.1.5.RELEASE.

- [https://github.com/xiaoqiMikko/thymeleaf-check](https://github.com/xiaoqiMikko/thymeleaf-check) :  ![starts](https://img.shields.io/github/stars/xiaoqiMikko/thymeleaf-check.svg) ![forks](https://img.shields.io/github/forks/xiaoqiMikko/thymeleaf-check.svg)


## CVE-2026-40477
 Thymeleaf is a server-side Java template engine for web and standalone environments. Versions 3.1.3.RELEASE and prior contain a security bypass vulnerability in the expression execution mechanisms. Although the library provides mechanisms to prevent expression injection, it fails to properly restrict the scope of accessible objects, allowing specific potentially sensitive objects to be reached from within a template. If an application developer passes unvalidated user input directly to the template engine, an unauthenticated remote attacker can bypass the library's protections to achieve Server-Side Template Injection (SSTI). This issue has ben fixed in version 3.1.4.RELEASE.

- [https://github.com/xiaoqiMikko/thymeleaf-check](https://github.com/xiaoqiMikko/thymeleaf-check) :  ![starts](https://img.shields.io/github/stars/xiaoqiMikko/thymeleaf-check.svg) ![forks](https://img.shields.io/github/forks/xiaoqiMikko/thymeleaf-check.svg)


## CVE-2026-34197
Users are recommended to upgrade to version 5.19.4 or 6.2.3, which fixes the issue

- [https://github.com/nirvanasec/CVE-2026-34197-PoC](https://github.com/nirvanasec/CVE-2026-34197-PoC) :  ![starts](https://img.shields.io/github/stars/nirvanasec/CVE-2026-34197-PoC.svg) ![forks](https://img.shields.io/github/forks/nirvanasec/CVE-2026-34197-PoC.svg)


## CVE-2026-33475
- `.github/workflows/typescript_test.yml`

- [https://github.com/pvharmo2/gha-lab-9b5e3ccfbe](https://github.com/pvharmo2/gha-lab-9b5e3ccfbe) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-9b5e3ccfbe.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-9b5e3ccfbe.svg)


## CVE-2026-33075
 FastGPT is an AI Agent building platform. In versions 4.14.8.3 and below, the fastgpt-preview-image.yml workflow is vulnerable to arbitrary code execution and secret exfiltration by any external contributor. It uses pull_request_target (which runs with access to repository secrets) but checks out code from the pull request author's fork, then builds and pushes Docker images using attacker-controlled Dockerfiles. This also enables a supply chain attack via the production container registry. A patch was not available at the time of publication.

- [https://github.com/pvharmo2/gha-lab-61c59f4acb](https://github.com/pvharmo2/gha-lab-61c59f4acb) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-61c59f4acb.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-61c59f4acb.svg)


## CVE-2026-31852
 Jellyfin is an open-source media system. The code-quality.yml GitHub Actions workflow in jellyfin/jellyfin-ios is vulnerable to arbitrary code execution via pull requests from forked repositories. Due to the workflow's elevated permissions (nearly all write permissions), this vulnerability enables full repository takeover of jellyfin/jellyfin-ios, exfiltration of highly privileged secrets, Apple App Store supply chain attack, GitHub Container Registry (ghcr.io) package poisoning, and full jellyfin organization compromise via cross-repository token usage. Note: This is not a code vulnerability, but a vulnerability in the GitHub Actions workflows. No new version is required for this GHSA and end users do not need to take any actions.

- [https://github.com/pvharmo2/gha-lab-3f1ff30e9c](https://github.com/pvharmo2/gha-lab-3f1ff30e9c) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-3f1ff30e9c.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-3f1ff30e9c.svg)


## CVE-2026-31787
This is XSA-487 / CVE-2026-31787

- [https://github.com/0xAtharv/CVE-2026-31787](https://github.com/0xAtharv/CVE-2026-31787) :  ![starts](https://img.shields.io/github/stars/0xAtharv/CVE-2026-31787.svg) ![forks](https://img.shields.io/github/forks/0xAtharv/CVE-2026-31787.svg)


## CVE-2026-29075
 Mesa is an open-source Python library for agent-based modeling, simulating complex systems and exploring emergent behaviors. In version 3.5.0 and prior, checking out of untrusted code in benchmarks.yml workflow may lead to code execution in privileged runner. This issue has been patched via commit c35b8cd.

- [https://github.com/pvharmo2/gha-lab-ca4fa82ac5](https://github.com/pvharmo2/gha-lab-ca4fa82ac5) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-ca4fa82ac5.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-ca4fa82ac5.svg)


## CVE-2026-27941
 OpenLIT is an open source platform for AI engineering. Prior to version 1.37.1, several GitHub Actions workflows in OpenLIT's GitHub repository use the `pull_request_target` event while checking out and executing untrusted code from forked pull requests. These workflows run with the security context of the base repository, including a write-privileged `GITHUB_TOKEN` and numerous sensitive secrets (API keys, database/vector store tokens, and a Google Cloud service account key). Version 1.37.1 contains a fix.

- [https://github.com/pvharmo2/gha-lab-6c3094af9e](https://github.com/pvharmo2/gha-lab-6c3094af9e) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-6c3094af9e.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-6c3094af9e.svg)


## CVE-2026-27938
 WPGraphQL provides a GraphQL API for WordPress sites. Prior to version 2.9.1, the `wp-graphql/wp-graphql` repository contains a GitHub Actions workflow (`release.yml`) vulnerable to OS command injection through direct use of `${{ github.event.pull_request.body }}` inside a `run:` shell block. When a pull request from `develop` to `master` is merged, the PR body is injected verbatim into a shell command, allowing arbitrary command execution on the Actions runner. Version 2.9.1 contains a fix for the vulnerability.

- [https://github.com/pvharmo2/gha-lab-a7f6217d26](https://github.com/pvharmo2/gha-lab-a7f6217d26) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-a7f6217d26.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-a7f6217d26.svg)


## CVE-2026-27701
 LiveCode is an open-source, client-side code playground. Prior to commit e151c64c2bd80d2d53ac1333f1df9429fe6a1a11, LiveCode's `i18n-update-pull` GitHub Actions workflow is vulnerable to JavaScript injection. The title of the Pull Request associated with the triggering issue comment is interpolated directly into a `actions/github-script` JavaScript block using a GitHub Actions template expression. An attacker who opens a PR with a crafted title can inject arbitrary JavaScript that executes with the privileges of the CI bot token (`CI_APP_ID` / `CI_APP_PRIVATE_KEY`), enabling exfiltration of repository secrets and unauthorized GitHub API operations. Commit e151c64c2bd80d2d53ac1333f1df9429fe6a1a11 fixes the issue.

- [https://github.com/pvharmo2/gha-lab-25b7988758](https://github.com/pvharmo2/gha-lab-25b7988758) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-25b7988758.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-25b7988758.svg)


## CVE-2026-25524
 Magento Long Term Support (LTS) is an unofficial, community-driven project provides an alternative to the Magento Community Edition e-commerce platform with a high level of backward compatibility. Prior to version 20.17.0, PHP functions such as `getimagesize()`, `file_exists()`, and `is_readable()` can trigger deserialization when processing `phar://` stream wrapper paths. OpenMage LTS uses these functions with potentially controllable file paths during image validation and media handling. An attacker who can upload a malicious phar file (disguised as an image) and trigger one of these functions with a `phar://` path can achieve arbitrary code execution. Version 20.17.0 patches the issue.

- [https://github.com/Emily-0309/unit-01-severity-vs-risk-reflection](https://github.com/Emily-0309/unit-01-severity-vs-risk-reflection) :  ![starts](https://img.shields.io/github/stars/Emily-0309/unit-01-severity-vs-risk-reflection.svg) ![forks](https://img.shields.io/github/forks/Emily-0309/unit-01-severity-vs-risk-reflection.svg)


## CVE-2026-25514
 FacturaScripts is open-source enterprise resource planning and accounting software. Prior to version 2025.81, FacturaScripts contains a critical SQL injection vulnerability in the autocomplete functionality that allows authenticated attackers to extract sensitive data from the database including user credentials, configuration settings, and all stored business data. The vulnerability exists in the CodeModel::all() method where user-supplied parameters are directly concatenated into SQL queries without sanitization or parameterized binding. This issue has been patched in version 2025.81.

- [https://github.com/Emily-0309/Unit-01-severity-vs-risk-reflection.md](https://github.com/Emily-0309/Unit-01-severity-vs-risk-reflection.md) :  ![starts](https://img.shields.io/github/stars/Emily-0309/Unit-01-severity-vs-risk-reflection.md.svg) ![forks](https://img.shields.io/github/forks/Emily-0309/Unit-01-severity-vs-risk-reflection.md.svg)


## CVE-2026-25057
 MarkUs is a web application for the submission and grading of student assignments. Prior to 2.9.1, instructors are able to upload a zip file to create an assignment from an exported configuration (courses/:course_id/assignments/upload_config_files). The uploaded zip file entry names are used to create paths to write files to disk without checking these paths. This vulnerability is fixed in 2.9.1.

- [https://github.com/ibrah-m/CVE-2026-25057](https://github.com/ibrah-m/CVE-2026-25057) :  ![starts](https://img.shields.io/github/stars/ibrah-m/CVE-2026-25057.svg) ![forks](https://img.shields.io/github/forks/ibrah-m/CVE-2026-25057.svg)


## CVE-2026-24480
 QGIS is a free, open source, cross platform geographical information system (GIS) The repository contains a GitHub Actions workflow called "pre-commit checks" that, before commit 76a693cd91650f9b4e83edac525e5e4f90d954e9, was vulnerable to remote code execution and repository compromise because it used the `pull_request_target` trigger and then checked out and executed untrusted pull request code in a privileged context. Workflows triggered by `pull_request_target` ran with the base repository's credentials and access to secrets. If these workflows then checked out and executed code from the head of an external pull request (which could have been attacker controlled), the attacker could have executed arbitrary commands with elevated privileges. This insecure pattern has been documented as a security risk by GitHub and security researchers. Commit 76a693cd91650f9b4e83edac525e5e4f90d954e9 removed the vulnerable code.

- [https://github.com/pvharmo2/gha-lab-b16a4f3554](https://github.com/pvharmo2/gha-lab-b16a4f3554) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-b16a4f3554.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-b16a4f3554.svg)


## CVE-2026-22869
 Eigent is a multi-agent Workforce. A critical security vulnerability in the CI workflow (.github/workflows/ci.yml) allows arbitrary code execution from fork pull requests with repository write permissions. The vulnerable workflow uses pull_request_target trigger combined with checkout of untrusted PR code. An attacker can exploit this to steal credentials, post comments, push code, or create releases.

- [https://github.com/pvharmo2/gha-lab-7927d7d06f](https://github.com/pvharmo2/gha-lab-7927d7d06f) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-7927d7d06f.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-7927d7d06f.svg)


## CVE-2026-19900
 A vulnerability was identified in LB-LINK X-PRO 1.0.22-20231206. The impacted element is an unknown function of the file /etc/shadow. The manipulation leads to hard-coded credentials. It is possible to initiate the attack remotely. A high degree of complexity is needed for the attack. The exploitability is regarded as difficult. The exploit is publicly available and might be used. The vendor was contacted early about this disclosure but did not respond in any way.

- [https://github.com/on3sk-0x1/cve-2026-19900-PoC](https://github.com/on3sk-0x1/cve-2026-19900-PoC) :  ![starts](https://img.shields.io/github/stars/on3sk-0x1/cve-2026-19900-PoC.svg) ![forks](https://img.shields.io/github/forks/on3sk-0x1/cve-2026-19900-PoC.svg)


## CVE-2026-19632
 The TranslatePress – Translate Multilingual sites with AI Translation plugin for WordPress is vulnerable to Sensitive Information Exposure in all versions up to, and including, 3.3.1 via the 'trp_get_translations_regular' AJAX action. This makes it possible for unauthenticated attackers to extract the raw administrator password-reset URL — including the plaintext reset key and login parameters stored in the translation dictionary table — enabling full administrator account takeover. This vulnerability is only exploitable when automatic string saving is enabled (the default setting) and the target administrator's profile locale is set to a published secondary language, as these conditions cause the password-reset URL to be persisted as a translatable string in the secondary-language dictionary table.

- [https://github.com/ghostpels/CVE-2026-19632](https://github.com/ghostpels/CVE-2026-19632) :  ![starts](https://img.shields.io/github/stars/ghostpels/CVE-2026-19632.svg) ![forks](https://img.shields.io/github/forks/ghostpels/CVE-2026-19632.svg)


## CVE-2026-19516
 A caller-supplied X-Grafana-URL request header controls the destination of mcp-grafana's outbound requests, and the grafana_api_request tool lets the caller also choose the HTTP method, path, and body. Because the destination is not restricted to the configured Grafana instance, a caller can direct requests at internal, loopback, and link-local network services (including metadata endpoints) and read the responses, resulting in server-side request forgery. The fix for CVE-2026-15583 prevented the configured service-account token from being sent to unintended destinations but did not restrict the destinations themselves.

- [https://github.com/HORKimhab/CVE-2026-19516](https://github.com/HORKimhab/CVE-2026-19516) :  ![starts](https://img.shields.io/github/stars/HORKimhab/CVE-2026-19516.svg) ![forks](https://img.shields.io/github/forks/HORKimhab/CVE-2026-19516.svg)


## CVE-2026-11613
 The Divi Ajax Filter plugin for WordPress is vulnerable to Local File Inclusion in all versions up to, and including, 5.1.2 via the 'custom_loop_template' parameter parameter. This makes it possible for unauthenticated attackers to include and execute arbitrary .php files on the server, allowing the execution of any PHP code in those files. This can be used to bypass access controls, obtain sensitive data, or achieve code execution in cases where .php file types can be uploaded and included. This vulnerability is only exploitable when the loop_templates parameter is set to 'custom-template'.

- [https://github.com/Wayang1337/CVE-2026-11613](https://github.com/Wayang1337/CVE-2026-11613) :  ![starts](https://img.shields.io/github/stars/Wayang1337/CVE-2026-11613.svg) ![forks](https://img.shields.io/github/forks/Wayang1337/CVE-2026-11613.svg)


## CVE-2026-10134
 IBM Langflow OSS 1.0.0 through 1.9.3 allows an attacker to read every secret available to the Langflow process, read and modify every flow, conversation, message, file upload, and saved component in the Langflow database, can connect to internal services, abuse cloud metadata endpoints, laterally move to other tenants on the same Langflow instance, and Establish persistence by modifying the public flow's `tool_code` so normal `/api/v1/build/...` calls by any user re-execute attacker code at each build.

- [https://github.com/rmhowe425/POC-CVE-2026-10134](https://github.com/rmhowe425/POC-CVE-2026-10134) :  ![starts](https://img.shields.io/github/stars/rmhowe425/POC-CVE-2026-10134.svg) ![forks](https://img.shields.io/github/forks/rmhowe425/POC-CVE-2026-10134.svg)


## CVE-2026-7355
 Use after free in Media in Google Chrome prior to 147.0.7727.138 allowed a remote attacker to execute arbitrary code inside a sandbox via a crafted HTML page. (Chromium security severity: Medium)

- [https://github.com/HORKimhab/CVE-2026-73554](https://github.com/HORKimhab/CVE-2026-73554) :  ![starts](https://img.shields.io/github/stars/HORKimhab/CVE-2026-73554.svg) ![forks](https://img.shields.io/github/forks/HORKimhab/CVE-2026-73554.svg)


## CVE-2026-6471
 Missing authorization in PostgreSQL logical decoding allows a non-superuser holding REPLICATION privilege to dlopen any file visible to the operating system account running the server, via the choice of logical decoding plugin.  This in turn runs arbitrary code as that account.  Versions before PostgreSQL 18.6, 17.11, 16.15, 15.19, and 14.24 are affected.

- [https://github.com/HORKimhab/CVE-2026-6471](https://github.com/HORKimhab/CVE-2026-6471) :  ![starts](https://img.shields.io/github/stars/HORKimhab/CVE-2026-6471.svg) ![forks](https://img.shields.io/github/forks/HORKimhab/CVE-2026-6471.svg)


## CVE-2026-4349
 A vulnerability was determined in Duende IdentityServer4 up to 4.1.2. The affected element is an unknown function of the file /connect/authorize of the component Token Renewal Endpoint. This manipulation of the argument id_token_hint causes improper authentication. It is possible to initiate the attack remotely. The attack is considered to have high complexity. The exploitability is described as difficult. This vulnerability only affects products that are no longer supported by the maintainer.

- [https://github.com/zychen027/CVE-2026-43499_HW-CLT-AL01](https://github.com/zychen027/CVE-2026-43499_HW-CLT-AL01) :  ![starts](https://img.shields.io/github/stars/zychen027/CVE-2026-43499_HW-CLT-AL01.svg) ![forks](https://img.shields.io/github/forks/zychen027/CVE-2026-43499_HW-CLT-AL01.svg)


## CVE-2026-1699
 In the Eclipse Theia Website repository, the GitHub Actions workflow .github/workflows/preview.yml used pull_request_target trigger while checking out and executing untrusted pull request code. This allowed any GitHub user to execute arbitrary code in the repository's CI environment with access to repository secrets and a GITHUB_TOKEN with extensive write permissions (contents:write, packages:write, pages:write, actions:write). An attacker could exfiltrate secrets, publish malicious packages to the eclipse-theia organization, modify the official Theia website, and push malicious code to the repository.

- [https://github.com/pvharmo2/gha-lab-b5c1313658](https://github.com/pvharmo2/gha-lab-b5c1313658) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-b5c1313658.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-b5c1313658.svg)


## CVE-2025-67727
 Parse Server is an open source backend that can be deployed to any infrastructure that runs Node.js. In versions prior to 8.6.0-alpha.2, a GitHub CI workflow is triggered in a way that grants the GitHub Actions workflow elevated permissions, giving it access to GitHub secrets and write permissions which are defined in the workflow. Code from a fork or lifecycle scripts is potentially included. Only the repository's CI/CD infrastructure is affected, including any public GitHub forks with GitHub Actions enabled. This issue is fixed version 8.6.0-alpha.2 and commits 6b9f896 and e3d27fe.

- [https://github.com/pvharmo2/gha-lab-51c6b6d0a0](https://github.com/pvharmo2/gha-lab-51c6b6d0a0) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-51c6b6d0a0.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-51c6b6d0a0.svg)


## CVE-2025-67303
 An issue in ComfyUI-Manager prior to version 3.38 allowed remote attackers to potentially manipulate its configuration and critical data. This was due to the application storing its files in an insufficiently protected location that was accessible via the web interface

- [https://github.com/1nhann/cm-cve-2025-67303-node](https://github.com/1nhann/cm-cve-2025-67303-node) :  ![starts](https://img.shields.io/github/stars/1nhann/cm-cve-2025-67303-node.svg) ![forks](https://img.shields.io/github/forks/1nhann/cm-cve-2025-67303-node.svg)


## CVE-2025-66478
 This CVE is a duplicate of CVE-2025-55182.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-yarn-workspaces.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-yarn-resolutions.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-patch-package.svg)


## CVE-2025-61584
 serverless-dns is a RethinkDNS resolver that deploys to Cloudflare Workers, Deno Deploy, Fastly, and Fly.io. Versions through abd including 0.1.30 have a vulnerability where the pr.yml GitHub Action interpolates in an unsafe manner untrusted input, specifically the github.event.pull_request.head.repo.clone_url and github.head_ref, to a command in the runner. Due to the action using the pull_request_target trigger it has permissive permissions by default. An unauthorized attacker can exploit this vulnerability to push arbitrary data to the repository. The subsequent impact on the end-user is executing the attackers' code when running serverless-dns. This is fixed in commit c5537dd, and expected to be released in 0.1.31.

- [https://github.com/pvharmo2/gha-lab-6904b2ccbe](https://github.com/pvharmo2/gha-lab-6904b2ccbe) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-6904b2ccbe.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-6904b2ccbe.svg)


## CVE-2025-60800
 Incorrect access control in the /jshERP-boot/user/info interface of jshERP up to commit 90c411a allows attackers to access sensitive information via a crafted GET request.

- [https://github.com/Bob-wentao/jsherp-user-info-idor](https://github.com/Bob-wentao/jsherp-user-info-idor) :  ![starts](https://img.shields.io/github/stars/Bob-wentao/jsherp-user-info-idor.svg) ![forks](https://img.shields.io/github/forks/Bob-wentao/jsherp-user-info-idor.svg)


## CVE-2025-58371
 Roo Code is an AI-powered autonomous coding agent that lives in users' editors. In versions 3.26.6 and below, a Github workflow used unsanitized pull request metadata in a privileged context, allowing an attacker to craft malicious input and achieve Remote Code Execution (RCE) on the Actions runner. The workflow runs with broad permissions and access to repository secrets. It is possible for an attacker to execute arbitrary commands on the runner, push or modify code in the repository, access secrets, and create malicious releases or packages, resulting in a complete compromise of the repository and its associated services. This is fixed in version 3.26.7.

- [https://github.com/pvharmo2/gha-lab-d14c91f1bb](https://github.com/pvharmo2/gha-lab-d14c91f1bb) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-d14c91f1bb.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-d14c91f1bb.svg)


## CVE-2025-54594
 react-native-bottom-tabs is a library of Native Bottom Tabs for React Native. In versions 0.9.2 and below, the github/workflows/release-canary.yml GitHub Actions repository workflow improperly used the pull_request_target event trigger, which allowed for untrusted code from a forked pull request to be executed in a privileged context. An attacker could create a pull request containing a malicious preinstall script in the package.json file and then trigger the vulnerable workflow by posting a specific comment (!canary). This allowed for arbitrary code execution, leading to the exfiltration of sensitive secrets such as GITHUB_TOKEN and NPM_TOKEN, and could have allowed an attacker to push malicious code to the repository or publish compromised packages to the NPM registry. There is a remediation commit which removes github/workflows/release-canary.yml, but a version with this fix has yet to be released.

- [https://github.com/pvharmo2/gha-lab-aa1cbc9bcf](https://github.com/pvharmo2/gha-lab-aa1cbc9bcf) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-aa1cbc9bcf.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-aa1cbc9bcf.svg)


## CVE-2025-54430
 dedupe is a python library that uses machine learning to perform fuzzy matching, deduplication and entity resolution quickly on structured data. Before commit 3f61e79, a critical severity vulnerability has been identified within the .github/workflows/benchmark-bot.yml workflow, where a issue_comment can be triggered using the @benchmark body. This workflow is susceptible to exploitation as it checkout the ${{ github.event.issue.number }}, which correspond to the branch of the PR manipulated by potentially malicious actors, and where untrusted code may be executed. Running untrusted code may lead to the exfiltration of GITHUB_TOKEN, which in this workflow has write permissions on most of the scopes - in particular the contents one - and could lead to potential repository takeover. This is fixed by commit 3f61e79.

- [https://github.com/pvharmo2/gha-lab-ba981941f0](https://github.com/pvharmo2/gha-lab-ba981941f0) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-ba981941f0.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-ba981941f0.svg)


## CVE-2025-54415
 dag-factory is a library for Apache Airflow® to construct DAGs declaratively via configuration files. In versions 0.23.0a8 and below, a high-severity vulnerability has been identified in the cicd.yml workflow within the astronomer/dag-factory GitHub repository. The workflow, specifically when triggered by pull_request_target, is susceptible to exploitation, allowing an attacker to execute arbitrary code within the GitHub Actions runner environment. This misconfiguration enables an attacker to establish a reverse shell, exfiltrate sensitive secrets, including the highly-privileged GITHUB_TOKEN, and ultimately gain full control over the repository. This is fixed in version 0.23.0a9.

- [https://github.com/pvharmo2/gha-lab-f894926966](https://github.com/pvharmo2/gha-lab-f894926966) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-f894926966.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-f894926966.svg)


## CVE-2025-53546
 Folo organizes feeds content into one timeline. Using pull_request_target on .github/workflows/auto-fix-lint-format-commit.yml can be exploited by attackers, since untrusted code can be executed having full access to secrets (from the base repo). By exploiting the vulnerability is possible to exfiltrate GITHUB_TOKEN which has high privileges. GITHUB_TOKEN can be used to completely overtake the repo since the token has content write privileges. This vulnerability is fixed in commit 585c6a591440cd39f92374230ac5d65d7dd23d6a.

- [https://github.com/pvharmo2/gha-lab-6926364d94](https://github.com/pvharmo2/gha-lab-6926364d94) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-6926364d94.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-6926364d94.svg)


## CVE-2025-53104
 gluestack-ui is a library of copy-pasteable components & patterns crafted with Tailwind CSS (NativeWind). Prior to commit e6b4271, a command injection vulnerability was discovered in the discussion-to-slack.yml GitHub Actions workflow. Untrusted discussion fields (title, body, etc.) were directly interpolated into shell commands in a run: block. An attacker could craft a malicious GitHub Discussion title or body (e.g., $(curl ...)) to execute arbitrary shell commands on the Actions runner. This issue has been fixed in commit e6b4271 where the discussion-to-slack.yml workflow was removed. Users should remove the discussion-to-slack.yml workflow if using a fork or derivative of this repository.

- [https://github.com/pvharmo2/gha-lab-3b0a828a69](https://github.com/pvharmo2/gha-lab-3b0a828a69) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-3b0a828a69.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-3b0a828a69.svg)


## CVE-2025-52467
 pgai is a Python library that transforms PostgreSQL into a retrieval engine for RAG and Agentic applications. Prior to commit 8eb3567, the pgai repository was vulnerable to an attack allowing the exfiltration of all secrets used in one workflow. In particular, the GITHUB_TOKEN with write permissions for the repository, allowing an attacker to tamper with all aspects of the repository, including pushing arbitrary code and releases. This issue has been patched in commit 8eb3567.

- [https://github.com/pvharmo2/gha-lab-e8902eccd3](https://github.com/pvharmo2/gha-lab-e8902eccd3) :  ![starts](https://img.shields.io/github/stars/pvharmo2/gha-lab-e8902eccd3.svg) ![forks](https://img.shields.io/github/forks/pvharmo2/gha-lab-e8902eccd3.svg)


## CVE-2025-34158
 Plex Media Server (PMS) 1.41.7.x through 1.42.0.x before 1.42.1 is affected by incorrect resource transfer between spheres because /myplex/account provides the credentials of the server owner (and a /api/resources call reveals other servers accessible by that server owner).

- [https://github.com/HORKimhab/CVE-2025-34158-CVE-2020-5741](https://github.com/HORKimhab/CVE-2025-34158-CVE-2020-5741) :  ![starts](https://img.shields.io/github/stars/HORKimhab/CVE-2025-34158-CVE-2020-5741.svg) ![forks](https://img.shields.io/github/forks/HORKimhab/CVE-2025-34158-CVE-2020-5741.svg)


## CVE-2025-29927
 Next.js is a React framework for building full-stack web applications. Starting in version 1.11.4 and prior to versions 12.3.5, 13.5.9, 14.2.25, and 15.2.3, it is possible to bypass authorization checks within a Next.js application, if the authorization check occurs in middleware. If patching to a safe version is infeasible, it is recommend that you prevent external user requests which contain the x-middleware-subrequest header from reaching your Next.js application. This vulnerability is fixed in 12.3.5, 13.5.9, 14.2.25, and 15.2.3.

- [https://github.com/0xPb1/Next.js-CVE-2025-29927](https://github.com/0xPb1/Next.js-CVE-2025-29927) :  ![starts](https://img.shields.io/github/stars/0xPb1/Next.js-CVE-2025-29927.svg) ![forks](https://img.shields.io/github/forks/0xPb1/Next.js-CVE-2025-29927.svg)
- [https://github.com/lucaschanzx/CVE-2025-29927-PoC](https://github.com/lucaschanzx/CVE-2025-29927-PoC) :  ![starts](https://img.shields.io/github/stars/lucaschanzx/CVE-2025-29927-PoC.svg) ![forks](https://img.shields.io/github/forks/lucaschanzx/CVE-2025-29927-PoC.svg)


## CVE-2025-8518
 A vulnerability was found in givanz Vvveb 1.0.5. It has been rated as critical. Affected by this issue is the function Save of the file admin/controller/editor/code.php of the component Code Editor. The manipulation leads to code injection. The attack may be launched remotely. The exploit has been disclosed to the public and may be used. Upgrading to version 1.0.6 is able to address this issue. The name of the patch is f684f3e374d04db715730fc4796e102f5ebcacb2. It is recommended to upgrade the affected component.

- [https://github.com/HORKimhab/CVE-2025-8518](https://github.com/HORKimhab/CVE-2025-8518) :  ![starts](https://img.shields.io/github/stars/HORKimhab/CVE-2025-8518.svg) ![forks](https://img.shields.io/github/forks/HORKimhab/CVE-2025-8518.svg)


## CVE-2025-6647
The specific flaw exists within the parsing of U3D files. The issue results from the lack of proper validation of user-supplied data, which can result in a write past the end of an allocated object. An attacker can leverage this vulnerability to execute code in the context of the current process. Was ZDI-CAN-26644.

- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-pnpm](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-pnpm) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-pnpm.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-monorepo-nextjs-pnpm.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-bun](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-bun) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-bun.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-bun.svg)
- [https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-packagemanager-field](https://github.com/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-packagemanager-field) :  ![starts](https://img.shields.io/github/stars/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-packagemanager-field.svg) ![forks](https://img.shields.io/github/forks/react2shell-repo-menagerie/CVE-2025-66478-single-nextjs-npm-packagemanager-field.svg)


## CVE-2025-2992
 A vulnerability classified as critical was found in Tenda FH1202 1.2.0.14(408). Affected by this vulnerability is an unknown functionality of the file /goform/AdvSetWrlsafeset of the component Web Management Interface. The manipulation leads to improper access controls. The attack can be launched remotely. The exploit has been disclosed to the public and may be used.

- [https://github.com/all3njk/NextJS_CVE-2025-29927](https://github.com/all3njk/NextJS_CVE-2025-29927) :  ![starts](https://img.shields.io/github/stars/all3njk/NextJS_CVE-2025-29927.svg) ![forks](https://img.shields.io/github/forks/all3njk/NextJS_CVE-2025-29927.svg)
- [https://github.com/enochgitgamefied/NextJS-CVE-2025-29927](https://github.com/enochgitgamefied/NextJS-CVE-2025-29927) :  ![starts](https://img.shields.io/github/stars/enochgitgamefied/NextJS-CVE-2025-29927.svg) ![forks](https://img.shields.io/github/forks/enochgitgamefied/NextJS-CVE-2025-29927.svg)


## CVE-2024-36058
 The Send Basket functionality in Koha Library before 23.05.10 is susceptible to Time-Based SQL Injection because it fails to sanitize the POST parameter bib_list in /cgi-bin/koha/opac-sendbasket.pl, allowing library users to read arbitrary data from the database.

- [https://github.com/hacklantic/CVE-2024-36058](https://github.com/hacklantic/CVE-2024-36058) :  ![starts](https://img.shields.io/github/stars/hacklantic/CVE-2024-36058.svg) ![forks](https://img.shields.io/github/forks/hacklantic/CVE-2024-36058.svg)


## CVE-2024-36057
 Koha Library before 23.05.10 fails to sanitize user-controllable filenames prior to unzipping, leading to remote code execution. The line "qx/unzip $filename -d $dirname/;" in upload-cover-image.pl is vulnerable to command injection via shell metacharacters because input data can be controlled by an attacker and is directly included in a system command, i.e., an attack can occur via malicious filenames after uploading a .zip file and clicking Process Images.

- [https://github.com/hacklantic/CVE-2024-36057](https://github.com/hacklantic/CVE-2024-36057) :  ![starts](https://img.shields.io/github/stars/hacklantic/CVE-2024-36057.svg) ![forks](https://img.shields.io/github/forks/hacklantic/CVE-2024-36057.svg)


## CVE-2022-42889
 Apache Commons Text performs variable interpolation, allowing properties to be dynamically evaluated and expanded. The standard format for interpolation is "${prefix:name}", where "prefix" is used to locate an instance of org.apache.commons.text.lookup.StringLookup that performs the interpolation. Starting with version 1.5 and continuing through 1.9, the set of default Lookup instances included interpolators that could result in arbitrary code execution or contact with remote servers. These lookups are: - "script" - execute expressions using the JVM script execution engine (javax.script) - "dns" - resolve dns records - "url" - load values from urls, including from remote servers Applications using the interpolation defaults in the affected versions may be vulnerable to remote code execution or unintentional contact with remote servers if untrusted configuration values are used. Users are recommended to upgrade to Apache Commons Text 1.10.0, which disables the problematic interpolators by default.

- [https://github.com/gustanini/CVE-2022-42889-Text4Shell-POC](https://github.com/gustanini/CVE-2022-42889-Text4Shell-POC) :  ![starts](https://img.shields.io/github/stars/gustanini/CVE-2022-42889-Text4Shell-POC.svg) ![forks](https://img.shields.io/github/forks/gustanini/CVE-2022-42889-Text4Shell-POC.svg)


## CVE-2022-35499
 In Trimble TM4WEB 21.4.0.4, the external bill viewer endpoint is vulnerable to reflected cross-site scripting via injection in a arbitrary parameter appended to the URL.

- [https://github.com/PN-Tester/CVE-2022-35499](https://github.com/PN-Tester/CVE-2022-35499) :  ![starts](https://img.shields.io/github/stars/PN-Tester/CVE-2022-35499.svg) ![forks](https://img.shields.io/github/forks/PN-Tester/CVE-2022-35499.svg)


## CVE-2022-35497
 In Trimble TM4WEB 21.4.0.4 due to security misconfiguration with session identifiers, it is possible to recover valid session cookies via reflected cross-site scripting affecting the external document viewer endpoint.

- [https://github.com/PN-Tester/CVE-2022-35497](https://github.com/PN-Tester/CVE-2022-35497) :  ![starts](https://img.shields.io/github/stars/PN-Tester/CVE-2022-35497.svg) ![forks](https://img.shields.io/github/forks/PN-Tester/CVE-2022-35497.svg)


## CVE-2022-0847
 A flaw was found in the way the "flags" member of the new pipe buffer structure was lacking proper initialization in copy_page_to_iter_pipe and push_pipe functions in the Linux kernel and could thus contain stale values. An unprivileged local user could use this flaw to write to pages in the page cache backed by read only files and as such escalate their privileges on the system.

- [https://github.com/Greetdawn/CVE-2022-0847-DirtyPipe](https://github.com/Greetdawn/CVE-2022-0847-DirtyPipe) :  ![starts](https://img.shields.io/github/stars/Greetdawn/CVE-2022-0847-DirtyPipe.svg) ![forks](https://img.shields.io/github/forks/Greetdawn/CVE-2022-0847-DirtyPipe.svg)


## CVE-2021-41773
 A flaw was found in a change made to path normalization in Apache HTTP Server 2.4.49. An attacker could use a path traversal attack to map URLs to files outside the directories configured by Alias-like directives. If files outside of these directories are not protected by the usual default configuration "require all denied", these requests can succeed. If CGI scripts are also enabled for these aliased pathes, this could allow for remote code execution. This issue is known to be exploited in the wild. This issue only affects Apache 2.4.49 and not earlier versions. The fix in Apache HTTP Server 2.4.50 was found to be incomplete, see CVE-2021-42013.

- [https://github.com/0xrogg/CVE-2021-41773](https://github.com/0xrogg/CVE-2021-41773) :  ![starts](https://img.shields.io/github/stars/0xrogg/CVE-2021-41773.svg) ![forks](https://img.shields.io/github/forks/0xrogg/CVE-2021-41773.svg)


## CVE-2021-4177
 livehelperchat is vulnerable to Generation of Error Message Containing Sensitive Information

- [https://github.com/mightysai1997/cve-2021-41773](https://github.com/mightysai1997/cve-2021-41773) :  ![starts](https://img.shields.io/github/stars/mightysai1997/cve-2021-41773.svg) ![forks](https://img.shields.io/github/forks/mightysai1997/cve-2021-41773.svg)
- [https://github.com/shiomiyan/CVE-2021-41773](https://github.com/shiomiyan/CVE-2021-41773) :  ![starts](https://img.shields.io/github/stars/shiomiyan/CVE-2021-41773.svg) ![forks](https://img.shields.io/github/forks/shiomiyan/CVE-2021-41773.svg)


## CVE-2020-6950
 Directory traversal in Eclipse Mojarra before 2.3.14 allows attackers to read arbitrary files via the loc parameter or con parameter.

- [https://github.com/TheLonelyCoder/mojarra-2.2.13-patched](https://github.com/TheLonelyCoder/mojarra-2.2.13-patched) :  ![starts](https://img.shields.io/github/stars/TheLonelyCoder/mojarra-2.2.13-patched.svg) ![forks](https://img.shields.io/github/forks/TheLonelyCoder/mojarra-2.2.13-patched.svg)


## CVE-2020-5741
 Deserialization of Untrusted Data in Plex Media Server on Windows allows a remote, authenticated attacker to execute arbitrary Python code.

- [https://github.com/HORKimhab/CVE-2025-34158-CVE-2020-5741](https://github.com/HORKimhab/CVE-2025-34158-CVE-2020-5741) :  ![starts](https://img.shields.io/github/stars/HORKimhab/CVE-2025-34158-CVE-2020-5741.svg) ![forks](https://img.shields.io/github/forks/HORKimhab/CVE-2025-34158-CVE-2020-5741.svg)


## CVE-2020-1938
 When using the Apache JServ Protocol (AJP), care must be taken when trusting incoming connections to Apache Tomcat. Tomcat treats AJP connections as having higher trust than, for example, a similar HTTP connection. If such connections are available to an attacker, they can be exploited in ways that may be surprising. In Apache Tomcat 9.0.0.M1 to 9.0.0.30, 8.5.0 to 8.5.50 and 7.0.0 to 7.0.99, Tomcat shipped with an AJP Connector enabled by default that listened on all configured IP addresses. It was expected (and recommended in the security guide) that this Connector would be disabled if not required. This vulnerability report identified a mechanism that allowed: - returning arbitrary files from anywhere in the web application - processing any file in the web application as a JSP Further, if the web application allowed file upload and stored those files within the web application (or the attacker was able to control the content of the web application by some other means) then this, along with the ability to process a file as a JSP, made remote code execution possible. It is important to note that mitigation is only required if an AJP port is accessible to untrusted users. Users wishing to take a defence-in-depth approach and block the vector that permits returning arbitrary files and execution as JSP may upgrade to Apache Tomcat 9.0.31, 8.5.51 or 7.0.100 or later. A number of changes were made to the default AJP Connector configuration in 9.0.31 to harden the default configuration. It is likely that users upgrading to 9.0.31, 8.5.51 or 7.0.100 or later will need to make small changes to their configurations.

- [https://github.com/lem0n817/tomcatfileread](https://github.com/lem0n817/tomcatfileread) :  ![starts](https://img.shields.io/github/stars/lem0n817/tomcatfileread.svg) ![forks](https://img.shields.io/github/forks/lem0n817/tomcatfileread.svg)

