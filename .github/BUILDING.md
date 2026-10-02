# GitHub validation

All project build and validation work runs on GitHub-hosted GitHub Actions
runners. Open **Actions → Hosted content validation → Run workflow** to run
validation manually. The same workflow runs on pushes and pull requests.

The repository currently has only a README and no source or dependency
manifest. CI checks tracked documentation for UTF-8 encoding, a nonempty README,
and Git whitespace errors. It publishes a documentation snapshot as a run
artifact. This is content validation; there is no application build yet.

Inspect the completed workflow and its artifact before reporting success.
Add an appropriate hosted build, security, lint, type-check, and test pipeline
when executable source and its manifest are introduced. Do not fall back to
local builds when Actions is unavailable.
