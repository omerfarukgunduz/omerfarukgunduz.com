# Ömer Faruk Gündüz — Portföy

Yazılım geliştirme ve görsel içerik hizmetlerini tanıtan tek sayfalık kişisel site.

**Canlı:** [omerfarukgunduz.com](https://omerfarukgunduz.com/)

## Teknoloji

- **HTML5** — anasayfa, iletişim sayfası
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

## Dosya yapısı

| Dosya | Açıklama |
|--------|-----------|
| `index.html` | Ana sayfa (stil + script tek dosyada) |
| `iletisim.html` | Bağımsız iletişim formu (FormFlow) |
| `ofg.png` | Favicon ve marka logosu |
| `ofg_portre.png` | Hakkımda portresi ve paylaşım önizlemesi (sunucuda, repoda opsiyonel) |
| `proje1.png` … `proje6.png` | Proje kartı ekran görüntüleri (sunucuda) |
| `robots.txt`, `sitemap.xml` | Arama motoru |

## İletişim formu

Formlar [FormFlow](https://formflow.omerfarukgunduz.com/) üzerinden gönderilir. API anahtarı `index.html` ve `iletisim.html` içinde tanımlıdır; FormFlow panelinde site domain’inin doğrulanmış olması gerekir.

## Yerel önizleme

```bash
python3 -m http.server 8080
```

Tarayıcıda `http://localhost:8080/` açın. Statik dosyalar (portre, proje görselleri) yerelde yoksa kartlarda placeholder görünür.

## Dağıtım

Statik dosyalar IIS / Plesk köküne kopyalanır veya `main` dalı GitHub üzerinden deploy edilir. Görsel dosyalar repoda yoksa sunucuya ayrıca yüklenmelidir.
