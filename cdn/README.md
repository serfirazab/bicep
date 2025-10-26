# CDN Egzersizi

Bu klasör CDN kaynaklarıyla ilgili bir egzersiz içerir.

İçerik:
- `main.bicep` — CDN dağıtımı için ana şablon.
- `modules/` — `app.bicep` ve `cdn.bicep` gibi alt modüller.

Amaç:
- Azure CDN profil ve endpoint oluşturma.
- Statik içeriği cachelemek ve dağıtımı yapılandırmak.

Hızlı dağıtım örneği (PowerShell):
```powershell
# Resource group seviyesinde deploy
az deployment group create --resource-group <rg-name> --template-file .\main.bicep
```

Notlar:
- Gerekli parametreler `main.bicep` içinde veya ayrı parametre dosyasında bulunabilir.
- Varsayılan olarak modüller `modules/` altında toplanmıştır.
