# Investigación de conectividad — CÓDIGO CERO

## Nota de verificación de emergencias
Las fuentes oficiales provinciales consultadas discrepan en el número de Defensa Civil: el Ministerio de Seguridad publica 103, mientras que el sitio de la Policía de Neuquén publica 105. La web incluye ambos accesos y pide confirmación local. No presentar uno como universalmente confirmado hasta que la autoridad operativa local lo resuelva.

## Para qué sirve
Documentar fuentes públicas para estudiar cobertura y radiobases alrededor de San Patricio del Chañar y orientar una futura coordinación con operadores y organismos. Esta investigación no certifica la cobertura real de cada picada ni permite conectar la web a una torre.

## Fuentes públicas para explorar
1. **ENACOM — Infraestructura de Datos Espaciales de Comunicaciones (IDECOM)**  
   https://www.argentina.gob.ar/telecomunicaciones-y-conectividad/infraestructura-de-datos-espaciales-de-comunicaciones  
   Describe capas geográficas que pueden incluir radiobases/antenas móviles 2G/3G/4G, fibra y nodos, conectividad rural en 450 MHz y otros servicios. Hay que abrir el visor y comprobar qué capas y fechas están disponibles.

2. **ENACOM — Mapa de conectividad**  
   https://indicadores.enacom.gob.ar/Mapas/conectividad  
   Permite filtrar por provincia, departamento/localidad y tecnologías/servicios informados por los prestadores. ENACOM lo identifica como beta y orientativo; la ausencia de un dato no demuestra que no haya conectividad.

3. **ENACOM — Indicadores y datos abiertos**  
   https://indicadores.enacom.gob.ar/  
   Contiene estadísticas y mapas georreferenciados de servicios TIC. Sirve para contexto de conectividad, no como medidor en tiempo real de una persona.

4. **COPADE Neuquén — Sistema de Información Geográfica (SIG)**  
   https://www.copade.gob.ar/sig/  
   Visor geográfico provincial con información territorial, infraestructura social y gestión del riesgo, útil para cruzar contexto territorial público con los puntos de conectividad.

5. **Municipalidad de San Patricio del Chañar — ubicación y accesos**  
   https://www.sanpatricio.gob.ar/llegar  
   Referencia institucional sobre rutas y acceso al ejido. No reemplaza cartografía operativa ni instrucciones de evacuación.

## Cómo hacer el relevamiento de 40 km
1. Abrir IDECOM y el mapa de conectividad de ENACOM desde una computadora con conexión.
2. Localizar San Patricio del Chañar y estudiar un área aproximada de 40 km alrededor; conservar la escala y la fecha de cada capa.
3. Registrar, cuando estén disponibles, proveedor, tecnología, tipo de infraestructura, coordenadas, fuente, fecha de actualización y nivel de precisión. No convertir una capa de antenas en una promesa de cobertura.
4. Cruzar con los sectores que realmente necesita la herramienta: casco urbano, barrios, ribera, chacras, picadas, RP 7/RP 8, zona del dique y accesos rurales.
5. Pedir a cada operador una confirmación escrita de cobertura y procedimiento de contingencia para la zona. Solicitar también información sobre fallas, respaldo eléctrico y continuidad, si el operador puede compartirla.
6. Hacer pruebas de campo autorizadas con varios operadores/SIM en puntos representativos, en diferentes horarios y condiciones. Registrar si hay llamada, SMS y datos por separado; no publicar números de abonados ni datos personales.
7. Compartir el resultado con Defensa Civil y el municipio para acordar qué zonas son críticas y cómo describirlas. No publicar puntos vulnerables ni rutas de evacuación sin validación institucional.

## Lo que una web puede y no puede hacer
- Puede solicitar ubicación al GPS/sistema del teléfono cuando la persona lo autoriza, preparar un mensaje, abrir un mapa externo y comprobar de forma muy básica si el navegador cree que está conectado a una red.
- El estado `navigator.onLine` no mide la potencia de señal, no confirma acceso real a internet y no indica a qué torre está conectado el teléfono.
- Una página web ordinaria no obtiene la identidad de la antena celular ni puede forzar que el equipo cambie de torre, encender repetidores, dar prioridad a una llamada o activar alertas masivas.
- Los servicios de localización por red que el sistema operativo pueda usar son administrados por el dispositivo/plataforma y no equivalen a una API pública de torres.
- La integración con radiobases, alertas celulares, centros de despacho o redes de emergencia exige participación y autorización de operadores y organismos responsables.

## Decisión técnica recomendada
Mantener CÓDIGO CERO como una página estática, ligera y de uso voluntario. Agregar enlaces a mapas públicos de conectividad para la planificación del equipo, pero no depender de ellos durante una emergencia. La ayuda inmediata debe seguir funcionando como interfaz aun cuando el mapa no cargue: llamadas, referencia escrita y mensaje corto.

## Fuentes consultadas
- ENACOM, Infraestructura de Datos Espaciales de Comunicaciones: https://www.argentina.gob.ar/telecomunicaciones-y-conectividad/infraestructura-de-datos-espaciales-de-comunicaciones
- ENACOM, Mapa de conectividad: https://indicadores.enacom.gob.ar/Mapas/conectividad
- ENACOM, portal de indicadores: https://indicadores.enacom.gob.ar/
- COPADE Neuquén, SIG: https://www.copade.gob.ar/sig/
- Municipalidad de San Patricio del Chañar, ubicación: https://www.sanpatricio.gob.ar/llegar
