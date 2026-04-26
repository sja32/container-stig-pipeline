# Container STIG Pipeline

This project demonstrates applying STIG-aligned security principles to containerized workloads using Docker and Trivy.

## Results

| Metric | Insecure Container | Hardened Container |
|---|---:|---:|
| Total Vulnerabilities | 42 | 1 |
| Critical | 0 | 0 |
| High | 0 | 0 |
| Medium | 20 | 1 |
| Low | 22 | 0 |

## Security Improvements

- Replaced full Ubuntu base image with minimal `nginx:alpine`
- Removed unnecessary packages
- Implemented non-root container execution
- Corrected ownership and permissions
- Reduced container attack surface

## Tools Used

- Docker
- Trivy
- Ubuntu VM

## Future Enhancements

- Automate scans with Ansible
- Integrate with AWX
- Deploy hardened container to Kubernetes

