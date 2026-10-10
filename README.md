# MorphTR (morphtr.dev)

> **Türkçe LLM ve RAG Sistemleri İçin Black-Box Test & Güvenlik Kütüphanesi**  
> *Bitirme Tezi Projesi*

MorphTR, Türkçe'nin sondan eklemeli (agglutinative) yapısını ve non-deterministik LLM yanıtlarındaki **Test Oracle** problemini çözmeyi hedefleyen açık kaynaklı bir test kütüphanesidir.

---

## 🎯 Projenin Temel Amaçları

1. **Metamorphic Testing (Biçim Değiştirmeli Test):**
   - Beklenen kesin çıktı (Ground Truth / Oracle) gerektirmeksizin girdilerin Türkçe morfolojik varyasyonları (devrik sözdizimi, eklemeli türetimler, eş anlamlılar) üzerinden anlamsal eşdeğerliğini (Invariance) ve kapsamını (Directional) denetler.
2. **Türkçe Jailbreak & Enjeksiyon Koruması:**
   - Türkçe deyimler, argo, kültürel bağlam ve dolaylı RAG enjeksiyonu gibi saldırı senaryolarına karşı savunma dayanıklılığını ve Saldırı Başarı Oranını (ASR) ölçer.
3. **Türkçe "LLM as a Judge":**
   - RAG mimarilerinde bağlam sadakati (faithfulness), Türkçe akıcılık ve soru-cevap uygunluğu ölçümleri için kalibre edilmiş yerel değerlendirme rubrikleri sunar.

---

## 📁 Dosya Yapısı

- `index.html`: Modern, responsive ve SEO uyumlu landing page.
- `style.css`: Koyu tema (dark mode), neon vurgular ve glassmorphism içeren tasarım sistemi.
- `app.js`: İnteraktif test simülatörü, kod blokları ve panoya kopyalama etkileşimleri.

---

## 🚀 Yerel Olarak Çalıştırma

Sayfayı doğrudan tarayıcıda açabilir ya da basit bir HTTP sunucusu ile görüntüleyebilirsiniz:

```bash
# Python ile:
python -m http.server 8080

# Tarayıcıda açın:
# http://localhost:8080
```

---

## 🌐 morphtr.dev Dağıtımı (Deployment)

Bu proje statik web standartlarında (HTML/CSS/JS) geliştirildiği için herhangi bir derleme (build) adımına ihtiyaç duymadan anında yayına alınabilir:

- **Vercel / Netlify:** Klasörü doğrudan sürükleyip bırakarak veya GitHub deposunu bağlayarak tek tıkla dağıtabilirsiniz.
- **Cloudflare Pages / GitHub Pages:** `d:\Projects\MorphTr` dizinini depoya gönderip `morphtr.dev` özel alan adını DNS panelinizden bağlayabilirsiniz.
