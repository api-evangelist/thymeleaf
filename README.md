# Thymeleaf

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
