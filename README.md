# inspect


```python

Root (Bug Bounty: Sources Analizi)
│
├── 1. JavaScript Dosyaları (JS)
│   │
│   ├── /api Endpoint'leri ve URL'ler
│   │   ├── Örnekler: /api, /v1, /v2, /graphql
│   │   ├── Kontrol Edilecekler:
│   │   │   ├── fetch, axios, XMLHttpRequest
│   │   │   ├── API URL'leri ve endpoint'ler
│   │   │
│   └── API Anahtarları veya Kimlik Bilgileri (Credentials)
│       ├── Aranacak Terimler:
│       │   ├── api_key, access_token, auth_token, jwt
│       │   └── password, username, secret
│
├── 2. Sayfa Kaynakları (HTML ve CSS)
│   │
│   ├── Gizli Yorumlar (`<!-- -->`)
│   │   ├── Aranacak Kelimeler:
│   │   │   ├── TODO, FIXME, debug, test, staging
│   │
│   └── Yönlendirme ve Form URL'leri
│       ├── Formların `action` attributunu kontrol edin
│       ├── Örnek: /api/login, /submit, /form-handler
│
├── 3. API Araştırması (`Sources` ve `Network`)
│   │
│   ├── API Endpoint'leri
│   │   ├── Örnekler: /api, /graphql, /data, /v1
│   │
│   └── `username`, `email`, `password` veya `token` Geçen Yerler
│       ├── Aranacak Kelimeler:
│       │   ├── username, user_id, email
│       │   └── password, jwt, session, token
│
├── 4. Yerel Saklama (`localStorage`, `sessionStorage`, `Cookies`)
│   │
│   ├── Tarayıcıda Saklanan Hassas Veriler
│   │   ├── Aranacak Terimler:
│   │   │   ├── localStorage.setItem, sessionStorage.setItem
│   │   │   └── document.cookie, getCookie
│
├── 5. Özel Dosyalar (`robots.txt` ve `sitemap.xml`)
│   │
│   ├── robots.txt
│   │   ├── Gizli veya engellenmiş URL'leri listeler
│   │   └── Örnek: Disallow: /admin, Disallow: /test
│   │
│   └── sitemap.xml
│       ├── Tüm site yapısını listeler
│       └── Endpoint keşfi için kullanılabilir
│
├── 6. WebSocket Bağlantıları
│   │
│   ├── `wss://` veya `ws://` Bağlantıları
│   │   ├── Anlık veri akışı veya mesajlaşma kontrolü
│   │   └── Örnekler: /socket, /ws, /stream
│
└── 7. Yüklenen Dosya Türleri (JSON, Config, Yedek Dosyalar)
    │
    ├── Yedek Dosyalar ve Yapılandırma Dosyaları
    │   ├── Örnekler: config.json, backup.zip, old-config.js
    │
    └── JSON veya JS Dosyalarındaki Özel İçerikler
        ├── Örnekler: settings.json, data.json, config.js
        └── Potansiyel olarak API anahtarları veya endpoint bilgileri içerebilir


```
