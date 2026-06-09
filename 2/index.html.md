---
date_published: 2026-05-10
date_modified: 2026-05-10
canonical_url: https://ike.network/index.html
---

# IKE Network

The IKE Network (Integrated Knowledge Exchange) is a sociotechnical fabric where knowledge compounds.

## [#foundation](#foundation)Foundation

The IKE foundation — published to Maven Central and inheritable by any project.

The foundation members fall into two layered orderings. `ike-base-parent` sits at the apex of the **parent** inheritance chain — every other foundation artifact inherits from it. `ike-platform` sits at the terminus of the **build-and-release** dependency chain — releases propagate through it last.

![Build/release dependency order](https://kroki.komet.sh/graphviz/svg/eNqFUstu2zAQvPsrCPXSIBZgx1BaI1APPfUDenOCYCWuZMYUSZCUErfIv2dXVGypl-okzr5mdlaq1oM7isb2RkJU1oi_KyE8mJNUvvz984FeVVtbbX0ZCQ4OPJrIcG07x2WE98iAsRLFIRzBYVnZt7UI8ayxzDxnoVw3SmuU2ZqmmWigo9Av1ANGVcOEBvUHy-2WHpSbpmZf8HtT4J4yPoE7_CZ3d9kTD0XZ0tD_dNxfa4vx41pWBgGFOGioUJeZOmHOSJ40Ppqv6UdYo8832ZJU0zQ73MxI4X2x3WwSqZfQu2XfFxggJ9RZz40H0D2KeHYYblJJtFYvSxhRpk3h14BvcRF-tf5EbtSYUwRNIO9SqrR1WHZiJMWchriMMdJY3803kv9ICg7JQAnhSPaJqUqkrcyUUj6Tnb9HvhddBDCHCzt689yrsAtASOirdJS17kNE_zx0OF6lmA5K2hhRPozI5_bvYVvtIUvgRNRjq7gBSkGqcUB_pnwT-g69qHql5aMhIxQdPobRDJl34E8UdcoEcSscOVArDFPf64VuEsDM5sukEewDdTHQYkdbmpnzz_3ssGiK2f1MCsatvq_eVx-IkS0e) Figure 1. Build/release dependency order 

Members at the same level have no dependency on each other — `ike-tooling` and `ike-workspace-extension` can release in either order or in parallel.

## [#ike-base-parent](#ike-base-parent)IKE Base Parent

[https://central.sonatype.com/artifact/network.ike/ike-base-parent](https://central.sonatype.com/artifact/network.ike/ike-base-parent)[1]

Tier 0 foundation parent for the IKE Network — the apex of the parent inheritance forest, inherited by ike-tooling, ike-docs, and ike-platform. Carries shared publishing metadata, GPG signing, and Maven Central publishing configuration.

| Version | 15 |
| --- | --- |
| Site | [ike.network/ike-base-parent](https://ike.network/ike-base-parent/)[2] |
| GitHub | [IKE-Network/ike-base-parent](https://github.com/IKE-Network/ike-base-parent)[3] |

## [#ike-java-support](#ike-java-support)IKE Java Support

[https://central.sonatype.com/artifact/network.ike/ike-java-support](https://central.sonatype.com/artifact/network.ike/ike-java-support)[4]

Shared, enforced-zero-dependency value types for the IKE Network: ConstantBackedEnum for compiler-visible constants, EnumDefinition for controlled-vocabulary enums, and the ReleasePolicy release-cascade policy ladder. See IKE-Network/ike-issues#498.

| Version | 9 |
| --- | --- |
| Site | [ike.network/ike-java-support](https://ike.network/ike-java-support/)[5] |
| GitHub | [IKE-Network/ike-java-support](https://github.com/IKE-Network/ike-java-support)[6] |

## [#ike-tooling](#ike-tooling)IKE Tooling

[https://central.sonatype.com/artifact/network.ike.tooling/ike-tooling](https://central.sonatype.com/artifact/network.ike.tooling/ike-tooling)[7]

Workspace management, release orchestration, gitflow workflows, and build-time utilities for IKE Network projects.

| Version | 217 |
| --- | --- |
| Site | [ike.network/ike-tooling](https://ike.network/ike-tooling/)[8] |
| GitHub | [IKE-Network/ike-tooling](https://github.com/IKE-Network/ike-tooling)[9] |

#### [#modules](#modules)Modules

- ike-build-standards
- ike-workspace-model
- ike-maven-plugin-support
- ike-maven-plugin

## [#ike-docs](#ike-docs)IKE Docs

[https://central.sonatype.com/artifact/network.ike.docs/ike-docs](https://central.sonatype.com/artifact/network.ike.docs/ike-docs)[10]

Documentation plumbing for the IKE Network. Hosts the ike-doc-maven-plugin (ike-doc packaging, AsciiDoc/render pipeline, PDF dispatch), the Koncept AsciiDoc extension, DocBook XSL + fonts, shared doc resources, and the semantic linebreak reformatter. Split from ike-pipeline to resolve the extensions=true reactor-load cycle. See IKE-Network/ike-issues#216.

| Version | 69 |
| --- | --- |
| Site | [ike.network/ike-docs](https://ike.network/ike-docs/)[11] |
| GitHub | [IKE-Network/ike-docs](https://github.com/IKE-Network/ike-docs)[12] |

#### [#modules_2](#modules_2)Modules

- ike-doc-resources
- minimal-fonts
- docbook-xsl
- koncept-asciidoc-extension
- ike-doc-maven-plugin
- semantic-linebreak
- ike-doc-ingest

## [#ike-workspace-extension](#ike-workspace-extension)IKE Workspace Extension

[https://central.sonatype.com/artifact/network.ike.tooling/ike-workspace-extension](https://central.sonatype.com/artifact/network.ike.tooling/ike-workspace-extension)[13]

Maven 4 build extension that prunes non-existent <subprojects> entries from workspace POMs before model validation. Lets a fresh clone of an IKE workspace bootstrap with mvn ws:scaffold-init before any subproject directory is on disk.

| Version | 9 |
| --- | --- |
| Site | [ike.network/ike-workspace-extension](https://ike.network/ike-workspace-extension/)[14] |
| GitHub | [IKE-Network/ike-workspace-extension](https://github.com/IKE-Network/ike-workspace-extension)[15] |

## [#ike-version-management-extension](#ike-version-management-extension)IKE Version Management Extension

[https://central.sonatype.com/artifact/network.ike.tooling/ike-version-management-extension](https://central.sonatype.com/artifact/network.ike.tooling/ike-version-management-extension)[16]

Maven 4 build extension that implements the IKE typed-marker family for version-property naming: ${groupId*GA*artifactId*VERSION}. Reads *ALIAS properties from the inherited file-model and injects the declared short-name indirections, fails fast on undeclared canonical references, and detects ${G.A} typos with a corrective hint. Accepts the pre-#525 U+00B7 form during the transition. See IKE-Network/ike-issues#470, #472, #525, #526.

| Version | 10 |
| --- | --- |
| Site | [ike.network/ike-version-management-extension](https://ike.network/ike-version-management-extension/)[17] |
| GitHub | [IKE-Network/ike-version-management-extension](https://github.com/IKE-Network/ike-version-management-extension)[18] |

## [#ike-platform](#ike-platform)IKE Platform

[https://central.sonatype.com/artifact/network.ike.platform/ike-platform](https://central.sonatype.com/artifact/network.ike.platform/ike-platform)[19]

Consumer-facing parent POM, BOM, and workspace management plugin for the IKE Network. External doc and code projects inherit from ike-parent (declared here); cross-repo workspace operations use ike-workspace-maven-plugin (ws:* goals). Consumes ike-docs as an external artifact — ike-parent declares ike-doc-maven-plugin with extensions=true, resolving from Nexus at project-load time. Split from the archived ike-pipeline; see IKE-Network/ike-issues#216.

| Version | 100 |
| --- | --- |
| Site | [ike.network/ike-platform](https://ike.network/ike-platform/)[20] |
| GitHub | [IKE-Network/ike-platform](https://github.com/IKE-Network/ike-platform)[21] |

#### [#modules_3](#modules_3)Modules

- ike-parent
- ike-workspace-maven-plugin
- ike-bom

## [#examples](#examples)Examples

Reference projects that show how to consume the IKE foundation. They are deliberately **not** published to Maven Central: they are worked examples to read and copy, not libraries to depend on. Publishing them as artifacts would invite accidental coupling to code that exists only to illustrate a pattern.

## [#ike-documentation-example](#ike-documentation-example)IKE Documentation Example

Documentation-only project demonstrating the IKE AsciiDoc pipeline. Exercises all diagram types, Koncept macros, typography, and layout features across all 6 PDF renderers.

| Version | 33 |
| --- | --- |
| Site | [ike.network/doc-example](https://ike.network/doc-example/)[22] |
| GitHub | [IKE-Network/doc-example](https://github.com/IKE-Network/doc-example)[23] |

## [#hl7-ig-corpus-example](#hl7-ig-corpus-example)HL7 IG Corpus Example

Worked example of the corpus-example pattern — multi-module documentation project that ingests a corpus of HL7 implementation guides into the IKE topic library and produces per-IG assemblies plus cross-IG analytic outputs.

| Version | 1 |
| --- | --- |
| Site | [ike.network/hl7-ig-corpus-example](https://ike.network/hl7-ig-corpus-example/)[24] |
| GitHub | [IKE-Network/hl7-ig-corpus-example](https://github.com/IKE-Network/hl7-ig-corpus-example)[25] |

#### [#modules_4](#modules_4)Modules

- ingest
- topics
- corpus-guide
- compendium
- us-core
- cross-ig-overlap

## [#ike-network_2](#ike-network_2)IKE Network

Organization landing page for IKE Network projects.

| Version | 2 |
| --- | --- |
| Site | [ike.network/ike-network-site](https://ike.network/ike-network-site/)[26] |
| GitHub | [IKE-Network/ike-network-site](https://github.com/IKE-Network/ike-network-site)[27] |

## [#ike-integration-tests-example](#ike-integration-tests-example)IKE Integration Tests Example

End-to-end smoke tests that exercise the IKE Network release cascade as external consumers would. Each IT case clones the intended usage pattern (doc-only project, java + docs, BOM import, ws:create scaffold) in a fresh Maven environment and asserts that the build succeeds and produces the expected artifacts.

| Version | 25 |
| --- | --- |
| Site | [ike.network/integration-tests-example](https://ike.network/integration-tests-example/)[28] |
| GitHub | [IKE-Network/integration-tests-example](https://github.com/IKE-Network/integration-tests-example)[29] |

## [#ike-project-example](#ike-project-example)IKE Project Example

Example Java project demonstrating IKE documentation pipeline integration with Java source, tests, and Koncept macros.

| Version | 33 |
| --- | --- |
| Site | [ike.network/project-example](https://ike.network/project-example/)[30] |
| GitHub | [IKE-Network/project-example](https://github.com/IKE-Network/project-example)[31] |

## [#ike-workspace-reactor-example](#ike-workspace-reactor-example)IKE Workspace Reactor Example

| Version | 24 |
| --- | --- |
| Site | [ike.network/workspace-reactor-example](https://ike.network/workspace-reactor-example/)[32] |
| GitHub | [IKE-Network/workspace-reactor-example](https://github.com/IKE-Network/workspace-reactor-example)[33] |

#### [#modules_5](#modules_5)Modules

- doc-example
- project-example
- integration-tests-example
