# CÓDIGO CERO — Plan operativo y arquitectura

## Objetivo
Reducir los pasos entre detectar peligro y comunicar un pedido claro en San Patricio del Chañar y su zona rural cercana. La interfaz debe ser rápida, legible, tolerante a errores y usable con una sola mano.

## Capas del sistema
1. **Interfaz de emergencia:** llamadas telefónicas y advertencias prioritarias; no requiere completar datos.
2. **Localización voluntaria:** permiso explícito del navegador; muestra coordenadas y precisión aproximada. El usuario puede rechazar el permiso y escribir una referencia.
3. **Contexto territorial:** sector seleccionado y referencia de terreno (barrio, picada, chacra, ruta, kilómetro, ribera o punto conocido).
4. **Composición local del mensaje:** el texto se crea en el dispositivo. No se transmite a un servidor ni queda guardado por la página.
5. **Salida manual:** copiar, compartir mediante el menú del sistema o abrir WhatsApp con el texto. El usuario confirma destinatario y envío.
6. **Caché de lectura:** service worker para volver a abrir los archivos estáticos después de una carga online inicial.
7. **Gobernanza pendiente:** validación de contactos, canal de recepción, protocolo de respuesta y mantenimiento por instituciones responsables.

## Torres, cobertura y comunicaciones
Una web común no puede conectarse directamente a torres celulares, solicitar triangulación de antenas ni consultar la cobertura privada de una operadora. El teléfono elige la red disponible y el navegador solo puede pedir servicios autorizados por el sistema, como geolocalización. Para alertas celulares masivas o integración con centrales se requiere acuerdo y tecnología del operador/organismo competente. No simular estas capacidades en la interfaz.

## Datos y privacidad
- No pedir nombre, DNI ni datos sensibles si no son necesarios.
- No solicitar ubicación hasta que la persona pulse el botón.
- No enviar coordenadas a ningún servidor propio.
- El enlace del mapa y el mensaje pueden revelar ubicación si el usuario decide compartirlos.
- Evitar almacenar incidentes o construir un mapa público de personas en riesgo.
- Cualquier futuro registro de reportes requiere evaluación de privacidad, acceso restringido, retención limitada y responsables claros.

## Prioridad territorial
Área de diseño inicial: San Patricio del Chañar y aproximadamente 40 km alrededor. El alcance es orientativo; el formulario deja que la persona elija el sector. No se debe afirmar que un evento está dentro del radio exacto sin una georreferencia validada. Para cada incidente rural, pedir una referencia humana útil además del GPS.

## Próximas fases recomendadas
### Fase 1 — Verificación local
- Confirmar teléfonos de Defensa Civil, salud, Bomberos, Policía y Seguridad Ciudadana.
- Validar nombres de barrios, caminos, picadas y accesos rurales.
- Conseguir aprobación de los organismos para textos preventivos.

### Fase 2 — Recepción real
- Acordar un WhatsApp/teléfono institucional atendido.
- Definir responsable principal, suplente, horario, protocolo de lectura y escalamiento.
- Mostrar con claridad cuándo el canal no está monitoreado.
- No presentar WhatsApp como despacho automático ni prometer tiempos de respuesta.

### Fase 3 — Mapa territorial seguro
- Incorporar solo capas públicas o autorizadas: localidades, caminos, centros de salud y puntos de referencia verificados.
- Evitar publicar ubicaciones de personas, refugios no confirmados o rutas de evacuación no aprobadas.
- Incluir enlaces a mapas externos y, si se aprueba, recursos offline descargables y fechados.

### Fase 4 — Pruebas
- Android/iOS, navegadores principales, teclado, lectores de pantalla, alto contraste, batería baja y conexión inestable.
- Permiso GPS permitido, denegado, timeout y precisión baja.
- Modo avión después de cargar la página.
- Simulacros controlados sin llamar a números de emergencia reales.

## Criterios de aceptación
- La llamada prioritaria se ve sin desplazarse en móvil.
- Ninguna función exige GPS para pedir ayuda.
- El mensaje generado es breve, claro y editable.
- No se afirma que el mensaje se envió o fue recibido hasta que la persona/organismo lo confirme.
- El estado de conexión nunca se interpreta como confirmación de cobertura de emergencia.
- Los teléfonos directos locales no se consideran definitivos hasta validación institucional.
