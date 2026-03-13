# 🛡️ Suggy Safe Repos — Sistema de Rollback

## Cómo funciona
Si una actualización nueva falla, Suggy descarga automáticamente de los repos safe.

## Repos
| Repo | Tipo | URL |
|------|------|-----|
| suggy-apk-releases | 🆕 Última versión Admin | version.json → última |
| suggy-apk-safe | 🛡️ Versión segura Admin | version.json → safe |
| suggy-client-releases | 🆕 Última versión Client | version.json → última |
| suggy-client-safe | 🛡️ Versión segura Client | version.json → safe |

## Flujo de actualización
1. APK chequea version.json del repo principal
2. Si hay nueva versión → descarga e instala
3. Si la nueva falla → descarga de repo safe automáticamente
4. Al confirmar que nueva versión funciona → copiar a repo safe
