# Contribution Guidelines

Hello! Thanks for your interest in contributing to this project.
Outlined below are the expected guidelines for contributing. Please read
them carefully!

**Note**: This document does not cover things that would belong in a
code of conduct document.

> [!NOTE]
> If you are contributing to a repository that lives on `git.rgst.io`
> (aka `go.rgst.io`), please read the contribution instructions at:
> https://jaredallard.dev/git.

## Table of Contents

<!-- go run sigs.k8s.io/mdtoc@latest --inplace --max-depth=5 CONTRIBUTING.md -->
<!-- toc -->
- [Contributing Code](#contributing-code)
  - [Commit Format](#commit-format)
  - [Pull Request Format](#pull-request-format)
  - [Code Size](#code-size)
  - [Code Style](#code-style)
<!-- /toc -->

## Contributing Code

Code contributions should follow the Github Pull Request model for all
changes, even for contributors with commit access. This means that you
should create a branch in a repo (even if it's your own fork) and create
a pull request from that branch into the main repo.

### Commit Format

Commits should follow the Conventional Commit format[^1]. However,
this is only a strong requirement for the Pull Request title and body,
because we **squash** commits on merge.

### Pull Request Format

We do not provide templates for pull requests because of our nature of
squash and merging using the PR body. A template would muddy each
commit's body. So, feel free to use whatever format you'd like, but we'd
like it to at least contain the following:

- A clear and concise title following conventional commit format[^1]
- A body that clearly explains the 5 W's of the change:
  - **What** is the change?
  - **Why** is the change necessary?
  - **When** should the change be merged?
  - **Who** is the change for?
  - **Where** does the change apply?
  - **This does not need to be a form! Just approach your wording from
    these questions.**
- (Optional, but recommended): 72 character line wrap for the title and
  body.

Some good examples:

- <https://github.com/rgst-io/stencil-golang/commit/676f11ef3925ba6bcf98fba2bfe0391a07aff3b6>
- <https://github.com/getoutreach/devbase/commit/7c4890efd8591442be2f975ef65d6929e31afea8>
- <https://github.com/getoutreach/devbase/commit/5dd66a2ddd23c4ff24a19a72465b89ca96181689>

### Code Size

Please keep pull requests small and focused. If you have a large change
that you'd like to make, likely create an issue to discuss it first but
at the very least, think about how to break it apart into multiple
distinct changes. We're here to help you do that!

### Code Style

All code should be formatted and match the style of code around it.
While we don't have a strong code style guide, we do have automatic
formatters and linters. These can be run with `mise run fmt` and `mise
run lint` respectively.

[^1]: [Conventional Commit](https://www.conventionalcommits.org/en/v1.0.0)
