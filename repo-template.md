## SOW
1. Up to 2 baseline repository templates configured with standard visibility, permission, and branch protection settings.
2. 6.8 Repository Standard Template

Repository templates should provide a practical starting point for consistent repository creation. Under the current engagement, implementation is limited to up to two templates. Additional templates, language-specific templates, automation, or organisation-wide template adoption should be treated as future scope.

### Essential Files

Essential repository files should include, at minimum, a README, CODEOWNERS where applicable, contribution guidance, and any required security or support notes. The objective is to make ownership and expected ways of working clear from repository creation.

Each repository template should include the following essential files, where applicable.

| File | Purpose | Requirement | Intended Audience |
| --- | --- | --- | --- |
| README.md | Provides the repository overview, purpose, setup instructions, usage guidance and support information. | Required | All stakeholders |
| CODEOWNERS | Identifies the individuals or GitHub teams responsible for reviewing changes to specified files, directories or code areas. | Required | Developers, reviewers and subject matter experts |
| CONTRIBUTING.md | Defines contribution processes, development standards, pull-request requirements and expected ways of working. | Required | Team members and external contributors |
| SECURITY.md | Defines the security policy, vulnerability-reporting process and responsible-disclosure requirements. | Required | Developers, security teams and security researchers |
| .gitignore | Defines technology-specific files and directories that must not be committed to the repository. | Required | Developers |
| LICENSE | Defines the legal terms under which the repository content may be used, modified or distributed. | Required where applicable | Legal, compliance and repository users |
| pull_request_template.md | Provides a standard structure that prompts pull-request authors to describe the change, testing performed, related work items, risks and required checklist items. | Required | Developers, reviewers and repository maintainers |

### Code Ownership

CODEOWNERS should be used to connect repository paths to accountable teams or individuals where practical. For the foundation scope, CODEOWNERS should be kept simple and aligned to the approved team model so pull request review expectations are enforceable without creating unnecessary operational overhead.
Repository templates should include a standard CODEOWNERS file to help repositories created from the template assign appropriate reviewers to different parts of the codebase.
Code owners may be individual subject matter experts or GitHub teams with the knowledge required to review changes to particular files, directories or components.

Code ownership may be assigned to:

- The entire repository
- A specific directory
- A specific file
- Files matching a defined pattern

For example:

- Application specialists may review files under src/.
- DevOps specialists may review files under .github/workflows/.
- Security specialists may review security-related configuration files.
- Infrastructure specialists may review files under infrastructure/ or modules/.

The template should contain placeholder ownership entries that must be updated when a new repository is created.
Where code-owner approval is enforced through GitHub rulesets, pull requests that modify code-owned files or paths must be approved by the relevant code owner before they can be merged.
This ensures that changes are reviewed by individuals or teams with the appropriate knowledge of the affected code or configuration.
