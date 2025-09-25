# Asterisk + Postfix Gmail Relay Configs

Repo này chứa cấu hình mẫu để:
- Triển khai **Asterisk VoIP PBX**
- Tích hợp **Postfix mail relay qua Gmail** (dùng cho voicemail gửi email)

## Nội dung
- `asterisk/` : Cấu hình Asterisk (sip.conf, extensions.conf, voicemail.conf)
- `postfix/` : Cấu hình Postfix relay Gmail
- `docs/`    : Hướng dẫn chi tiết cài đặt & cấu hình

## Yêu cầu
- Ubuntu 20.04 / Debian 11
- Asterisk 18+
- Postfix
- Gmail account (bật App Password nếu có 2FA)

## Cách dùng
1. Copy file cấu hình vào `/etc/asterisk/` và `/etc/postfix/`
2. Reload dịch vụ:
   ```bash
   sudo systemctl restart asterisk
   sudo systemctl restart postfix
