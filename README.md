# surge-rules

Surge DOMAIN-SET lists converted from upstream rule projects, hosted here so Surge can fetch them directly.

## meta-domainset.list

- Source: MetaCubeX/meta-rules-dat, `geo/geosite/classical/meta.list` (meta branch), fetched 2026-11-19.
- Format: Surge DOMAIN-SET, one domain per line. A leading dot (`.facebook.com`) matches the domain and all its subdomains; a bare domain matches exactly.
- Conversion: upstream uses Clash text format (`+.domain` = suffix, bare = exact). `+.x` was rewritten to `.x`; bare entries kept as-is. 5 entries provably covered by sibling suffix entries were dropped (developers/analytics/pixel.facebook.com, graph/graph-fallback.instagram.com); coverage is unchanged.
- Served via jsDelivr: https://cdn.jsdelivr.net/gh/jtian93/surge-rules@main/meta-domainset.list
- Refresh: re-run the conversion from the latest upstream list and push.
