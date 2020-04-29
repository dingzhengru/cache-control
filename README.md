# cache-control
http header cache-control 測試 & 筆記


## 參考
* HTTP 快取: https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/http-caching?hl=zh-tw
* 循序漸進理解 HTTP Cache 機制: https://blog.techbridge.cc/2017/06/17/cache-introduction/
* MDN: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Cache-Control

## 測試
* express server 的 get('/') ```res.set('Cache-Control', 'no-store')```
* 針對那 / 頁面不會快取，但其他資源還是會照各個 response 做對應的快取策略