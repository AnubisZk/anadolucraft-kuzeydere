# AnatolianCraft: Kuzeydere

AnatolianCraft: Kuzeydere, karlı dağlar, taş kaleler ve kuzey rüzgarları
etrafında şekillenen web tabanlı bir micro-MMO başlangıç paketidir. Bu repo,
Batıdere Craft altyapısı üzerine kurulmuş yeni Kuzeydere varyantıdır.

![AnatolianCraft: Kuzeydere title screen](public/loading-screen.jpg)

- Kaynak kod: https://github.com/AnubisZk/anadolucraft-kuzeydere
- Temel altyapı: Vite, TypeScript, Three.js, WebSocket server, Postgres destekli
  çevrim içi karakter kalıcılığı
- Modlar: çevrim içi sunucu modu ve hızlı çevrim dışı tarayıcı modu

## Kuzeydere Yönü

Açılış ekranı Kuzeydere konseptine göre hazırlandı: karlı dağ vadisi, taş kale,
köprü ve soğuk sisli atmosfer. Kutup kurdu, çevre objeleri, müzik ve ek Meshy
modelleri üretildiğinde bunlar `public/` ve `src/render/characters/manifest.ts`
üzerinden bağlanabilir.

Önerilen ilk asset işleri:

- Kutup kurdu modeli: mevcut wolf/yeti yaratık hattına yeni GLB olarak ekle.
- Kuzeydere müziği: `public/audio/` altına MP3 koyup `src/game/music.ts`
  içinde rota/playlist olarak tanıt.
- Kale/köprü/kar prop setleri: optimize edilmiş GLB dosyalarını `public/models/`
  altına koyup prop manifestine bağla.
- Logo finali: mevcut `public/anatoliancraft-logo.png` korunuyor; Kuzeydere
  özel logo hazır olduğunda aynı dosya adıyla değiştirilebilir.

## Lokal Çalıştırma

```bash
npm install
npm run dev
```

Tarayıcıda http://localhost:5173 adresini açıp **Çevrim Dışı Oyna** ile hemen
deneyebilirsin.

## Çevrim İçi Geliştirme

```bash
npm run db:up
npm run server
npm run dev
```

Sunucu tarafı hesap, karakter, envanter, görev ve konum verilerini Postgres'te
saklar. Çevrim dışı mod aynı simülasyon çekirdeğini kullanır ama kalıcı kayıt
yapmaz.

## Lisans ve Krediler

Kod MIT lisansı ile gelir. Üçüncü taraf asset bildirimleri ve kaynaklar için
`CREDITS.md` dosyasına bak.
