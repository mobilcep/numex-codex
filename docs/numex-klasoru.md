# 🧠 `.numex/` — Ajanın Şeffaf Hafızası

Codex, her projede **açık ve okunabilir** bir `.numex/` klasörü tutar. Ajanın ne bildiği ve ne
yaptığı bir kara kutuda değil, **senin diskinde, düz dosyalarda** durur.

| Dosya / klasör | İçerik |
|---|---|
| `rag/index.json` · `rag/graph.json` · `rag/symbols.json` · `rag/summary.md` | Kod tabanı indeksi, bağımlılık grafiği, sembol tablosu, proje özeti |
| `audit/audit-trail.jsonl` | Ajanın yaptığı **her işlemin** zaman damgalı denetim kaydı |
| `checkpoints/stack.json` · `checkpoints/redo.json` | Geri al / yinele noktaları (`numex undo`) |
| `mission-state.json` · `async-tasks.json` | Süren otonom misyonlar ve arka plan görevleri |
| `agent-registry.json` · `services.json` | Kayıtlı ajanlar ve çalışan servisler (ör. geliştirme sunucusu) |
| `learned-errors.json` · `rag/error-kb-local.json` | Bu projede öğrenilen hatalar ve çözümleri |
| `chronicle.jsonl` · `digest.md` | Oturum günlüğü ve özet |
| `project-map-cache.json` | Proje haritası önbelleği |
| `telemetry/token-usage.jsonl` · `sessions/*-usage.json` | Token kullanımı |
| `economy-state.json` | Bütçe / maliyet durumu |
| `logs/` | Ajan logları |

## Neden önemli?

- **Denetlenebilirlik:** "Dün bu projeye ne oldu?" → `audit-trail.jsonl`.
- **Süreklilik:** Projeyi kapatıp açtığında ajan projeyi yeniden öğrenmez, kaldığı yerden devam eder.
- **Öğrenme:** Aynı hatayı ikinci kez yaşamamak için çözümler projeye özel saklanır.
- **Sahiplik:** Hafıza senin projende; istersen okursun, istersen silersin.

> İpucu: `.numex/` klasörünü `.gitignore`'a ekleyebilir ya da ekip arkadaşlarınla indeksi paylaşmak
> için bazı dosyalarını depoda tutabilirsin.

---
← [Ana sayfa](../README.md)
