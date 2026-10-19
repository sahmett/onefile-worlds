# onefile-worlds

Real-time worlds rendered with WebGPU, each one a single HTML file you can double-click.
No engine, no libraries, no build step.

**[Open the gallery →](https://sahmett.github.io/onefile-worlds/)**

[Türkçe aşağıda ↓](#türkçe)

![Sunset over the FFT ocean in Blue Planet](orbit-to-abyss/thumb.jpg)

## Worlds

| World | What it is |
|---|---|
| [**Blue Planet — Orbit to Abyss**](orbit-to-abyss/) | Fall from orbit through the atmosphere and clouds, onto FFT-simulated waves, over a coral reef and down a reef wall to hydrothermal vents 3,400 m deep. [Details](orbit-to-abyss/README.md) |

## The rules

Every world in this collection follows the same constraints:

- **One file.** The whole world is one `index.html`: HTML, CSS, JavaScript and WGSL shaders inline. It also opens straight from disk (`file://`).
- **No engine.** No Three.js, Babylon, Unity or other engines and libraries; everything is written directly against WebGPU.
- **Procedural.** Landscapes, textures and sound are generated in code, not loaded from asset files.
- **Two languages.** The interface works in English and Turkish.

## Running

Open a world's `index.html` in a browser that supports WebGPU (recent Chrome or Edge, Safari 26+). A dedicated or recent integrated GPU is recommended; each world has a quality setting.

To work on a world locally, any static server works, for example:

```bash
python3 -m http.server 8080
```

## Contributing

New worlds are welcome. In short:

1. Fork the repo and create a folder with a short, lowercase name, e.g. `meadow/`.
2. Put the whole world in `meadow/index.html` (one file, no engine or libraries, no external files) and add a `meadow/README.md` and a 960×540 `meadow/thumb.jpg`.
3. Add one entry for your world to the list near the end of the root `index.html`: title, description, tags, your name and GitHub username. Your name appears on the gallery card.
4. Open a pull request. Contributions are released under the MIT license.

## License

[MIT](LICENSE). Some ocean-rendering techniques are adapted from [Noniv/web-ocean](https://github.com/Noniv/web-ocean) (MIT); see the notice in [LICENSE](LICENSE).

---

## Türkçe

WebGPU ile gerçek zamanlı çizilen dünyalar; her biri çift tıklayıp açabileceğin tek bir HTML dosyası. Motor yok, kütüphane yok, derleme adımı yok.

**[Galeriyi aç →](https://sahmett.github.io/onefile-worlds/)**

### Dünyalar

| Dünya | Nedir |
|---|---|
| [**Blue Planet — Yörüngeden Abise**](orbit-to-abyss/) | Yörüngeden atmosfer ve bulutların arasından FFT ile simüle edilen dalgalara, mercan resifinin üstünden resif duvarı boyunca 3.400 m derindeki hidrotermal bacalara in. [Ayrıntılar](orbit-to-abyss/README.md) |

### Kurallar

- **Tek dosya.** Dünyanın tamamı tek bir `index.html`: HTML, CSS, JavaScript ve WGSL shader'ları içinde. Doğrudan diskten de (`file://`) açılır.
- **Motor yok.** Three.js, Babylon, Unity ya da başka bir motor veya kütüphane yok; her şey doğrudan WebGPU ile yazıldı.
- **Prosedürel.** Manzaralar, dokular ve sesler dosyadan yüklenmez, kodla üretilir.
- **İki dil.** Arayüz İngilizce ve Türkçe çalışır.

### Çalıştırma

Bir dünyanın `index.html` dosyasını WebGPU destekleyen bir tarayıcıda aç (güncel Chrome veya Edge, Safari 26+). Ayrı ya da güncel bir entegre ekran kartı önerilir; her dünyanın bir kalite ayarı var.

### Katkı

Yeni dünyalar memnuniyetle karşılanır. Kısaca:

1. Repoyu fork'la ve kısa, küçük harfli bir klasör oluştur; ör. `meadow/`.
2. Dünyanın tamamını `meadow/index.html` içine koy (tek dosya; motor, kütüphane ya da harici dosya yok), bir `meadow/README.md` ve 960×540 boyutunda bir `meadow/thumb.jpg` ekle.
3. Kök dizindeki `index.html`'in sonlarına doğru duran listeye dünyan için bir kayıt ekle: başlık, açıklama, etiketler, adın ve GitHub kullanıcı adın. Adın galerideki kartta görünür.
4. Pull request aç. Katkılar MIT lisansıyla yayımlanır.

### Lisans

[MIT](LICENSE). Bazı okyanus çizim teknikleri [Noniv/web-ocean](https://github.com/Noniv/web-ocean) (MIT) projesinden uyarlanmıştır; ayrıntı [LICENSE](LICENSE) dosyasında.
