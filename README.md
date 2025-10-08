# octra-vps-setup
A guide for quickly installing and configuring the testnet client for the Octra FHE blockchain on a Virtual Private Server (VPS). Includes steps for secure and continuous operation using python venv and screen commands.

# Octra Testnet İstemcisi VPS Kurulum Rehberi

Bu rehber, Octra Testnet istemcisini bir Sanal Özel Sunucu (VPS) üzerine kurmak, yapılandırmak ve **GNU Screen** kullanarak SSH oturumundan bağımsız olarak arka planda çalıştırmak için gerekli adımları özetler.

## ⚠️ ÖNEMLİ UYARI
Bu kurulum, Octra tarafından sağlanan komutlara dayanır ve testnet katılımı amaçlıdır. Cüzdan özel anahtarlarınızı (priv) her zaman güvenli bir yerde saklayın.

---

## 1. Ön Koşullar (VPS)

* **İşletim Sistemi:** Yeni bir Linux tabanlı VPS (Ubuntu 22.04+ veya Debian önerilir).
* **Erişim:** VPS'inize SSH ile erişim.
* **Gereksinimler:** Python 3, `git`, `pip` ve **`screen`** yüklü olmalıdır.

Eğer `screen` yüklü değilse, aşağıdaki komutla kurabilirsiniz (Debian/Ubuntu için):
```bash
sudo apt update && sudo apt install screen -y
