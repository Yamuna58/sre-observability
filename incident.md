# Incident Report

## What broke

The CI/CD pipeline initially failed during the Docker authentication step, which prevented the build and deployment workflow from completing successfully.

## How I noticed it

The GitHub Actions Build/Deploy workflow reported a failure. After checking the workflow logs, the issue was identified around Docker authentication/credentials.

## The cause

The required Docker credentials/secrets were not correctly configured for the GitHub Actions workflow.

## The fix

The required Docker credentials were configured in the GitHub repository secrets. The workflow was then rerun successfully.

## The follow-up

The Build and Deploy workflows are now green.

A dashboard screenshot has also been added as evidence of the current system status.
