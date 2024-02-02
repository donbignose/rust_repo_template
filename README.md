# Rust Project Template 🦀

This Rust Project Template is designed to provide a comprehensive starting point
for Rust-based projects. It integrates several tools and practices to ensure
code quality, consistency, and security from the outset.

## Features

- **Pre-Commit with Commitizen**: Enforces conventional commit messages ensuring
  a clean and readable commit history.
- **Rustfmt and Clippy**: Ensures code is formatted according to Rust's
  standards and checks for common mistakes and improvements.
- **CI with GitHub Actions**: Automates building, testing, and auditing
  dependencies on every push or pull request.
- **Dependabot Configuration**: Keeps crate dependencies and GitHub Actions
  up-to-date with automated pull requests.

## Getting Started

1. **Clone the Repository**: Start by cloning this template to your local
   machine or use it to initialize your GitHub repository.

```sh
git clone https://github.com/donbignose/rust-project-template.git
```

2. **Install Dependencies**: Make sure you have Rust and Cargo installed. You
   can download them from [rust-lang.org](https://www.rust-lang.org/learn/get-started).

3. **Configure Pre-Commit Hooks**: This template uses pre-commit hooks managed
   by the `pre-commit` tool. Install it following the instructions
   [here](https://pre-commit.com/#install) and set up the hooks with:

```sh
pre-commit install
```

## Usage

- **Developing**: Write your Rust code in the `src/main.rs` file or create new
  modules as needed.
- **Committing Changes**: Use Commitizen for commit messages. Run `git cz`
  instead of `git commit`.
- **Testing and Linting**: Run tests, format your code, and lint it using the
  pre-commit hooks automatically or manually with `cargo test`, `cargo fmt`, and
  `cargo clippy`.
- **GitHub Actions**: The `.github/workflows/ci.yml` file contains the CI
  configuration. It runs on every push and pull request to `main` branch.

## Configuration

- **Commitizen**: Customize commit types, scopes, etc., in the `.cz.toml` file.
- **GitHub Actions**: Modify the CI workflow in `.github/workflows/ci.yml` as
  per your project's requirements.
- **Dependabot**: Adjust the frequency and package-ecosystem in the
  `.github/dependabot.yml`.

## Contributing

Contributions to this Rust Project Template are welcome. Please ensure that your
code adheres to the existing style and that all tests pass.
