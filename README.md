# CÓDIGO CERO · Ayuda inmediata

Herramienta comunitaria estática para San Patricio del Chañar y zonas rurales cercanas (alcance de diseño inicial: aproximadamente 40 km). No es un sistema oficial de despacho.

## Funciones actuales
- Accesos a **103 y 105**: fuentes oficiales provinciales difieren sobre el número de Defensa Civil (Ministerio de Seguridad publica 103; Policía de Neuquén publica 105). La discrepancia queda visible y debe resolverse con validación local antes de difundir.
- Acceso directo a 107 (emergencias médicas), 100 (Bomberos) y 101 (Policía).
- Contactos locales directos separados y etiquetados como pendientes de confirmación: Hospital 0299 485-5084; Comisaría 13.ª 0299 485-5236; Seguridad Ciudadana municipal 0299 458-4229.
- Selector de tipo de emergencia y sector territorial.
- Ubicación del navegador si el usuario la autoriza, con precisión aproximada y enlace de mapa.
- Mensaje corto para copiar, compartir o abrir WhatsApp.
- Service worker para volver a abrir la página después de haberla cargado con conexión.
- Diseño adaptable a celular, tableta y computadora, con botones grandes y controles accesibles.

## Activar GitHub Pages
1. Abrí **Settings** del repositorio.
2. Entrá en **Pages**.
3. En **Build and deployment**, elegí **Deploy from a branch**.
4. Seleccioná la rama `main` y la carpeta `/ (root)`.
5. Guardá y esperá a que GitHub publique el sitio.

URL prevista: https://eliasmartinezcultural-glitch.github.io/C-DIGO-CERO/

## Documentación técnica
- [Plan operativo y arquitectura](PLAN-OPERATIVO.md)
- [Investigación de conectividad y radiobases](MAPA-CONECTIVIDAD.md)

## Límites técnicos y de seguridad
- No se conecta a torres celulares, no puede leer cobertura de operadoras ni activar redes de emergencia.
- El GPS del navegador requiere permiso y normalmente un contexto seguro HTTPS; puede ser impreciso o no estar disponible.
- Los enlaces `tel:` abren el marcador del dispositivo; no garantizan que la llamada conecte. La posibilidad de llamada de emergencia sin saldo depende de la red y el operador.
- WhatsApp se abre con un texto preparado. La persona debe elegir destinatario y enviar; no existe recepción ni confirmación automática.
- No hay central de monitoreo, base de datos, notificaciones push, despacho ni rastreo de personas.
- Sin señal de telefonía y sin Wi-Fi no se puede garantizar llamada ni envío. Los mapas externos necesitan conexión.
- La caché offline depende del navegador, almacenamiento y de que la página haya cargado previamente. No sustituye mapas offline descargados ni un plan de evacuación.
- El radio de 40 km es una prioridad de diseño, no una geocerca ni garantía de cobertura.
- No se deben publicar refugios, rutas de evacuación, puntos de reunión o números personales sin validación de las autoridades responsables.

## Antes de difundir a la comunidad
1. **Validación institucional:** pedir revisión a Defensa Civil municipal/provincial, hospital, Policía y Bomberos.
2. **Verificar teléfonos:** llamar en horario apropiado a cada institución para confirmar número, nombre del servicio y disponibilidad. En particular, validar los contactos directos mostrados en la web.
3. **Canal real de recepción:** acordar un teléfono/WhatsApp institucional atendido, quién responde, horarios, suplencias, privacidad y qué hacer si no se recibe el mensaje. Publicarlo solo con autorización.
4. **Prueba de dispositivos:** Android, iPhone y computadora; pantalla chica, texto grande, teclado, GPS permitido/denegado y conexión lenta.
5. **Prueba offline:** cargar online, abrir de nuevo en modo avión y comprobar qué queda accesible. Confirmar que la interfaz no sugiera que se puede enviar sin señal.
6. **Prueba de emergencia simulada:** nunca probar con llamadas reales a números de emergencia; validar enlaces con los organismos de manera coordinada.
7. **Revisión territorial:** validar nombres de barrios, chacras, picadas, accesos y referencias con gente que conoce la zona.
8. **Responsable de mantenimiento:** definir quién revisa los teléfonos, enlaces y mensajes oficiales, y con qué frecuencia.

## Seguridad junto al río
Alejarse de la costa, canales y zonas anegadas. No cruzar agua a pie ni en vehículo. Buscar un lugar alto y seguro únicamente si se puede llegar sin exponerse. Seguir instrucciones oficiales.

## Estado
Prototipo mejorado. No es oficial ni está conectado a un centro de recepción. No presentarlo como servicio de rescate ni como garantía de ayuda hasta que los organismos validen el contenido y exista un canal de recepción probado.