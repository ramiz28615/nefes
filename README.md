# 🫁 Nefes — Bilimsel Nefes Koçu

Tarayıcıda çalışan, kurulum gerektirmeyen nefes egzersizi uygulaması.
Uyku, stres, odak ve sıfırlama için dört farklı bilimsel protokol.

**Canlı:** https://ramiz28615.github.io/nefes/

---

## Neden bu ürün?

Nefes, otonom sinir sistemine açılan tek bilinçli kapıdır. Yavaş ve derin nefes vagus siniri
üzerinden parasempatik sistemi devreye alır — kalp atışı yavaşlar, stres hormonları düşer,
zihin sakinleşir. Piyasadaki uygulamaların çoğu bunu abonelik arkasına kilitler.

**Nefes** aynı işi yapar, ama: kayıt yok, reklam yok, sunucu yok, veri cihazdan çıkmıyor.
Bu yüzden sıfır işletme maliyetiyle sonsuza kadar ücretsiz kalabilir.

## Protokoller

| Mod | Ritim | Tur | Kullanım |
|---|---|---|---|
| 🌙 **Uykuya Dal** | 4-7-8 | 4 | Yatmadan önce, uykuya geçiş |
| 🌿 **Stresi Azalt** | 5-5 | 6 | Gün içi dengeleme, kaygı |
| ⚡ **Odaklan** | 2-2 | 15 | İşe/sınava başlamadan önce |
| 🔄 **Sıfırla** | 4-4-6-1 | 5 | Zihin dağınıkken toparlanma |

## Özellikler

- **Görsel halka rehberi** — saymak gerekmez, halka nefesin olur
- **Sesli yönlendirme** — Web Speech API ile Türkçe faz anonsu
- **Üretilen ses tonları** — Web Audio API, ses dosyası yok (0 KB medya)
- **Titreşim** — destekleyen cihazlarda faz geçişlerinde haptic geri bildirim
- **İlerleme takibi** — seans, dakika, gün serisi (localStorage)
- **Tema renkleri** — seçilen moda göre tüm arayüz rengi yumuşak geçişle değişir
- **Klavye kısayolu** — boşluk tuşu ile başlat/durdur
- **Sekme değişince otomatik duraklama**
- **Erişilebilirlik** — `prefers-reduced-motion` desteği
- **Tamamen duyarlı** — mobil öncelikli tasarım

## Teknik

- Bağımlılık **sıfır**: saf HTML + CSS + JavaScript
- Tek dosya (`index.html`, ~37 KB) — herhangi bir statik sunucuda çalışır
- Aurora arka plan, film grain dokusu, cam efektli kartlar
- `IntersectionObserver` ile kaydırma animasyonları
- `requestAnimationFrame` tabanlı hassas faz zamanlayıcı
- Renkler CSS `color-mix()` ve özel değişkenlerle tema bazlı

## Çalıştırma

```bash
# herhangi bir statik sunucu
npx serve .
# ya da
python -m http.server
```

Ya da `index.html` dosyasını doğrudan tarayıcıda aç.

## Lisans

MIT — ticari kullanım dahil serbestçe kullanılabilir.
