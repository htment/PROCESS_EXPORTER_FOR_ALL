# Process Exporter Role

Automatically installs Process Exporter for Prometheus with architecture detection.

## Supported Architectures
- x86_64 (amd64)
- i686/i386 (32-bit)
- aarch64 (arm64)
- armv7l

## Variables
- `process_exporter_version`: Version to install (default: 0.7.10)
- `process_exporter_user`: Service user (default: process_exporter)
- `process_exporter_group`: Service group (default: process_exporter)

## Usage
```yaml
- hosts: all
  roles:
    - process_exporter
```
## Запуск 

```
ansible-playbook -i inventory playbook.yml --limit zm
```