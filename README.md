# GitHub Actions Lab - Kashish

## Workflow 1 - Job Dependencies

### Purpose
This workflow demonstrates how jobs can be executed in a specific order using the `needs` keyword.

### Jobs
- Build
- Test
- Deploy

### Key Concepts
- `needs` creates dependencies between jobs
- `runs-on` specifies the operating system runner
- Jobs execute sequentially

---

## Workflow 2 - Multi-Platform Testing

### Purpose
This workflow demonstrates running jobs on multiple operating systems simultaneously.

### Jobs
- ubuntu-job
- windows-job
- macos-job

### Key Concepts
- `runs-on` specifies the operating system
- No `needs` keyword means jobs run in parallel
- `actions/checkout@v4` checks out repository code

---

## Challenges Faced

### Challenge 1
The workflow file was initially placed in `.github` instead of `.github/workflows`.

### Solution
Moved the workflow file into the correct folder.

### Challenge 2
Understanding job dependencies and parallel execution.

### Solution
Used the `needs` keyword for Workflow 1 and removed dependencies in Workflow 2 to allow parallel execution.

---

## Conclusion

This lab demonstrated GitHub Actions workflows, job dependencies, pull request triggers, and multi-platform testing using Ubuntu, Windows, and macOS runners.
