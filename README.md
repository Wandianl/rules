# Mihomo Binary Rules

Generated at: $(date -u +%Y-%m-%dT%H:%M:%SZ)

## Available Rule Sets

| File | Description |
|------|-------------|
| direct.mrs | direct rules |
| proxy.mrs | proxy rules |
| reject.mrs | reject rules |

## Usage in mihomo config

```yaml
rule-providers:
  direct:
    type: http
    behavior: domain
    format: mrs
    url: https://github.com/YOUR_USERNAME/YOUR_REPO/releases/latest/download/direct.mrs
    interval: 86400
  proxy:
    type: http
    behavior: domain
    format: mrs
    url: https://github.com/YOUR_USERNAME/YOUR_REPO/releases/latest/download/proxy.mrs
    interval: 86400
  reject:
    type: http
    behavior: domain
    format: mrs
    url: https://github.com/YOUR_USERNAME/YOUR_REPO/releases/latest/download/reject.mrs
    interval: 86400

rules:
  - RULE-SET,reject,REJECT
  - RULE-SET,direct,DIRECT
  - RULE-SET,proxy,PROXY
```
