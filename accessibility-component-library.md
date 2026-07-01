# Accessibility Component Library
### Building an accessibility-first design system to prepare for the European Accessibility Act
> **Tech:** React, React Native, TypeScript, Accessibility (WCAG 2.1 AA), Feature Flags, Codemods  
> **Focus:** Design Systems · Accessibility · Developer Experience · Cross-team Leadership

---

## Overview

As part of a company-wide initiative to prepare for the European Accessibility Act, I helped lead the effort to improve accessibility across our web and mobile applications.

Rather than treating accessibility as hundreds of individual bug fixes, we focused on improving the shared UI foundation that every product team depended on. The result was an accessibility-first component library, automated migration tooling, and an adoption strategy that enabled engineering teams to incrementally migrate without disrupting feature development.

The initiative increased audit compliance from **57% to 100%**, enabled the launch of new European products, and established a long-term foundation for building accessible experiences by default.

---

## The Problem

Accessibility issues had accumulated over several years across many independently owned product surfaces.

An external accessibility audit identified hundreds of findings spanning web and React Native applications. While many issues appeared unique, a large percentage originated from inconsistencies in shared UI components.

Examples included:

- inconsistent screen reader behavior
- missing accessibility labels
- incorrect semantic markup
- keyboard navigation issues
- inconsistent focus management
- components that required every product team to implement accessibility themselves

Fixing each issue independently would have required every engineering team to solve the same problems repeatedly while introducing inconsistent behavior across the product.

---

## Goals

Our goals extended beyond passing an accessibility audit.

We wanted to:

- build reusable accessible components
- make accessible implementations the default rather than optional
- minimize disruption to product teams
- support incremental adoption
- reduce future accessibility regressions
- establish a long-term accessibility foundation

---

## My Role

Initially, I partnered with a Staff Engineer to build the shared component library and define the overall migration strategy.

Midway through the initiative, the Staff Engineer transitioned to another high-priority project. I became responsible for driving much of the remaining implementation while onboarding another engineer who joined the project later.

Beyond implementation, I worked closely with engineers across multiple product teams by:

- consulting on accessibility issues
- reviewing migration plans
- answering implementation questions
- writing technical documentation
- helping prioritize remediation work
- identifying reusable accessibility patterns

---

## Solution

Instead of fixing accessibility issues one screen at a time, we invested in improving the shared foundation.

The strategy centered around four major pieces:

### 1. Accessibility-first components

We redesigned commonly used UI components so that accessible behavior became the default experience.

This included improvements around:

- semantic HTML
- keyboard interactions
- screen reader support
- focus management
- accessible naming
- consistent interaction patterns

---

### 2. Consistent component APIs

Many legacy components exposed different APIs despite solving similar problems.

As new components were introduced, we designed more consistent APIs that reduced implementation complexity while encouraging accessible usage patterns.

Rather than relying on documentation alone, the component APIs themselves guided developers toward correct implementations.

---

### 3. Automated migrations

Migrating hundreds of component usages manually would have required significant engineering effort.

To reduce migration cost, we built codemods that automatically transformed many existing component usages into the new APIs.

This allowed teams to migrate substantially faster while reducing manual errors.

---

### 4. Incremental rollout

Replacing shared UI components across many products carried significant risk.

We introduced feature flags to support gradual adoption, allowing individual teams to validate changes safely before broader rollout.

This approach reduced deployment risk while enabling teams to continue shipping product work throughout the migration.

---

## Technical Decisions

### Shared components over one-off fixes

Although fixing individual accessibility issues would have produced short-term progress, many findings shared common root causes.

Investing in reusable components ensured future product development inherited accessible behavior by default instead of repeatedly solving the same problems.

---

### Codemods over manual migrations

The migration affected a large number of existing component usages.

Automating repetitive transformations significantly reduced engineering effort while making adoption more consistent across teams.

---

### Feature flags over large releases

Rolling out foundational UI changes incrementally reduced operational risk and allowed teams to validate behavior in production before wider adoption.

---

## Challenges

### Learning before the audit finished

While waiting for the external accessibility audit to complete, I spent time learning accessibility standards, tooling, and common implementation patterns so we could begin remediation work immediately.

---

### Scaling across many teams

Different engineering teams owned different parts of the application.

Success depended less on writing code and more on enabling other engineers through documentation, consultation, and reusable abstractions.

---

### Balancing consistency with flexibility

Shared components needed to support many product use cases without becoming overly configurable.

Finding the right API surface required balancing developer ergonomics, accessibility requirements, and long-term maintainability.

---

## Results

- Increased accessibility compliance from **57% to 100%**
- Enabled launch of two new European products
- Resolved hundreds of accessibility findings
- Reduced duplicated implementation effort across engineering teams
- Established reusable accessibility patterns for future development
- Automated significant portions of the migration through codemods

---

## Lessons Learned

The most valuable outcome wasn't simply fixing accessibility issues—it was changing how engineers built software.

By investing in shared components, migration tooling, and developer education, accessibility became part of the development workflow rather than a separate remediation effort.

This project reinforced my belief that the highest-leverage engineering work often comes from improving the systems that enable other engineers to move faster while producing more consistent, higher-quality software.
