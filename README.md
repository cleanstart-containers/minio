# CleanStart Container for MinIO

Official MinIO container image optimized for enterprise environments. Includes high-performance object storage server compatible with Amazon S3 API for scalable and secure data storage. Features security-hardened base image, minimal attack surface, and FIPS-compliant cryptographic modules. Supports both production deployments and development workflows with separate tagged versions. Includes MinIO server, web console, and essential object storage tools.

---

## Key Features

Complete object storage environment with S3-compatible API:

- Complete object storage environment with S3-compatible API
- Optimized for cloud-native and microservices architectures
- High-performance object storage server
- Security-hardened base image with minimal attack surface
- FIPS-compliant cryptographic modules
- Web console for management

---

## Common Use Cases

Typical scenarios where this container excels:

- Building and deploying object storage solutions
- Cloud-native data storage development
- S3-compatible storage infrastructure
- Backup and archival storage
- Media and asset storage
- Data lake implementations

---

## Getting Started

### Pull Commands

Download the runtime container images:
```bash
docker pull cleanstart/minio:latest
docker pull cleanstart/minio:latest-dev
```

### Interactive Development

Start interactive session for development:
```bash
docker run --rm -it --entrypoint /bin/sh cleanstart/minio:latest-dev
```

### Container Start

Start the container:
```bash
docker run --rm -it --name minio-dev cleanstart/minio:latest
```

---

## Best Practices

- Use specific image tags for production (avoid latest)
- Configure resource limits: memory and CPU constraints
- Enable read-only root filesystem when possible

---

## Architecture Support

### Multi-Platform Images
```bash
docker pull --platform linux/amd64 cleanstart/minio:latest
docker pull --platform linux/arm64 cleanstart/minio:latest
```

---

## Resources

- **Official Documentation:** https://min.io/docs/
- **Provenance / SBOM / Signature:** https://images.cleanstart.com/images/minio
- **Docker Hub:** https://hub.docker.com/r/cleanstart/minio
- **CleanStart All Images:** https://images.cleanstart.com
- **CleanStart Community Images:** https://hub.docker.com/u/cleanstart

---

## Vulnerability Disclaimer

CleanStart offers Docker images that include third-party open-source libraries and packages maintained by independent contributors. While CleanStart maintains these images and applies industry-standard security practices, it cannot guarantee the security or integrity of upstream components beyond its control.

Users acknowledge and agree that open-source software may contain undiscovered vulnerabilities or introduce new risks through updates. CleanStart shall not be liable for security issues originating from third-party libraries, including but not limited to zero-day exploits, supply chain attacks, or contributor-introduced risks.

**Security remains a shared responsibility:** CleanStart provides updated images and guidance where possible, while users are responsible for evaluating deployments and implementing appropriate controls.
