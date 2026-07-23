SAFECOM currently uses Azure DevOps as its primary software development lifecycle platform, with limited GitHub usage primarily supporting vendor collaboration. The existing GitHub environment is not centrally gov-erned; it presents security and operational risks.
This engagement establishes a controlled GitHub Enterprise Cloud foundation through identity-based access, policy enforcement, repository governance, and defined collaboration patterns for internal teams and approved external contributors. The foundation is designed to give SAFECOM stronger control over source code repositories and access lifecycle management while keeping operational change proportionate to the agreed scope.
Beyond the immediate vendor-led repository use cases, SAFECOM has identified potential future internal use cases for the GitHub platform. Internal technical assets, including PowerShell scripts, are currently distributed across network drives, OneDrive locations, and individual user devices. This distributed storage model presents challenges relating to version control, consistency, discoverability, ownership, peer review, and lifecycle man-agement.
The consolidation of these assets into centrally governed GitHub repositories is outside the scope of the current engagement. However, the platform design considers this potential future requirement to ensure that the GitHub Enterprise foundation can support broader internal repository adoption and is not limited to externally driven col-laboration scenarios.

1.3 GitHub Copilot Future Consideration
GitHub Copilot is not part of the current implementation scope. References to Copilot in this design are included only as future-state considerations and as a reason to establish governed repositories, identity controls, access lifecycle management, and security guardrails before any future Copilot assessment or rollout.
Any future Copilot licensing, configuration, policy design, enablement, training, adoption support, or rollout activi-ty would require a separate SAFECOM decision and agreed scope of work. This design does not commit Insight to enabling, configuring, licensing, training users for, or driving adoption of GitHub Copilot under the current en-gagement.

1.4 Recommended Adoption Model
Given SAFECOM’s current operating model and established use of Azure DevOps, a hybrid adoption model is recommended rather than a wholesale migration. Azure DevOps should remain the primary platform for existing work management, delivery pipelines, release processes, and repositories that do not have a clear business or technical driver for migration. Governed GitHub repositories can be introduced selectively where controlled source code management and collaboration provide clear value.
Under this model, source code may be hosted in GitHub while existing Azure DevOps delivery capabilities are re-tained where appropriate. Azure Pipelines supports building, validating, testing, and deploying code held in GitHub repositories, allowing SAFECOM to adopt GitHub incrementally without immediately replacing established delivery processes.
Migration of Azure DevOps repositories, pipelines, boards, or release processes is outside the current engagement. Any future migration should be treated as a separate assessment, business case, design, and delivery activity.






