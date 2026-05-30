# @naturacosmeticos/natds-icons

## Supply Chain Security PoC

**This repo was created to demonstrate a GitHub username recycling attack.**

The npm package `@naturacosmeticos/natds-icons` is loaded by `natura.com.br` via:
```html
<link href="https://cdn.jsdelivr.net/npm/@naturacosmeticos/natds-icons@latest/dist/natds-icons.css" />
```

- Tag: `@latest` (no version pinning)
- No Subresource Integrity (SRI) hash
- Maintainer `robert-lichtnow` has publish access
- Original GitHub account was deleted

### Attack Vector
1. Compromise npm account `robert-lichtnow` (email: personal Gmail)
2. Publish malicious version with CSS exfiltration or JS payload
3. jsdelivr CDN picks up `@latest` within ~12 hours
4. natura.com.br serves malicious content to all visitors

### This is a responsible disclosure PoC.
