# Contributing to LogiFact 🌊

First off, thank you for being part of the LogiFact Wave! We are building the future of logistics finance, and we’re glad to have you.

## 🛠️ Development Workflow

1. **Claim an Issue:** Browse our [Issues](https://github.com/Bappa-Kamba/LogiFact/issues) and comment on any task. A maintainer will assign it to you.
2. **Fork & Branch:** Create a branch from `main` using the format `feature/LF-[IssueID]-[Task-Name]`.
3. **Strict Standards:**
   - **TypeORM:** Do NOT modify the database directly. All schema changes must be done via TypeORM Entities.
   - **Rust:** All Soroban functions must include `#!no_std` and pass `cargo test`.
   - **Commits:** Use [Conventional Commits](https://www.conventionalcommits.org/).

## 🧪 Testing Requirements
- **Backend:** Ensure `yarn run test` passes.
- **Contracts:** Run `stellar contract build` followed by `cargo test`.
- **UI:** Ensure no Tailwind build errors.

## 📬 Pull Request Process
- Include a screenshot/video for UI changes.
- Link the Issue ID (e.g., `Closes #12`).
- Tag `@Bappa-Kamba` for review.
