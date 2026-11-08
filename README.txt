LED Remote para Android — proyecto inicial

IMPORTANTE
- Este ZIP contiene el PROYECTO FUENTE Android, no un APK compilado.
- Los patrones IR están vacíos intencionalmente: todavía no se han identificado los códigos exactos de tu control.
- Por eso la interfaz abre, pero las luces no responderán hasta completar IrCodes.patterns.
- El emisor IR del POCO transmite; no puede recibir/aprender las señales del mando original.

CÓMO GENERAR EL APK
1. Instala Android Studio en una computadora.
2. Abre la carpeta LEDRemote como proyecto.
3. Deja que Gradle sincronice y descargue los componentes.
4. Conecta un teléfono Android o usa Build > Build Bundle(s) / APK(s) > Build APK(s).
5. Instala el APK generado en el POCO X7 Pro.

CÓDIGOS IR
El archivo app/src/main/java/com/example/ledremote/MainActivity.kt contiene IrCodes.
Cada botón necesita un patrón de duraciones en microsegundos a 38 kHz.
No rellenes con códigos al azar. Para obtenerlos hace falta un receptor IR externo,
un analizador compatible, o una base de datos fiable para el modelo exacto del mando/controlador.
