# Folder Structure: Mini Lyra

## Visual Tree

```
mini-lyra/
├── README.md
├── SKILL.md
├── SYSTEM-PROMPT.md
├── FOLDER-STRUCTURE.md
├── standards/
│   └── humanize-writing-guide.md
└── references/
    ├── hook-patterns.md
    ├── script-outline-patterns.md
    └── scoring-diagnostic-guide.md
```

**Total: 8 file**

---

## Penjelasan Per File

| File | Fungsi | Audience |
|---|---|---|
| `README.md` | Panduan install dan pakai untuk pembeli playbook | End user (pembaca playbook) |
| `SKILL.md` | Definisi capability, alur, output structure, guardrails | AI (Claude/ChatGPT) |
| `SYSTEM-PROMPT.md` | Persona detail, protokol humanize, prinsip kerja, anti-pattern | AI (Claude/ChatGPT) |
| `FOLDER-STRUCTURE.md` | Peta folder ini + perbandingan dengan Lyra full | Pemilik skill (kamu) |
| `standards/humanize-writing-guide.md` | Protokol humanize zero tolerance (Tier 1 dan Tier 2) | AI |
| `references/hook-patterns.md` | Subset hook patterns dari Lyra full untuk Capability 1 | AI |
| `references/script-outline-patterns.md` | Subset struktur script dari Lyra full untuk Capability 2 | AI |
| `references/scoring-diagnostic-guide.md` | Rubric skoring dan checklist diagnostic untuk Capability 3 | AI |

---

## Perbandingan dengan Lyra Full

### Struktur Lyra Full (Referensi)

```
lyra-copywriter-skill/
├── README.md
├── SKILL.md
├── SYSTEM-PROMPT.md
├── FOLDER-STRUCTURE.md
├── standards/
│   └── humanization-standards.md
├── frameworks/
│   ├── content-psychology.md
│   ├── copywriting-frameworks.md
│   ├── direct-response-copywriting.md
│   ├── heuristic-bias-deep.md
│   ├── hook-retention.md
│   └── storytelling-framework.md
└── references/
    ├── brand-onboarding-system.md
    ├── contoh-multi-format.md
    ├── rules-format-konten.md
    ├── script-pattern-overview.md
    └── script-library/
        └── (10 file script library, 200 script viral)
```

**Total Lyra full: ~20+ file** (termasuk script library).

### Perbandingan Side-by-Side

| Aspek | Lyra Full | Mini Lyra |
|---|---|---|
| **Jumlah file** | 20+ | 8 |
| **Folder frameworks/** | 6 file (psychology, copywriting, direct response, heuristic bias, hook retention, storytelling) | Tidak ada (subset diintegrasikan ke references/) |
| **Folder references/** | 4 file utama + folder script-library (10 file) | 3 file (hook patterns, script outline, scoring guide) |
| **Brand Profile system** | Ada (onboarding 10 pertanyaan, file dokumen) | Tidak ada (cukup 3-4 pertanyaan ad-hoc) |
| **Mode kerja** | 6 mode (buat copy, kritik, arahan ide, develop caption, suggest struktur, compression) | 3 capability (hook, outline, skor) |
| **Format output** | Per platform spesifik (Reels, TikTok, Carousel, Stories, Single Image) dengan rules format | Generic markdown di chat |
| **Iterasi** | Konsultatif multi-round | One-shot |
| **Script library** | 200 script viral dengan 1000+ pattern | Subset terbatas 10 hook patterns + 5 struktur outline |
| **Humanize standards** | Zero tolerance Tier 1 + Tier 2 lengkap | Zero tolerance Tier 1 + Tier 2 lengkap (copy persis dari Lyra full) |

---

## Yang Sama antara Mini Lyra dan Lyra Full

- **Humanize standards**: file `standards/humanize-writing-guide.md` di Mini Lyra adalah copy persis dari `standards/humanization-standards.md` di Lyra full. Zero tolerance tetap berlaku.
- **Persona inti**: nama Lyra (versi Mini), tone personal-hangat-profesional, tajam secara strategi.
- **Komitmen kualitas**: walaupun scope ringan, output harus tetap pintar dan menggigit. Hindari pola generic AI.

---

## Yang Diturunkan (Disederhanakan)

- **Hook patterns**: dari hook-retention.md Lyra full yang punya 30+ pattern, Mini Lyra ambil 10 pattern paling versatile dan anti-klise.
- **Script outline**: dari storytelling-framework.md + script-pattern-overview.md, Mini Lyra ambil 5 struktur paling umum untuk short-form.
- **Diagnostic**: dari Mode 2 Lyra full (Kritik/Review) yang punya deep evaluation per kalimat, Mini Lyra ambil format skoring 1-10 + 3-5 poin per kategori, tanpa rewrite.

---

## Yang Eksklusif Lyra Full (TIDAK Ada di Mini Lyra)

- **Brand Profile System lengkap** (onboarding 10 pertanyaan, dokumen permanen)
- **6 mode kerja lengkap** (buat copy dari nol, kritik/review per kalimat, arahan ide, develop caption, suggest struktur, compression)
- **Format output per platform spesifik** (Reels vs TikTok beda treatment, Carousel rules, Stories rules, dll)
- **Heuristic bias deep mapping** (per audience, per industri, per objective)
- **Strategic pillar alignment check**
- **TTA (Trigger to Action) mapping**
- **Script library lengkap** (200 script viral dengan 1000+ pattern terdokumentasi)
- **Direct response copywriting framework** (untuk performance content)
- **Storytelling framework lengkap** (story loops, anatomi, applikasi)
- **Content psychology framework** (mekanisme kognitif lengkap)
- **Multi-format examples**
- **Adaptasi gaya bahasa dari Brand Profile**
- **Iterasi konsultatif multi-round**
- **Output siap publish per platform**

---

## Eksklusif Mini Lyra (TIDAK Ada di Lyra Full)

- **Format skoring numerik 1-10**: Lyra full kasih kritik mendalam tapi tanpa skor numerik. Mini Lyra justru kasih skor sebagai verdict cepat.
- **Onboarding ringan ad-hoc**: 3-4 pertanyaan per request, tidak disimpan sebagai dokumen. Cocok untuk one-shot interaction.
- **Anchor playbook eksplisit di setiap output**: setiap output Mini Lyra rujuk bab playbook spesifik. Lyra full tidak punya pattern ini karena positioning-nya beda.
- **Built-in upsell pattern**: setiap output ditutup dengan offering ke Lyra full. Lyra full tidak punya pattern ini.

---

## Catatan untuk Pemilik Skill

Link Lyra full sudah di-set ke `https://nakama-creative-lab.myscalev.com/lyra-ai` di:

- SKILL.md (3 kali, untuk 3 capability di template output)
- README.md (1 kali di section "Kapan Upgrade ke Lyra Full")

Kalau link berubah di masa depan, cari-replace string `nakama-creative-lab.myscalev.com/lyra-ai` di file-file di atas.
