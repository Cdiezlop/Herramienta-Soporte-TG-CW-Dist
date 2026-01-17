# Herramienta de Gestión - Analista Conectividad B2B

## Información General
Esta herramienta es una solución de software diseñada para agilizar la tipificación, diagnóstico y reporte de incidentes en el área de conectividad. El código fuente ha sido ofuscado para garantizar la seguridad de la lógica de negocio y reducir el tamaño de los archivos para su distribución.

## Instrucciones de Ejecución
1. Asegúrese de que todos los archivos (HTML, CSS y JS) estén en la misma carpeta.
2. Haga doble clic en el archivo index.html.
3. La herramienta se abrirá en su navegador web predeterminado.
4. Si aparece la pantalla de bloqueo, contacte al administrador. 

## Funcionalidades Principales
- Generación automática de plantillas para notas de casos (Incidencias y Requerimientos).
- Botones de copiado rápido para identificadores corporativos y resúmenes de llamadas.
- Llenar plantillas generales en base a los datos ingresados.
- Tener las credenciales a la mano, para agilizar el ingreso a los aplicativos. 

## Historial de Versiones

A continuación se describe la evolución de la herramienta hasta la versión actual distribuida.

### Versión 0001 - Funcionalidad Base
Esta fue la versión inicial de la herramienta. Sus características incluían:
- Estructura básica de formulario para ingreso de datos del cliente.
- Botones simples para copiar al portapapeles.
- Generación de guiones básicos de diagnóstico N1. (Solo para N1)
- Interfaz con campos de texto estándar sin validación geográfica avanzada.
- Gestion de claves para ingreso de aplicativos, todo guardado de manera local.

### Versión 001 - Funcionalidad NE. 
Esta fue la versión inicial de la herramienta. Sus características incluían:
- Todas las funcionalidades de la V0001, ademas esta contiene la busqueda del NE importando el archivo, y descargar el word con hora y fecha actualizada. Despues de importar una plantilla de word. 

### Versión 002 - Actualización Geográfica y Estructural
Esta actualización representa una reingeniería importante de la interfaz y la lógica interna, implementada antes de la integración del módulo avanzado de procesamiento de texto. Los cambios incluyen:

1. Reestructuración del Datos:
   - Se reorganizó la columna izquierda del formulario.
   - Implementación de una estructura de 3 filas para la ubicación: Fila exclusiva para Empresa, fila compartida para Ciudad/Dirección y fila compartida para Departamento/Barrio.

2. Módulo Geográfico Offline:
   - Se incorporó una base de datos interna masiva.
   - Lógica para interpretar direcciones complejas (Sur, Este, Circulares) y asignar el barrio automáticamente sin necesidad de internet. SOLO PARA MEDELLIN Y BOGOTA. 
   - Autocorrección de nombres de ciudades mediante atajos.
   - Eliminacion de espacios en blanco en automatico y espacios intermedios en el correo. 

3. Nuevos Campos y Controles:
   - Inclusión del campo "Infraestructura" en el bloque principal.
   - Agregado del botón "IdCorp" para copiar la combinación NIT-Celular para el registro de contactos. 
   - Agregado del botón "Datos Llamada" con estilo visual destacado para generar resúmenes rápidos. Cuando lo requiere la operacion. 

4. Lógica de Negocio:
   - Actualización de las plantillas de diagnóstico, reprueba y correos con las nuevas nemotecnias de seguimiento. AQUI SE INCLUYEN PARA LAS DEMAS AREAS DE N1, N2, Y LC. 

## Nota Técnica
El código JavaScript contenido en esta distribución no es editable directamente. Para realizar modificaciones o escalar funcionalidades (como futuras mejoras en el módulo de pegado rápido), se requiere acceso al código fuente original. Propiedad de cdiezlop. 
