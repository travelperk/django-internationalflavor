# Template repository
Base repository to use for any new repository creation. Feel free to customize the content of the following files to suit your needs.

- **CODEOWNERS:** Add you team ownership objects and code.

- **README:** Add your custom project details.

- **.gitignore:** A file specifies intentionally untracked files that Git should ignore.

- **.circleci:** Files to setup your CI/CD pipelines.

- **.trivyignore:** Indicate to our vulnerability scanner (Trivy) detects unpatched/unfixed vulnerabilities. If you can't fix these vulnerabilities and you would like to ignore them, use this file.

- **.semgrepignore:** Indicate to our static code analysis tool (Semgrep) to ignore some files and folders.

- **.gitleaks.toml:** Indicate to our tool (GitLeaks) that detects hardcoded secrets like passwords, api keys, and tokens, to ignore some files or folders.
