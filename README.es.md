# Aviso legal y política de privacidad – CFOP Trainer

[Deutsch (versión vinculante)](README.md) · [English](README.en.md) · [Français](README.fr.md) · [Italiano](README.it.md) · **Español**

*Traducción de cortesía. En caso de discrepancia, solo es vinculante la versión alemana.*

## Aviso legal (Impressum)

Información conforme al § 5 DDG (ley alemana de servicios digitales, antes § 5 TMG):

Roland Albrecht
Im Jägeracker 42
79312 Emmendingen
Alemania

Contacto: rca@quantentunnel.de

## Política de privacidad

Fecha: 18/10/2026

### 1. Responsable del tratamiento

Roland Albrecht
Correo electrónico: rca@quantentunnel.de

La persona indicada arriba, como desarrollador de la app "CFOP/Fridrich-Algorithmen-Trainer" (en adelante, "la app"), es responsable en el sentido del Reglamento General de Protección de Datos (RGPD) de los tratamientos descritos a continuación.

### 2. Resumen

La app no recoge, almacena ni transmite **ningún dato personal al desarrollador ni a terceros**. No hay:

- cuenta de usuario ni inicio de sesión,
- conexión a internet (la app no solicita el permiso correspondiente y no se comunica con ningún servidor),
- servicios de análisis, seguimiento o publicidad (ni Google Analytics, ni SDK de informes de errores o de anuncios),
- transmisión de datos a terceros, ya que ningún dato sale del dispositivo.

Todos los datos que se generan en la app permanecen exclusivamente en local en el dispositivo de la persona usuaria. Lo mismo vale para la conexión Bluetooth opcional a un smart cube: se establece solo directamente entre el dispositivo y el cubo, sin acceso a la ubicación (apartado 5).

### 3. ¿Qué datos se guardan en local en el dispositivo?

Para cumplir sus funciones de entrenamiento (entrenamiento de algoritmos, curso guiado, repaso con repetición espaciada), la app guarda los siguientes datos **exclusivamente en local, en una base de datos en el propio dispositivo**:

- estadísticas de entrenamiento y práctica por caso de algoritmo (p. ej., número de intentos, porcentaje de aciertos),
- datos de planificación y vencimiento de los repasos con repetición espaciada (fecha del próximo repaso de cada caso),
- progreso en el curso guiado (niveles y casos ya desbloqueados o consolidados),
- variantes de secuencias de movimientos guardadas por la persona usuaria para casos concretos,
- idioma elegido para la app (alemán, inglés, francés, italiano o español) y demás ajustes de la app (p. ej., valor predeterminado de la vista de pegatinas, visualización de la racha diaria).
- si se usa un smart cube (apartado 5): nombre y dirección Bluetooth del último cubo conectado con los ajustes correspondientes (conectar automáticamente, usar la orientación del cubo) y, para cada intento, si se hizo con la pantalla táctil o con el smart cube.

Estos datos se almacenan en el dispositivo mediante una base de datos Room local (SQLite) y el almacenamiento local de ajustes (SharedPreferences). No se trata de una transmisión al desarrollador: nadie salvo la persona que usa el dispositivo tiene acceso a estos datos.

### 4. Función de copia de seguridad (archivo de copia local)

En los ajustes, la app ofrece de forma opcional crear un archivo de copia de seguridad local con las estadísticas de aciertos, el historial de intentos con la planificación y los vencimientos de los repasos, el progreso en el curso, las variantes de algoritmo favoritas y los algoritmos guardados por la persona usuaria, así como volver a cargar un archivo de copia creado antes. El archivo se guarda o se lee exclusivamente mediante el diálogo de selección de archivos del sistema operativo, en la ubicación que elija la persona usuaria: la app no elige ninguna ubicación automáticamente y nunca transmite el archivo al desarrollador ni a terceros. Si la persona usuaria elige como ubicación una carpeta sincronizada con un servicio en la nube (p. ej., una integración de Drive u OneDrive del dispositivo), el tratamiento posterior de ese archivo se rige por la política de privacidad del proveedor de nube correspondiente, no por la de esta app.

### 5. Conexión Bluetooth a un smart cube (opcional)

A partir de Android 12 la app puede conectarse de forma opcional a un cubo de Rubik con Bluetooth ("smart cube", actualmente GAN i4 y GoCube) que comunica a la app los giros realizados en el cubo. La función es voluntaria; sin ella la app sigue siendo totalmente utilizable de forma táctil.

- **Conexión solo local:** la app busca smart cubes cercanos mediante Bluetooth Low Energy y se conecta directamente al cubo elegido. No intervienen servidores, cuentas del fabricante ni conexión a internet.
- **Datos tratados:** la app recibe del cubo exclusivamente eventos de giro (qué cara se giró y en qué sentido, con marca de tiempo), eventos de orientación (posición del cubo en el espacio), el nivel de batería y el nombre del dispositivo, el modelo e información de hardware. Estos datos solo se usan para el ejercicio en curso; de ellos solo se guardan los datos de entrenamiento habituales del apartado 3 (secuencia de movimientos, tiempo y valoración de un intento, más la fuente de entrada).
- **Cubo guardado:** para poder volver a conectarse al mismo cubo en el siguiente inicio, la app guarda en local en el dispositivo su nombre y su dirección Bluetooth. Esta entrada puede borrarse en cualquier momento con "Quitar" en el menú smart cube. Estos datos no forman parte del archivo de copia de seguridad (apartado 4).
- **Sin acceso a la ubicación:** la app solo usa el permiso "Dispositivos cercanos" (apartado 8) y declara expresamente al sistema que no deduce ninguna ubicación de la búsqueda Bluetooth. Los demás dispositivos Bluetooth encontrados no se muestran ni se guardan.
- **Sin transmisión:** ni los datos del cubo ni la dirección Bluetooth guardada salen del dispositivo.

### 6. Sin transmisión de datos, sin servidor, sin cuenta

La app no necesita ni tiene permiso de acceso a internet. Por tanto, a través de la app nunca se transmiten datos al desarrollador, a Google ni a otros terceros. No hay cuenta de usuario, registro ni sincronización en la nube.

### 7. Sin servicios de análisis, seguimiento o publicidad

La app no contiene software de análisis (p. ej., Firebase Analytics), servicios de informes de errores (p. ej., Crashlytics) ni SDK de publicidad. No se crean perfiles de uso, no se determina la ubicación y no se lee el ID de publicidad.

### 8. Permisos de la app

La app no solicita permisos especiales de acceso al dispositivo (p. ej., ni cámara, ni ubicación, ni contactos, ni micrófono, ni internet), con una excepción: para la conexión opcional a un smart cube (apartado 5) usa a partir de Android 12 el permiso "Dispositivos cercanos" (`BLUETOOTH_SCAN` con la indicación de que no se deduce ninguna ubicación, y `BLUETOOTH_CONNECT`). Solo se solicita cuando la persona usuaria busca o conecta un cubo en el menú smart cube y puede revocarse en cualquier momento en los ajustes de Android; el resto de la app funciona también sin él. La función de copia de seguridad (apartado 4) utiliza el diálogo de selección de archivos del sistema (Storage Access Framework), que no requiere permisos adicionales.

### 9. Plazo de conservación y supresión

Los datos indicados en el apartado 3 permanecen guardados en local en el dispositivo hasta que:

- se restablecen mediante las funciones integradas en la app (p. ej., "Restablecer" en las estadísticas o "Borrar mis algoritmos" en los ajustes), o
- se eliminan por completo del dispositivo al desinstalar la app.

El smart cube guardado (apartado 5) puede borrarse además en cualquier momento con "Quitar" en el menú smart cube.

Como no se guarda ningún dato fuera del dispositivo, tras desinstalar la app no queda ninguna otra copia de los datos, salvo un archivo de copia de seguridad creado por la persona usuaria (apartado 4), que permanece en la ubicación elegida con independencia de la app y que puede borrar ella misma si lo desea.

### 10. Derechos de la persona interesada

Como la app no transmite datos personales al desarrollador, todos los datos indicados en el apartado 3 están exclusivamente bajo el acceso directo y el control total de la persona usuaria (el acceso, la rectificación y la supresión se realizan directamente a través de la app o desinstalándola). Aun así, para cualquier pregunta sobre protección de datos relacionada con la app puede utilizarse en todo momento el contacto indicado en el apartado 1.

### 11. Menores

La app no está dirigida específicamente a niños y no recoge ningún dato personal, independientemente de la edad de la persona usuaria.

### 12. Cambios en esta política de privacidad

Esta política de privacidad puede adaptarse cuando sea necesario, por ejemplo si nuevas funciones de la app lo requieren. La versión vigente está disponible en la dirección enlazada en la ficha de Play Store.

### 13. Contacto

Para cualquier pregunta sobre esta política de privacidad o sobre la app, escribe a:

rca@quantentunnel.de
