# igd-anamnesa-templates

Template anamnesa (KU, RPS, RPD, alergi, RPO) untuk bookmarklet "Isi Anamnesa & PE" di EMR IGD.
Bookmarklet mengambil `anamnesa-templates.json` dari repo ini setiap dibuka; edit file ini, tidak perlu bookmark ulang.
Tanpa data pasien. Jangan isi nama/RM/identitas apa pun di sini.

## Format
```json
{
  "version": 1,
  "default": { "rpd": "...", "alergi": "...", "rpo": "..." },
  "templates": {
    "Nama pilihan": {
      "alias": ["kata kunci", "dx"],
      "ku": "Keluhan utama",
      "rps": "Teks RPS (\n untuk baris baru)",
      "rpd": "opsional, menimpa default",
      "alergi": "opsional",
      "rpo": "opsional"
    }
  }
}
```
