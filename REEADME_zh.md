# 免费代理来源清单

以下为公网常见的**免费代理列表 / API 来源**，供学习与测试使用。不保证可用性、速度与安全性，**请勿用于生产或非法用途**。

---

## 一、免费代理列表网站

| 名称 | 说明 | 链接 |
|------|------|------|
| ProxyScrape | 提供 HTTP/HTTPS/SOCKS 列表，可在线筛选国家、匿名等级，支持导出与 API | [proxyscrape.com](https://proxyscrape.com) |
| Free Proxy List | 按国家、匿名类型筛选，页面展示 IP:端口，可手动复制 | [free-proxy-list.net](https://free-proxy-list.net) |
| ProxyRadar | 多国家代理聚合，支持 HTTP/HTTPS/SOCKS4/SOCKS5，可导出 TXT/CSV/JSON 或调用 API | [proxyradar.net](https://proxyradar.net) |
| GeoNode | 免费与付费混合，提供免费代理列表与 API，可按国家筛选 | [geonode.com](https://geonode.com/free-proxy-list) |
| Spys.one | 按国家、端口、类型筛选，更新较频繁 | [spys.one](https://spys.one/en/) |

特点：无需注册即可浏览或下载列表，但**存活率普遍较低**，使用前建议自建测速与过滤。

---

## 二、免费代理 API

适合在脚本中直接请求，获取当前可用的代理列表（多为 IP:PORT 或 JSON）。

| 名称 | 说明 | 示例 / 文档 |
|------|------|-------------|
| ProxyScrape API | 按类型、国家、匿名等级获取，返回文本或 JSON | [docs.proxyscrape.com](https://docs.proxyscrape.com/) |
| Proxy List API | RESTful API，支持按 HTTP/HTTPS/SOCKS、国家、匿名等级筛选 | [proxy-list.download](https://www.proxy-list.download/api/v1) |
| ProxyRadar API | 聚合多源，支持按国家、协议筛选，可导出或 API 调用 | [proxyradar.net/docs/api](https://proxyradar.net/docs/api) |

注意：多数免费 API 有请求频率限制，且返回的代理**未做长期可用性保证**，需要本地测速与轮换。

---

## 三、GitHub 上的代理列表与工具

| 仓库 | 说明 |
|------|------|
| [clarketm/proxy-list](https://github.com/clarketm/proxy-list) | 每日更新的公网免费代理列表，可直接用 raw 链接拉取文本 |
| [ProxRipper](https://github.com/mohammedcha/ProxRipper) | 自动抓取并更新，提供 HTTP/HTTPS/SOCKS4/SOCKS5 分文件，约 15 分钟更新一次，raw 文件可直接 wget/curl |

使用方式示例（ProxRipper）：

```bash
# 拉取 HTTP 代理列表（示例，以仓库实际路径为准）
curl -sL "https://raw.githubusercontent.com/mohammedcha/ProxRipper/main/full_proxies/http.txt"
```

---

## 四、使用建议

1. **先测速再使用**：免费列表里大量代理已失效，建议用脚本批量检测（如检测 HTTP 响应、超时时间），只保留可用节点。
2. **不要带敏感流量**：免费代理多为他人搭建或公开转发，存在窃听、篡改风险，不要传输账号密码、支付信息等。
3. **控制请求频率**：即使用代理，对目标站点也请合理限速，避免滥用。
4. **生产环境**：若需要稳定、可观测的动态代理，建议使用带免费额度的正规服务（如 [Bytesflows 签到领流量](https://bytesflows.com)），或自建代理池。

---

## 五、免责声明

- 本清单仅整理**公开来源**，不托管、不运营任何代理节点。
- 上述网站与 API 的可用性、合规性由各自运营方负责，使用前请自行核实。
- 使用代理时请遵守目标网站的服务条款及所在地区法律法规，**禁止将免费代理用于非法用途**。

如有更好来源或发现链接失效，欢迎提 Issue 或 PR 更新本清单。
