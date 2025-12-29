
```cardlink
url: https://engineering.atspotify.com/2020/8/how-we-use-golden-paths-to-solve-fragmentation-in-our-software-ecosystem?
title: "How We Use Golden Paths to Solve Fragmentation in Our Software Ecosystem | Spotify Engineering"
description: "“His spice-induced visions show him a myriad of possible futures where humanity has become extinct and only one where humanity survives. He names this future ‘The Golden Path’ and resolves to bring it to fruition.”"
host: engineering.atspotify.com
favicon: https://engineering.atspotify.com/favicon.ico
image: https://images.ctfassets.net/p762jor363g1/attachment_cf05b065cf08d49ef915dd17f4eb74a3/d0ace00d0c3c1451b2d56088ae06a29d/attachment_cf05b065cf08d49ef915dd17f4eb74a3.png
```

```cardlink
url: https://www.redhat.com/en/topics/platform-engineering/golden-paths
title: "What is a Golden Path for software development?"
description: "A Golden Path refers to an opinionated, well-documented, and supported way of building and deploying software within an organization."
host: www.redhat.com
favicon: https://www.redhat.com/favicon.ico
image: https://www.redhat.com/profiles/rh/themes/redhatdotcom/img/logo-rh-og-image.png
```



[[The Case Against Golden Paths]]
[[Golden Path or Golden Cage? When Platform Abstractions Go Too Far]]
[[Golden Path vs. Golden Cage in Platform Engineering -  Why Flexibility Matters]]


In an IT engineering platform context, the "paved road, dirty road, jungle" metaphor describes different approaches to software development and infrastructure management, ranging from highly guided and standardized paths to completely unconstrained and unsupported environments.

Paved Road (Golden Path)

The **paved road** (or "golden path") is an opinionated, well-defined, and fully supported path for building and deploying software within an organization. It provides:

- **Standardization**: A curated set of best practices, tools, libraries, and architecture choices that are officially endorsed by the platform team.
- **Efficiency**: Developers can follow clear, documented processes to get their applications from idea to production quickly, reducing cognitive load and boilerplate work.
- **Safety and Compliance**: Security, monitoring, and compliance checks are built-in by default, ensuring that the "right way" of doing things is also the safe and compliant way.
- **Support**: The central platform team maintains the road and provides support for teams using it.
- **Guiderails**: It uses mechanisms like pre-approved infrastructure modules and CI/CD templates to guide developers toward successful outcomes without being overly restrictive.

Dirty Road

The **dirty road** typically refers to deviations from the paved road where some support or guidance might exist, but the path is not as smooth, consistent, or well-maintained.

- It might involve using non-standard tools or configurations that are not fully integrated into the main platform.
- Developers choosing this path take on more responsibility for their infrastructure, support, and compliance, potentially encountering more operational headaches or "potholes" along the way.
- This path is often chosen when a team has specific needs that the paved road doesn't address.

Jungle

The **jungle** represents a completely unconstrained, unsupported environment with no predefined path or standards.

- Developers have complete autonomy to choose any technology, language, or framework they want.
- The primary challenge here is immense complexity, as teams must build everything from scratch, including basic operational tools, security protocols, and monitoring.
- This environment has the highest cognitive load and the greatest risk of fragmentation and technical debt.
- It is generally an anti-pattern for large organizations aiming for efficiency and consistency, though it can be a place for R&D teams to experiment with new technologies that might one day become part of the paved road.