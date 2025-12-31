# Mihomo规则集构建报告

**构建时间:** 2026-01-01 07:21:36 (北京时间)
**Mihomo版本:** 
**触发方式:** schedule

## 生成的规则集

- **direct-domain.mrs** - 536274 bytes (.51 MB)
- **direct-ip.mrs** - 22311 bytes (.02 MB)
- **proxy-domain.mrs** - 191385 bytes (.18 MB)
- **proxy-ip.mrs** - 157 bytes (0 MB)
- **reject-domain.mrs** - 1231559 bytes (1.17 MB)

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
