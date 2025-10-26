# HR (Human Resources) Egzersizi

Bu klasör, parametre yönetimi ve ortam (örn. dev) bazlı dağıtım örneği içerir.

İçerik:
- `main.bicep` — uygulamanın ana şablonu.
- `main.parameters.dev.json` — örnek development parametreleri.

Amaç:
- Farklı ortamlar için parametre dosyası kullanımı.
- Modüler ve yeniden kullanılabilir Bicep şablonları ile güvenli değişken yönetimi.

Dağıtım örneği:
```powershell
az deployment group create --resource-group <rg-name> --template-file .\main.bicep --parameters @main.parameters.dev.json
```

Notlar:
- Parametre dosyalarını ortam bazlı olarak çoğaltabilirsiniz (dev/staging/prod).
