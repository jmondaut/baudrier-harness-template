# Baudrier harness starter

This public repository supplies the starter used by `baudrier setup --starter`. Its `harnesses/example/harness.yaml`
is a Harness Protocol v1 profile with practical shared instructions for an existing project. It declares no
harness-specific skills or subagents; Baudrier installs its capture and conflict skills during setup.

Use GitHub's template action to create your own repository when you are ready to maintain shared instructions.
Edit the copied profile and add skills or subagents only when they serve your project. The GitHub Action in
`.github/workflows/validate.yml` validates each harness on pull requests.

To use your own harness with Baudrier, install the Baudrier GitHub App on that repository and register it in the
Library. See `docs/onboarding.md` in the Baudrier platform repository for the full flow.
