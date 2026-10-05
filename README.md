# Ömer Faruk Gündüz — Portföy

Yazılım geliştirme ve görsel içerik hizmetlerini tanıtan tek sayfalık kişisel site.

**Canlı:** [omerfarukgunduz.com](https://omerfarukgunduz.com/)

## Teknoloji

- **HTML5** — tek sayfa (`index.html`)
- **CSS** — gömülü stiller (açık tema, responsive, `prefers-reduced-motion`)
- **Vanilla JavaScript** — menü, scroll ilerleme, yazı animasyonu, FormFlow iletişim formu
- **FormFlow API** — iletişim formu gönderimi
- **Instagram embed.js** — görsel çalışmalar bölümü

Harici UI framework yok; bağımlılık minimum.

## Özellikler

- Tam responsive (mobil menü, güvenli alan / safe area)
- Projeler: tıklanabilir kartlar, ekran görüntüsü alanları
- SEO: canonical, Open Graph, Twitter kartları, Schema.org (`Person`, proje listesi)
- Erişilebilirlik: skip link, ARIA, klavye ile menü kapatma

## İletişim formu

Formlar [FormFlow](https://formflow.omerfarukgunduz.com/) üzerinden gönderilir. API anahtarı `index.html` içinde tanımlıdır; FormFlow panelinde site domain’inin doğrulanmış olması gerekir.
