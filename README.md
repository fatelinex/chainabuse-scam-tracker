# Chainabuse Scam Tracker

Public dataset of AI-verified live scam websites sourced from [Chainabuse](https://chainabuse.com/) reports, enriched with origin IP discovery and upstream IDC/ASN abuse contact resolution.

## Dataset (`scam_websites.csv`)

Updated automatically every hour (when new verified scam domains are detected). Sorted newest-first by UTC report timestamp.

| Column | Description |
| --- | --- |
| `报告ID` | Chainabuse report UUID (with `#2`, `#3` suffix if one report covers multiple distinct scam domains) |
| `举报时间(UTC)` | Report creation timestamp in UTC |
| `诈骗类型` | Scam category in Chinese |
| `主域名` | Registrable root domain (`eTLD+1`) |
| `可访问网址` | Verified reachable URL at time of capture |
| `网页标题` | Extracted HTML `<title>` |
| `AI研判摘要` | Concise AI-verified summary of the scam tactic and domain evidence |
| `报告链接` | Direct link to the Chainabuse report |
| `真实IP` | Resolved origin IPv4 address(es), or Cloudflare CDN status |
| `上游IDC/ASN` | Upstream hosting provider / ASN and country |
| `IDC官网` | Official website(s) of the upstream IDC/ASN |
| `IP定位手段与线索` | DNS/OSINT method used to identify the origin IP |
| `机房投诉邮箱` | Abuse contact email(s) for takedown reporting |
