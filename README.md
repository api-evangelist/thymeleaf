# Thymeleaf

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Thymeleaf is a modern server-side Java template engine for both web and standalone environments, capable of processing HTML, XML, JavaScript, CSS, and plain text. Its primary goal is to bring elegant natural templates to development workflows — HTML pages that can be correctly displayed in browsers as static prototypes while also working as dynamic server-side templates. With deep Spring Framework integration, Thymeleaf 3.1 is the standard view technology for Spring Boot web applications.

- **Human URL:** [https://www.thymeleaf.org/](https://www.thymeleaf.org/)
- **GitHub:** [https://github.com/thymeleaf](https://github.com/thymeleaf)
- **Version:** 3.1.5.RELEASE

## Description

Thymeleaf uses Spring EL for expression evaluation in Spring applications and provides a rich Standard Dialect with `th:*` attribute processors for text substitution, iteration, conditionals, URL generation, form binding, and fragment composition. The extensible dialect system enables integration with Spring Security (via `sec:*` attributes), page layouts, Java 8 time types, and custom processors.

## Links

- [Documentation](https://www.thymeleaf.org/doc/tutorials/3.1/usingthymeleaf.html)
- [Spring Integration Tutorial](https://www.thymeleaf.org/doc/tutorials/3.1/thymeleafspring.html)
- [GitHub Core](https://github.com/thymeleaf/thymeleaf)
- [GitHub Spring](https://github.com/thymeleaf/thymeleaf-spring)
- [Spring Security Extras](https://github.com/thymeleaf/thymeleaf-extras-springsecurity)
- [Issue Tracker](https://github.com/thymeleaf/thymeleaf/issues)
- [Maven](https://mvnrepository.com/artifact/org.thymeleaf/thymeleaf)
- [Spring Boot Starter](https://mvnrepository.com/artifact/org.springframework.boot/spring-boot-starter-thymeleaf)

## APIs / Modules

| Module | Description |
|--------|-------------|
| Thymeleaf Core | Core template engine supporting HTML, XML, TEXT, JavaScript, and CSS template modes |
| Thymeleaf Spring Integration | SpringStandardDialect, SpringTemplateEngine, ThymeleafViewResolver, Spring MVC integration |
| Thymeleaf Extras and Dialects | Spring Security dialect, Java 8 Time dialect, Layout Dialect |

## Maven Quick Start

```xml
<!-- Spring Boot (recommended) -->
<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-starter-thymeleaf</artifactId>
</dependency>

<!-- Standalone Spring 6 -->
<dependency>
  <groupId>org.thymeleaf</groupId>
  <artifactId>thymeleaf-spring6</artifactId>
  <version>3.1.5.RELEASE</version>
</dependency>
```

## Expression Syntax

| Expression | Syntax | Example |
|------------|--------|---------|
| Variable | `${...}` | `${user.name}` |
| Selection | `*{...}` | `*{firstName}` |
| Message | `#{...}` | `#{page.title}` |
| URL | `@{...}` | `@{/users/{id}(id=${user.id})}` |
| Fragment | `~{...}` | `~{footer :: copy}` |

## Artifacts

### JSON Schema

| File | Description |
|------|-------------|
| [thymeleaf-template-schema.json](json-schema/thymeleaf-template-schema.json) | JSON Schema for Thymeleaf engine configuration, dialects, template resolvers, and template metadata |

### JSON Structure

| File | Description |
|------|-------------|
| [thymeleaf-template-structure.json](json-structure/thymeleaf-template-structure.json) | Structural documentation for Thymeleaf configuration models, Standard Dialect attributes, and expression types |

### JSON-LD Context

| File | Description |
|------|-------------|
| [thymeleaf-context.jsonld](json-ld/thymeleaf-context.jsonld) | JSON-LD context mapping Thymeleaf vocabulary to linked data semantics |

### Examples

| File | Description |
|------|-------------|
| [thymeleaf-spring-boot-example.json](examples/thymeleaf-spring-boot-example.json) | Complete Spring Boot integration example with template configuration, form binding, fragment composition, and Spring Security dialect usage |

### Vocabulary

| File | Description |
|------|-------------|
| [thymeleaf-vocabulary.yml](vocabulary/thymeleaf-vocabulary.yml) | Normative vocabulary covering template modes, Standard Dialect attributes, expression types, Spring integration, dialects, and template resolution |

## Tags

HTML, Java, Open Source, Server Side Rendering, Spring, Spring Boot, Template Engine, Thymeleaf, Web Development
