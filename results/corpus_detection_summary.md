# Aletheia Prism — Corpus Detection Summary

**Mensor XAI | EAIVP Forensic Analysis Platform**

---

## Validation Overview

| Metric | Value |
|---|---|
| Total samples analysed | 422 |
| Malware families | 21 |
| Overall detection rate | 97.9% |
| Families at 100% detection | 16 |
| Detection threshold | MEDIUM or above (Aletheia Prism triad) |
| Corpus source | MalwareBazaar (community-curated, tagged samples) |
| Analysis date | March 2026 |
| Analysis engine | Aletheia Prism — Lens A + Lens B + Lens C combined verdict |

---

## Per-Family Results

| Family | Category | Detected | Samples | Rate |
|---|---|---|---|---|
| AsyncRAT | Remote Access Trojan | 20 | 20 | 100% |
| BlackCat | Ransomware | 20 | 20 | 100% |
| CobaltStrike | Post-Exploitation Framework | 20 | 20 | 100% |
| Conti | Ransomware | 20 | 20 | 100% |
| DarkComet | Remote Access Trojan | 20 | 20 | 100% |
| Dridex | Banking Trojan | 20 | 20 | 100% |
| Emotet | Loader / Botnet | 20 | 20 | 100% |
| GuLoader | Loader / Downloader | 20 | 20 | 100% |
| IcedID | Banking Trojan | 20 | 20 | 100% |
| LockBit | Ransomware | 20 | 20 | 100% |
| Mirai | Botnet | 23 | 23 | 100% |
| RedLine | Information Stealer | 19 | 19 | 100% |
| TrickBot | Banking Trojan / Loader | 20 | 20 | 100% |
| Vidar | Information Stealer | 20 | 20 | 100% |
| WannaCry | Ransomware | 20 | 20 | 100% |
| njRAT | Remote Access Trojan | 20 | 20 | 100% |
| AgentTesla | Information Stealer | 19 | 20 | 95% |
| Ryuk | Ransomware | 19 | 20 | 95% |
| XWorm | Remote Access Trojan | 19 | 20 | 95% |
| Stealc | Information Stealer | 18 | 20 | 90% |
| FormBook | Information Stealer | 16 | 20 | 80% |
| **TOTAL** | | **413** | **422** | **97.9%** |

---

## Category Summary

| Category | Families | Overall Rate |
|---|---|---|
| Ransomware | BlackCat, Conti, LockBit, Ryuk, WannaCry | 95–100% |
| Remote Access Trojans | AsyncRAT, DarkComet, njRAT, XWorm | 95–100% |
| Information Stealers | AgentTesla, RedLine, Stealc, Vidar, FormBook | 80–100% |
| Banking Trojans / Loaders | Dridex, Emotet, GuLoader, IcedID, TrickBot | 100% |
| Post-Exploitation | CobaltStrike | 100% |
| Botnet | Mirai | 100% |

---

## Methodology Notes

- All samples sourced from MalwareBazaar, a public community threat intelligence platform operated by abuse.ch
- Detection threshold is MEDIUM or above across the combined Aletheia Prism verdict
- Lens B (Pixel Space) is not applicable to EXE, DLL, or ZIP file types — correct by design
- FormBook at 80% is the only family below 90% and is reported without adjustment
- Results represent honest, uncontaminated analysis — no figures have been inflated

---

## Known Limitations

- Lens B pixel-space analysis applies to image files only; not a factor in EXE/DLL/ZIP detection
- Highly obfuscated or padded samples may reduce entropy signal strength in Lens A
- File-type-aware entropy baselines are on the development roadmap and will improve precision further

---

*EAIVP — Aletheia Prism · Corpus Detection Summary · March 2026 · Mensor XAI*
