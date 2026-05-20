---
date_published: 2026-05-10
date_modified: 2026-05-10
canonical_url: https://ike.network/index.html
---

# IKE Network

The IKE Network (Integrated Knowledge Exchange) is a sociotechnical fabric where knowledge compounds.

## [#foundation](#foundation)Foundation

The IKE foundation — published to Maven Central and inheritable by any project. Each layer builds on the one above it.

## [#ike-base-parent](#ike-base-parent)IKE Base Parent

[https://central.sonatype.com/artifact/network.ike/ike-base-parent](https://central.sonatype.com/artifact/network.ike/ike-base-parent)[1]

Tier 0 foundation parent for the IKE Network — the apex of the parent inheritance forest, inherited by ike-tooling, ike-docs, and ike-platform. Carries shared publishing metadata, GPG signing, and Maven Central publishing configuration.

| Version | 3 |
| --- | --- |
| Site | [ike.network/ike-base-parent](https://ike.network/ike-base-parent/)[2] |
| GitHub | [IKE-Network/ike-base-parent](https://github.com/IKE-Network/ike-base-parent)[3] |

## [#ike-tooling](#ike-tooling)IKE Tooling

[https://central.sonatype.com/artifact/network.ike.tooling/ike-tooling](https://central.sonatype.com/artifact/network.ike.tooling/ike-tooling)[4]

Workspace management, release orchestration, gitflow workflows, and build-time utilities for IKE Network projects.

| Version | 190 |
| --- | --- |
| Site | [ike.network/ike-tooling](https://ike.network/ike-tooling/)[5] |
| GitHub | [IKE-Network/ike-tooling](https://github.com/IKE-Network/ike-tooling)[6] |

#### [#modules](#modules)Modules

- ike-build-standards
- ike-java-support
- ike-workspace-model
- ike-maven-plugin-support
- ike-maven-plugin

## [#ike-docs](#ike-docs)IKE Docs

[https://central.sonatype.com/artifact/network.ike.docs/ike-docs](https://central.sonatype.com/artifact/network.ike.docs/ike-docs)[7]

Documentation plumbing for the IKE Network. Hosts the ike-doc-maven-plugin (ike-doc packaging, AsciiDoc/render pipeline, PDF dispatch), the Koncept AsciiDoc extension, DocBook XSL + fonts, shared doc resources, and the semantic linebreak reformatter. Split from ike-pipeline to resolve the extensions=true reactor-load cycle. See IKE-Network/ike-issues#216.

| Version | 47 |
| --- | --- |
| Site | [ike.network/ike-docs](https://ike.network/ike-docs/)[8] |
| GitHub | [IKE-Network/ike-docs](https://github.com/IKE-Network/ike-docs)[9] |

#### [#modules_2](#modules_2)Modules

- ike-doc-resources
- minimal-fonts
- docbook-xsl
- koncept-asciidoc-extension
- ike-doc-maven-plugin
- semantic-linebreak

## [#ike-workspace-extension](#ike-workspace-extension)IKE Workspace Extension

[https://central.sonatype.com/artifact/network.ike.tooling/ike-workspace-extension](https://central.sonatype.com/artifact/network.ike.tooling/ike-workspace-extension)[10]

Maven 4 build extension that prunes non-existent <subprojects> entries from workspace POMs before model validation. Lets a fresh clone of an IKE workspace bootstrap with mvn ws:scaffold-init before any subproject directory is on disk.

| Version | 2 |
| --- | --- |
| Site | [ike.network/ike-workspace-extension](https://ike.network/ike-workspace-extension/)[11] |
| GitHub | [IKE-Network/ike-workspace-extension](https://github.com/IKE-Network/ike-workspace-extension)[12] |

## [#ike-platform](#ike-platform)IKE Platform

[https://central.sonatype.com/artifact/network.ike.platform/ike-platform](https://central.sonatype.com/artifact/network.ike.platform/ike-platform)[13]

Consumer-facing parent POM, BOM, and workspace management plugin for the IKE Network. External doc and code projects inherit from ike-parent (declared here); cross-repo workspace operations use ike-workspace-maven-plugin (ws:* goals). Consumes ike-docs as an external artifact — ike-parent declares ike-doc-maven-plugin with extensions=true, resolving from Nexus at project-load time. Split from the archived ike-pipeline; see IKE-Network/ike-issues#216.

| Version | 77 |
| --- | --- |
| Site | [ike.network/ike-platform](https://ike.network/ike-platform/)[14] |
| GitHub | [IKE-Network/ike-platform](https://github.com/IKE-Network/ike-platform)[15] |

#### [#modules_3](#modules_3)Modules

- ike-parent
- ike-workspace-maven-plugin
- ike-bom

## [#examples](#examples)Examples

Reference projects that show how to consume the IKE foundation. They are deliberately **not** published to Maven Central: they are worked examples to read and copy, not libraries to depend on. Publishing them as artifacts would invite accidental coupling to code that exists only to illustrate a pattern.

## [#ike-documentation-example](#ike-documentation-example)IKE Documentation Example

Documentation-only project demonstrating the IKE AsciiDoc pipeline. Exercises all diagram types, Koncept macros, typography, and layout features across all 6 PDF renderers.

| Version | 31 |
| --- | --- |
| Site | [ike.network/doc-example](https://ike.network/doc-example/)[16] |
| GitHub | [IKE-Network/doc-example](https://github.com/IKE-Network/doc-example)[17] |

## [#ike-example-project](#ike-example-project)IKE Example Project

Example Java project demonstrating IKE documentation pipeline integration with Java source, tests, and Koncept macros.

| Version | 31 |
| --- | --- |
| Site | [ike.network/example-project](https://ike.network/example-project/)[18] |
| GitHub | [IKE-Network/example-project](https://github.com/IKE-Network/example-project)[19] |

## [#ike-example-integration-test-harness](#ike-example-integration-test-harness)IKE Example Integration Test Harness

End-to-end smoke tests that exercise the IKE Network release cascade as external consumers would. Each IT case clones the intended usage pattern (doc-only project, java + docs, BOM import, ws:create scaffold) in a fresh Maven environment and asserts that the build succeeds and produces the expected artifacts.

| Version | 23 |
| --- | --- |
| Site | [ike.network/ike-example-its](https://ike.network/ike-example-its/)[20] |
| GitHub | [IKE-Network/ike-example-its](https://github.com/IKE-Network/ike-example-its)[21] |

## [#ike-example-workspace](#ike-example-workspace)IKE Example Workspace

| Version | 22 |
| --- | --- |
| Site | [ike.network/ike-example-ws](https://ike.network/ike-example-ws/)[22] |
| GitHub | [IKE-Network/ike-example-ws](https://github.com/IKE-Network/ike-example-ws)[23] |

#### [#modules_4](#modules_4)Modules

- doc-example
- example-project
- its
