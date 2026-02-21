# Free Proxy List · Public Sources

A curated list of **free proxy list websites and APIs** commonly found on the public internet. For **learning and testing only**. No guarantee of availability, speed, or security. **Do not use in production or for illegal purposes.**

---

## 1. Free proxy list websites

| Name | Description | Link |
|------|-------------|------|
| ProxyScrape | HTTP/HTTPS/SOCKS lists; filter by country and anonymity; export and API | [proxyscrape.com](https://proxyscrape.com) |
| Free Proxy List | Filter by country and anonymity; IP:port on page, copy manually | [free-proxy-list.net](https://free-proxy-list.net) |
| ProxyRadar | Multi-country aggregation; HTTP/HTTPS/SOCKS4/SOCKS5; export TXT/CSV/JSON or API | [proxyradar.net](https://proxyradar.net) |
| GeoNode | Free + paid; free proxy list and API; filter by country | [geonode.com](https://geonode.com/free-proxy-list) |
| Spys.one | Filter by country, port, type; updated frequently | [spys.one](https://spys.one/en/) |

No sign-up needed to browse or download. **Survival rate is generally low**; consider testing and filtering before use.

---

## 2. Free proxy APIs

Suitable for use in scripts to fetch current proxy lists (usually IP:PORT or JSON).

| Name | Description | Docs / example |
|------|-------------|----------------|
| ProxyScrape API | Get by type, country, anonymity; returns text or JSON | [docs.proxyscrape.com](https://docs.proxyscrape.com/) |
| Proxy List API | RESTful API; filter by HTTP/HTTPS/SOCKS, country, anonymity | [proxy-list.download](https://www.proxy-list.download/api/v1) |
| ProxyRadar API | Aggregated sources; filter by country and protocol; export or API | [proxyradar.net/docs/api](https://proxyradar.net/docs/api) |

Most free APIs are rate-limited and **do not guarantee long-term availability**; run local checks and rotation.

---

## 3. Proxy lists and tools on GitHub

| Repository | Description |
|------------|-------------|
| [clarketm/proxy-list](https://github.com/clarketm/proxy-list) | Daily-updated public free proxy list; fetch via raw URLs |
| [ProxRipper](https://github.com/mohammedcha/ProxRipper) | Auto-scraped; HTTP/HTTPS/SOCKS4/SOCKS5 in separate files; ~15 min updates; raw files for wget/curl |

Example (ProxRipper):

```bash
# Fetch HTTP proxy list (path may change; check repo)
curl -sL "https://raw.githubusercontent.com/mohammedcha/ProxRipper/main/full_proxies/http.txt"
```

---

## 4. Usage tips

1. **Test before use** — Many entries are dead. Batch-check (e.g. HTTP response, timeout) and keep only working proxies.
2. **No sensitive traffic** — Free proxies are often third-party; risk of sniffing or tampering. Do not send passwords, payment data, etc.
3. **Throttle requests** — Even with proxies, respect target sites; avoid abuse.
4. **Production** — For stable, observable dynamic proxy, use a service with a free tier (e.g. [Bytesflows — daily check-in for proxy traffic](https://bytesflows.com)) or build your own proxy pool.

---

## 5. Disclaimer

- This list only **curates public sources**. We do not host or operate any proxy nodes.
- Availability and compliance of the listed sites/APIs are the responsibility of their operators; verify before use.
- Use proxies in compliance with target sites’ terms of service and local laws. **Do not use free proxies for illegal purposes.**

If you have better sources or find broken links, feel free to open an Issue or PR to update this list.
