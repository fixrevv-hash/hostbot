# Hosting bot - versi bersih

## Environment variable
| Env | Wajib | Keterangan |
|---|---|---|
| BOT_TOKEN | ya | token bot panel (WAJIB token baru, yang lama anggap bocor) |
| OWNER_ID | sangat disarankan | ID Telegram Anda. Jika kosong, orang pertama yang /start jadi owner |
| BRAND_NAME / BRAND_VERSION | tidak | nama panel |
| SUPPORT_USERNAME | tidak | contoh @admin_anda |
| UPDATE_CHANNEL | tidak | link channel update |
| PAY_BKASH_NUMBER, PAY_NAGAD_NUMBER, PAY_ROCKET_NUMBER, PAY_UPAY_NUMBER, PAY_BINANCE_ID, PAY_BANK_INFO | tidak | info pembayaran Anda |

Ubah juga link referral `https://t.me/your_bot?start=` di bot.py (cari `your_bot`).

## Catatan
- Grup wajib-join, backup GitHub/Telegram diatur dari panel admin (bukan hardcode).
- Folder `fonts/` dipakai untuk captcha, jangan dihapus.
- Kunci cache lokal diturunkan dari `BOT_TOKEN|OWNER_ID`; mengganti keduanya membuat cache lama tak terbaca (kunci di GitHub key vault tetap aman).
