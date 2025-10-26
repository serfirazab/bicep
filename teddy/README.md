# Teddy Egzersizi (Database)

Bu klasörde veritabanı ile ilgili bir egzersiz bulunur.

İçerik:
- `main.bicep` — ana dağıtım dosyası.
- `modules/database.bicep` — veritabanı kaynaklarını oluşturan modül.

Amaç:
- Veritabanı sunucusu, veritabanı örneği ve bağlantı bilgilerini güvenli şekilde konfigüre etmek.

Dağıtım örneği:
```powershell
az deployment group create --resource-group <rg-name> --template-file .\main.bicep
```

Güvenlik:
- Sensitive (secret) değerler için Key Vault kullanımı önerilir.
