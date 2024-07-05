# Security Policy

We take security seriously, and are committed to prevent and resolve any security problems in a timely and responsible manner.

Our CI/CD pipeline is configured to thoroughly scan the code to find potential software vulnerabilities. The main repository providing the base to setup all source code checks is https://github.com/travelperk/security_pipeline
  * **Secret Scanning** Security step for preventing hardcoded secrets like passwords, and API keys in repositories powered by [gitleaks](https://github.com/gitleaks/gitleaks).

  * **Static Code Analysis (SAST)** Security step for preventing code containing vulnerabilities, misconfigurations, and more from being pushed to main/master branch powered by [semgrep](https://github.com/returntocorp/semgrep). Currenly scanning: (typescript, dockerfile, html, json, kotlin, swift, terraform, yaml)

  * **Infrastructure as Code (IaC) Analysis** Security step for preventing vulnerabilities and missconfigurations in our AWS cloud infrastructure powered by [tfsec](https://github.com/aquasecurity/tfsec). 

  * **Software Composition Analysis (SCA)** Security step for preventing vulnerable software dependencies, and vulnerabilities in Dockerfiles from being pushed to main/master branch powered by [trivy](https://github.com/aquasecurity/trivy)

  * **License Scanning** Security step for preventing non-compliant licensing packages from being pushed to main/master branch powered by [pip-license](https://pypi.org/project/pip-licenses/).

  * **Codeowners** This is a custom pipeline script that checks the existence of the file and if it was updated.

  * **Sync to DefectDojo** This is a custom pipeline script that sends in the background the spotted seciurity issues to our Defect Dojo (DD) vulnerability management platform.
  

Our security protocol follows these industry best practices:

  * Code follows the [OWASP Secure Coding Practices-Quick Reference Guide](https://owasp.org/www-project-secure-coding-practices-quick-reference-guide/)
  * Code also follows the [TK Engineering Security Principles](https://drive.google.com/file/d/1HPUBKZRI52GSmklF_yNbzQgafOe8gV6M/view)
  * Resolve reported vulnerabilities within the SLA's stated [in our policies](https://docs.google.com/document/d/1CbYCn_J3IhOHlaTrtoeRvON7yczJ669LRhJqXqnyjO0/edit).
  * Code follows the internal SDLC guidelines.
