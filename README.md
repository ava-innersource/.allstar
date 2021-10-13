# .allstar configuration for the Avanade org
> Configuration for Allstar, a security tool produced by the [Open Source Security Foundation](https://openssf.org/).

[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://avanade.github.io/code-of-conduct/)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## Overview
[Allstar](https://github.com/ossf/allstar) is a security-policy GitHub App. It is installed on this org, and this repo contains the configuration for that app. It is configured to create issues on repos that do not comply with the configured policy.


## Configuration

### Enabled Repos

- Apart from branch protection, Allstar is configured on all public repositories, unless a specific opt-out has been granted. [See here for the list of opt-outs](allstar.yaml)
- All opt-outs are at the global level - repositories may not opt out by creating a file in their own repository.
- Allstar is disabled for private repositories
- Feel free to submit a PR to opt a repository out, but please include a brief message explaining why the exclusion is needed.

### Policy Configuration
These are the expected settings to be in compliance:

#### [Branch Protection](branch_protection.yaml)
Branch protection is currently opt-in only, as remediation is required.

| | |
| - | - |
| Branches enforced | default |
| Require approval | yes |
| Approvals required | 1 |
| Dismiss stale reviews | not required |
| Block force push | yes |

#### [Binary Artifacts](binary_artifacts.yaml)

- Binary artifacts are not allowed.

#### [Outside Collaborators](outside.yaml)

- Push access is allowed.
- Admin access is not allowed.

#### [SECURITY.md](security.yaml)

- SECURITY.md is required.

## Licensing
.allstar is available under the [Apache Licence](./LICENSE).

## Contact
Feel free to [raise an issue on GitHub](https://github.com/Avanade/.allstar/issues), or see our [security disclosure](./SECURITY.md) policy.

## Who is Avanade?

[Avanade](https://www.avanade.com) is the leading provider of innovative digital and cloud services, business solutions and design-led experiences on the Microsoft ecosystem, and the power behind the Accenture Microsoft Business Group.
