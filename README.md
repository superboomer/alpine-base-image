# Alpine Base Image

A minimal Alpine-based Docker image built on top of the official Golang Alpine image. This image includes essential tools and certificates for building and running Go applications.

## Features

- Based on the official `golang:alpine` image
- Pre-installed packages:
  - `git`: For source code management
  - `tzdata`: Time zone database
  - `ca-certificates`: SSL certificates for secure communications

## Usage

To use this image as a base for your application, reference it in your Dockerfile:

```dockerfile
FROM superboomer/alpine-base-image:latest

# Add your application-specific instructions here
```

## Building

To build the image locally:

```bash
docker build -f Dockerfile-alpine -t alpine-base-image .
```
