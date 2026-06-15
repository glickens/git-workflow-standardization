# Git Workflow Standardization and Repository Setup

## Repository Link

https://github.com/glickens/git-workflow-standardization

## Workflow Model

This repository uses the Feature Branch Workflow.

Developers do not commit directly to the main branch. All work is performed in feature branches and merged through Pull Requests after review and approval.

## Branch Naming Convention

Feature branches:

`feature/<feature-name>`

Examples:

feature/login-page

feature/user-authentication

feature/report-generation

Bug fixes:

`bugfix/<bug-name>`

Examples:

bugfix/login-error

bugfix/database-connection

## Commit Message Standards

This project follows Conventional Commits.

Examples:

feat: add login page

feat: create user registration form

fix: resolve database connection issue

docs: update workflow documentation

refactor: simplify validation logic

test: add unit tests for login service

## Merge Approval Process

1. Create a feature branch from main.
2. Implement changes in the feature branch.
3. Commit changes using Conventional Commit messages.
4. Create a Pull Request.
5. At least one approval is required before merging.
6. Direct commits to main are not allowed.
7. Force pushes and branch deletions are restricted.
8. Merge the approved Pull Request into main.

## Branch Protection Rules

The main branch is protected with the following controls:

- Pull Request required before merging
- Minimum of one approval required
- Force pushes blocked
- Branch deletion restricted
- Conversation resolution required before merge

## Purpose

This workflow supports Continuous Integration by enforcing code reviews, protecting the main branch, and encouraging structured collaboration.
