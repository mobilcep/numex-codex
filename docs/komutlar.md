# ⌨️ Komutlar ve Kısayollar

## Codex CLI

| Komut | Açıklama |
|---|---|
| `numex` | Etkileşimli terminal sohbeti (REPL) |
| `numex basla` | Giriş + başlangıç menüsü (terminal sohbeti / web'den PC kontrolü) |
| `numex login` | Tarayıcı onaylı cihaz girişi |
| `numex "<görev>"` | Tek seferlik görev |
| `numex plan "<görev>"` | Mimar planlayıcı — kod değiştirmez |
| `numex mission "<görev>"` | İzole sandbox çalışma alanlarında uzun süreli otonom misyon |
| `numex undo` | Son turu geri al |
| `numex --devam` | Son oturumdan devam et |
| `numex --offline "<görev>"` | Yerel Ollama ile internetsiz çalış |
| `numex --api-key nx_live_…` | API anahtarı tanımla |
| `numex --version` | Sürüm |
| `numex uzak` | Uzaktan PC köprüsünü başlat (terminal açık kalır) |
| `numex uzak install` | Köprüyü arka plan servisi olarak kur (sistem tepsisi) |
| `numex uzak pause` | Köprüyü duraklat |

### REPL içi komutlar

| Komut | Açıklama |
|---|---|
| `/yardim` | Yardım |
| `/cikis` | Çıkış |
| `/model fast \| pro \| code` | Aktif profili kilitle |
| `/proje "C:\yol\proje"` | Belirli bir projeye geç (proje hafızası yüklenir) |

### Konseyi çağırma ifadeleri
*"konseyi topla"* · *"ajanları çağır"* · *"ekibi topla"* · *"takımı çağır"* · *"herkesi topla"* ·
*"hep birlikte bak"* · *"swarm council"*

## Codex IDE / VS Code eklentisi

### Kısayollar

| Kısayol | İşlev |
|---|---|
| `Ctrl+Alt+M` | Sohbeti aç/kapat |
| `Ctrl+Alt+N` | Seçimi sor |
| `Ctrl+K` | Satır içi düzenle |
| `Tab` | Sonraki düzenleme önerisini uygula |

### Komut paleti (`Ctrl+Shift+P` → "Numex")

| Grup | Komutlar |
|---|---|
| **Başlangıç** | Hoş Geldiniz · Bu klasörde çalış · Çalışma klasörü seç / sıfırla · Giriş / Çıkış |
| **Sohbet** | Sohbeti Aç/Kapat · Sohbet Paneli · Yeni Sohbet · Sohbet Geçmişi · Transkripti Dışa Aktar · Son Yanıtı Tekrar Üret |
| **Kod** | Seçimi Sor · Bu Dosya Hakkında Sor · Seçimi Açıkla · Kod Lens Sorgusu · Satır-içi Düzenle · Sonraki Düzenlemeyi Uygula / Kapat · Dosyadaki Hataları AI ile Düzelt · Composer |
| **Kod tabanı** | Projeyi İndeksle · Yeniden İndeksle (leksikal) · Anlamsal Aramayı Aç · Kod Tabanında Ara |
| **Görsel** | Ekran Görüntüsü Al ve Sohbete Ekle · Tarayıcıyı Aç · Design Mode |
| **Terminal** | Terminal Komutu Üret (doğal dil) · Terminal Çıktısını Sohbete Gönder |
| **Git** | Commit Mesajı Üret · Değişiklikleri İncele (AI) · Pull Request Aç |
| **Ajanlar** | Otonom Modu Aç/Kapat · Arka Plan Ajanı · Bulut Ajanı |
| **Uzak** | Uzak Sunucuya Bağlan · SSH ile Bağlan · WSL ile Bağlan |
| **Diğer** | Ayarlar · Ekran Dilini Seç · Güncellemeleri Denetle · Destek / Hata Bildir |

### Eklenti ayarları

| Ayar | Varsayılan | Açıklama |
|---|---|---|
| `numex.command` | `numex` | CLI komutu veya tam yolu |
| `numex.extraArgs` | — | REPL başlatma argümanları (ör. `--yolo --lint`) |

## Codex Web

| Kısayol | İşlev |
|---|---|
| `Ctrl+N` / `Ctrl+Shift+N` | Yeni proje / yeni dosya |
| `Ctrl+O` | Proje aç |
| `Ctrl+S` / `Ctrl+Shift+S` | Kaydet / tümünü kaydet |
| `Ctrl+Shift+P` | Yayınla |
| `Ctrl+K` | Komut paleti |
| `Ctrl+B` | Dosya gezgini |
| `Ctrl+F` / `Ctrl+H` | Bul / değiştir |
| `F11` | Tam ekran |
| `Ctrl+Shift+K` | Klavye kısayolları |

---
← [Ana sayfa](../README.md)
