# Action Stars Build Workflows for GitHub Actions

![GitHub Release (latest SemVer)](https://img.shields.io/github/v/release/action-stars/build-workflows?sort=semver)
![Validate](https://github.com/action-stars/build-workflows/actions/workflows/_validate.yaml/badge.svg?branch=main)

This repository contains a collection of GitHub Actions workflows for building and testing various types of projects. The workflows are designed to be used as-is or as a starting point for your own projects.

## Build OCI Image

This workflow builds a Docker image and pushes it to an OCI registry.

<!-- MERGE:START:build-oci-image - Do not remove or modify this section -->
### Inputs

<!-- AUTO-DOC-INPUT:START - Do not remove or modify this section -->

|       INPUT       |  TYPE   | REQUIRED |           DEFAULT           |                                                                                          DESCRIPTION                                                                                          |
|-------------------|---------|----------|-----------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|    annotations    | string  |  false   |                             |                                                Annotations to apply to the manifest image; as multi-line values in the format `<key>=<value>`.                                                |
| artifacts_pattern | string  |  false   |                             | Pattern to match artifacts that should be downloaded to be used for image building. The path where these artifacts are downloaded to is available in the `WORKFLOW_ARTIFACTS` build argument. |
|      context      | string  |  false   |            `"."`            |                                                                          Path to the context to build the image in.                                                                           |
|    dockerfile     | string  |   true   |                             |                                                                               Path to the Dockerfile to build.                                                                                |
|      labels       | string  |  false   |                             |                                                       Labels to apply to the image; as multi-line values in the format `<key>=<value>`.                                                       |
|       name        | string  |   true   |                             |                                                                                  Name of the image to build.                                                                                  |
|     platforms     | string  |  false   | `"linux/amd64,linux/arm64"` |                                                                 Platforms to build the image for; as comma separated values.                                                                  |
|    push_image     | boolean |  false   |           `true`            |                                                                          Whether to push the image to the registry.                                                                           |
|    push_sarif     | boolean |  false   |           `true`            |                                                                     Whether to push the SARIF files for GitHub Security.                                                                      |
|     push_sbom     | boolean |  false   |           `true`            |                                                                 Whether to push the SBOM to the GitHub dependency submission.                                                                 |
|    repository     | string  |   true   |                             |                                                                          The GHCR repository to build the image in.                                                                           |
|    scan_image     | boolean |  false   |           `true`            |                                                                             Whether to scan the image with Grype.                                                                             |
|       tags        | string  |  false   |                             |                               Tags to apply to the image; as comma separated values. If no tags are provided then a tag will be created from the Git short SHA.                               |

<!-- AUTO-DOC-INPUT:END -->
### Outputs

<!-- AUTO-DOC-OUTPUT:START - Do not remove or modify this section -->

|      OUTPUT      |                   DESCRIPTION                    |
|------------------|--------------------------------------------------|
|      digest      |      Digest of the manifest image created.       |
|      image       |     Full name of the manifest image created.     |
| platform_digests | Digests of the images created for each platform. |
|       tags       |   Tags applied to the manifest image created.    |

<!-- AUTO-DOC-OUTPUT:END -->
<!-- MERGE:END:build-oci-image - Do not remove or modify this section -->
