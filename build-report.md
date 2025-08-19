# Mihomo规则集构建报告

**构建时间:** 2025-08-20 07:19:20 (北京时间)
**Mihomo版本:** 
**触发方式:** schedule

## 生成的规则集

- **direct-domain.mrs** - 559448 bytes (.53 MB)
- **direct-ip.mrs** - 43294 bytes (.04 MB)
- **proxy-domain.mrs** - 218098 bytes (.20 MB)
- **proxy-ip.mrs** - 157 bytes (0 MB)
- **reject-domain.mrs** - 1286525 bytes (1.22 MB)

## 使用方法

```yaml
rule-providers:
  direct-domain:
    type: http
    format: mrs
    url: https://github.com/Wandianl/rules/raw/main/direct-domain.mrs
    interval: 86400

  direct-ip:
    type: http
    format: mrs
    url: https://github.com/Wandianl/rules/raw/main/direct-ip.mrs
    interval: 86400

  proxy-domain:
    type: http
    format: mrs
    url: https://github.com/Wandianl/rules/raw/main/proxy-domain.mrs
    interval: 86400

  proxy-ip:
    type: http
    format: mrs
    url: https://github.com/Wandianl/rules/raw/main/proxy-ip.mrs
    interval: 86400

  reject-domain:
    type: http
    format: mrs
    url: https://github.com/Wandianl/rules/raw/main/reject-domain.mrs
    interval: 86400

```
