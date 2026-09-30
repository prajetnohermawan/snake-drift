# Snake Drift

Game ular di browser dengan satu kejutan: arena mulai bergoyang begitu kamu makan, dan makin banyak kamu makan, makin miring arenanya dan makin cepat ularnya.

Arah kontrol selalu mengikuti papan, bukan layar. Jadi "atas" tetap berarti atas di papan, walaupun papannya sedang miring.

## Cara main

Tidak perlu instalasi atau build. Buka `index.html` di browser modern apa saja:

```bash
open index.html
```

## Kontrol

| Aksi | Keyboard | Layar sentuh |
| --- | --- | --- |
| Mengarahkan | Tombol panah atau `W` `A` `S` `D` | Geser |
| Mulai / main lagi | `Spasi`, `Enter`, atau tombol Main | Ketuk Main |
| Jeda / lanjut | `Spasi` (atau `Enter` untuk lanjut) | Ketuk Lanjut |

## Aturan main

- Papannya berukuran 20 × 20 kotak. Setiap titik merah muda yang dimakan menambah satu skor dan memanjangkan ular satu kotak.
- Setiap skor membuat ular makin cepat, dari 140 ms per langkah sampai paling cepat 60 ms.
- Goyangan arena makin besar seiring skor, sampai sekitar 38°.
- Menabrak dinding atau badan sendiri berarti permainan selesai. Penuhi seluruh papan untuk menang.
- Skor terbaikmu disimpan di browser (`localStorage`), jadi tidak hilang saat halaman dimuat ulang.

Semuanya, termasuk HTML, CSS, dan JavaScript, ada di satu file `index.html`.
