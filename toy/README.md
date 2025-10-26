# Toy Egzersizi (App Service)

Bu klasör App Service veya uygulama servisleri ile ilgili bir egzersiz içerir.

İçerik:
- `main.bicep` — App Service kaynaklarını oluşturan ana şablon.
- `modules/appService.bicep` — app service ile ilgili modül.

Amaç:
- App Service Plan ve App Service oluşturma.
- Uygulama ayarları, bağlantı stringleri ve yapılandırma ile entegre etmek.

Dağıtım örneği:
```powershell
az deployment group create --resource-group <rg-name> --template-file .\main.bicep
```

Notlar:
- Deploy öncesi `plan` ve `sku` gibi parametreleri kontrol edin.
