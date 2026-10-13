# Space / Aurora Ambient — 6 prompt Suno cho video 1 giờ

Bộ 6 bản nhạc cùng chất (ấm, không chói, không cello, không trống), khác nhau về tông,
nhạc cụ dẫn và năng lượng để video không bị một màu. Các tông nằm trong họ F major /
C major nên chuyển bài êm.

## Thứ tự trong video

| # | Tên bản | Tông | BPM | Nhạc cụ dẫn | Năng lượng |
|---|---|---|---|---|---|
| 1 | Aurora Rising | F Lydian | 60 | Rhodes ấm | Vừa, mở màn |
| 2 | Frozen Horizon | D minor | 56 | Felt piano | Thấp, trầm lắng |
| 3 | Nebula Strings | Bb major | 60 | Guitar nylon ngón | Vừa, ấm áp |
| 4 | Stardust Drift | C major | 64 | Arpeggio synth mềm, quãng thấp | Cao nhất, có chuyển động |
| 5 | Deep Space Breath | A minor | 60 | Pad nhiều lớp, piano có delay | Nhẹ nhất, vẫn có chuyển động |
| 6 | Return to Aurora | F major | 60 | Rhodes và piano | Vừa, khép lại vòng |

## Thông số Suno

Bật **Instrumental** cho mọi bản.

| # | Weirdness | Style Influence | Variety |
|---|---|---|---|
| 1 | 30% | 70% | Normal |
| 2 | 25% | 75% | Normal |
| 3 | 30% | 80% | Normal |
| 4 | 35% | 70% | Normal |
| 5 | 28% | 75% | Normal |
| 6 | 30% | 70% | Normal |

- Còn nốt chói: hạ Weirdness 5–10%.
- Nhạc quá đều: tăng Weirdness lên 35–40% (chỉ bản 1, 4, 6).
- Suno bỏ qua nhạc cụ trong prompt: tăng Style Influence thêm 5–10%.
- Khi dùng Extend, giữ đúng thông số của lần tạo gốc.

## Exclude Styles (dùng chung cho cả 6 bản)

```
cello, strings, violin, viola, orchestra, bells, chimes, glockenspiel, celesta, music box, high-pitched, piercing, shrill, bright, sparkle, shimmer, glassy, crystal, whistle, high arpeggio, harsh, drums, percussion, vocals, choir, edm, bass drop, epic
```

---

## 1. Aurora Rising — F Lydian, Rhodes

**Style:**
```
warm space ambient, aurora, mellow analog synth pads, soft rounded low-register melody, warm Rhodes, soft felt piano in low and middle register, deep warm analog synth drone, warm tape saturation, low-pass filtered, soft attack, slow swells, 60 BPM, F lydian, floating, cozy, dreamy, deep and warm, soft rounded highs, dark warm tone, smooth, no harsh frequencies, no drums, no vocals, instrumental
```

**Lyrics:**
```
[Instrumental]

[Intro]
[warm analog synth drone fades in, soft and rounded]

[Verse 1]
[mellow analog pads, chords F - C - G, slow swells, low-pass filtered]

[Verse 2]
[soft low-register melody on warm Rhodes, few notes, long pauses]

[Bridge]
[pads swell gently, warmer and wider, same low register, no high notes]
[chords F - C - G - Am]

[Verse 3]
[soft felt piano in middle register, calm, floating]

[Outro]
[warm pads and synth drone only, same opening chord F, steady volume, seamless loop]
```

## 2. Frozen Horizon — D minor, felt piano

**Style:**
```
warm space ambient, frozen horizon at night, soft felt piano in low and middle register, mellow analog synth pads, deep warm synth drone, slow sparse melody with long silences, introspective, calm, slightly melancholic but warm, warm tape saturation, low-pass filtered, soft attack, 56 BPM, D minor, soft rounded highs, no drums, no vocals, instrumental
```

**Lyrics:**
```
[Instrumental]
[Intro] [warm drone and soft pads, very quiet]
[Verse] [felt piano, few notes, long silences, chords Dm - Bb - F - C]
[Bridge] [pads swell slowly, piano rests]
[Verse] [felt piano returns, softer, lower register]
[Outro] [pads and drone only, chord Dm, steady volume, seamless loop]
```

## 3. Nebula Strings — Bb major, guitar nylon

**Style:**
```
warm space ambient, drifting nebula, soft fingerpicked nylon guitar in low register, warm analog pads, gentle synth drone, intimate, cozy, floating, slow gentle picking, warm tape saturation, low-pass filtered, soft attack, 60 BPM, Bb major, soft rounded highs, no drums, no vocals, instrumental
```

**Lyrics:**
```
[Instrumental]
[Intro] [warm pads fade in]
[Verse] [soft fingerpicked nylon guitar, slow, chords Bb - F - Gm - Eb]
[Bridge] [guitar rests, pads swell warmly]
[Verse] [nylon guitar returns with gentle melody, low register]
[Outro] [pads and soft guitar harmonics fade into drone, chord Bb, seamless loop]
```

Nếu Suno bỏ mất guitar, xóa `strings` khỏi Exclude cho riêng bản này.

## 4. Stardust Drift — C major, arpeggio mềm

**Style:**
```
warm space ambient, drifting through stardust, soft slow analog synth arpeggio in low and middle register, warm Rhodes chords, mellow pads, gentle pulse without drums, gently moving, hopeful, floating, warm tape saturation, low-pass filtered, soft attack, 64 BPM, C major, soft rounded highs, no drums, no vocals, instrumental
```

**Lyrics:**
```
[Instrumental]
[Intro] [soft low arpeggio fades in, warm and muted]
[Verse] [Rhodes chords join, C - G - Am - F, gentle motion]
[Bridge] [arpeggio thins out, pads swell, same low register]
[Verse] [arpeggio and Rhodes together, calm and steady]
[Outro] [arpeggio fades, pads remain, chord C, seamless loop]
```

## 5. Deep Space Breath — A minor, pad nhiều lớp

**Style:**
```
warm space ambient, deep space breathing, layered mellow analog synth pads, slow gentle low-register synth pulse, soft felt piano motifs with warm tape delay echoes, warm Rhodes chords, deep warm analog bass, evolving textures, gentle movement, meditative but flowing, calm, weightless, warm tape saturation, low-pass filtered, soft attack, 60 BPM, A minor, soft rounded highs, no drums, no vocals, instrumental
```

**Lyrics:**
```
[Instrumental]

[Intro]
[warm drone and soft low synth pulse fade in]

[Verse 1]
[layered pads breathe in and out, chords Am - F - C - G]
[warm analog bass follows the chords gently]

[Verse 2]
[soft felt piano motifs with warm tape delay echoes, few notes]
[warm Rhodes chords join softly]

[Bridge]
[pads open up, new chord colors Fmaj7 - Em7 - Am, gentle swell]

[Verse 3]
[piano motifs and Rhodes together, low synth pulse continues, calm flowing]

[Outro]
[pads, bass and pulse only, chord Am, steady volume, seamless loop]
```

- Vẫn thấy thưa: thêm `richer arrangement, more layers` vào Style.
- Dày quá, mất cảm giác "nghỉ": bỏ `warm Rhodes chords`.

## 6. Return to Aurora — F major, Rhodes và piano

**Style:**
```
warm space ambient, aurora returning at dawn, warm Rhodes and soft felt piano in middle register, mellow analog pads, deep warm synth drone, gentle and peaceful, resolving, comforting, warm tape saturation, low-pass filtered, soft attack, slow swells, 60 BPM, F major, soft rounded highs, no drums, no vocals, instrumental
```

**Lyrics:**
```
[Instrumental]
[Intro] [warm pads and drone fade in]
[Verse] [Rhodes melody, few notes, chords F - C - Dm - Bb]
[Verse] [felt piano answers Rhodes, calm conversation]
[Bridge] [pads swell warmly, both instruments rest]
[Outro] [Rhodes plays the opening phrase once more, pads hold chord F, seamless loop]
```

---

## Ghép thành video 1 giờ

- Dùng **Extend** kéo mỗi bản lên khoảng 8–10 phút, hoặc tạo 2 phiên bản mỗi bản rồi ghép.
- Thứ tự 1 → 6, tổng khoảng 60 phút. Muốn dài hơn thì lặp lại cả chuỗi (bản 6 về lại tông F của bản 1).
- Crossfade 8–12 giây giữa các bản.
- Master mọi bản về khoảng −14 LUFS, true peak ≤ −1 dBTP.
- Nếu còn chỗ chói: giảm 2,5–5 kHz khoảng 3–5 dB, low-pass mềm ở 8–10 kHz.
- Nếu sub bass quá nhiều: cắt dưới 40 Hz, giảm 60–100 Hz khoảng 3 dB.
- Gợi ý hình ảnh: đổi nhẹ màu cực quang khi chuyển bài (bản 2 xanh lạnh, bản 3 tím ấm, bản 5 tối hơn).
