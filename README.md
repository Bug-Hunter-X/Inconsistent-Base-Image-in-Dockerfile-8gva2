# Inconsistent Base Image in Dockerfile

This repository demonstrates a common error in Dockerfiles: using `ubuntu:latest` as the base image.  This can lead to build inconsistencies as the `latest` tag changes over time.  This repo shows the problem and a solution.

**Problem:** The original `Dockerfile` uses `ubuntu:latest`, which is a moving target. This can result in build failures or unexpected behavior as new versions of Ubuntu are released.

**Solution:** The `Dockerfile.fixed` uses a specific version of Ubuntu, ensuring consistent builds across different environments.