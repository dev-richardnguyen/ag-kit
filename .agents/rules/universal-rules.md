---
name: universal-rules
version: 1.1.0
priority: P0
trigger: always_on
---

# Universal Rules (TIER 0) - AG Kit

> Always-active rules that apply to every request, regardless of domain.

---

## 🌐 Language Handling

When user's prompt is NOT in English:

1. **Internally translate** for better comprehension
2. **Respond in user's language** - match their communication
3. **Code comments/variables** remain in English

---

## 🏛️ Codebase & Architecture Respect (Global Mandatory)

**ALWAYS respect, align with, and preserve the existing project architecture, conventions, and codebase.**

1. **Discovery Before Creation**: Before writing any new code, you MUST inspect and understand the existing codebase:
   - **UI & Components**: Search for existing UI components, design system elements, and shared widgets before creating new ones.
   - **Hooks & State**: Inspect existing custom hooks, state stores, and context providers.
   - **Themes & Styling**: Strictly use existing theme tokens, color palettes, spacing variables, and typography rules. Never introduce arbitrary or conflicting styles.
   - **Utilities & Helpers**: Discover and reuse existing helper functions, formatters, validators, and API clients.
2. **Reinventing the Wheel is Forbidden**: NEVER write duplicate utilities, one-off styling solutions, or parallel component variants when an existing project abstraction already exists.
3. **Architectural Consistency**: Adhere strictly to the established project patterns (folder structure, naming conventions, error handling, typing paradigms, and data fetching strategies).

---

## 🧹 Clean Code (Global Mandatory)

**ALL code MUST follow `@[skills/clean-code]` rules. No exceptions.**

- **Code**: Concise, direct, no over-engineering. Self-documenting.
- **Testing**: Mandatory. Pyramid (Unit > Int > E2E) + AAA Pattern.
- **Performance**: Measure first. Adhere to current Core Web Vitals standards.
- **Infra/Safety**: 5-Phase Deployment. Verify secrets security.

---
