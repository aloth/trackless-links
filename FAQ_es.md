🇺🇸 [English](FAQ.md) | 🇩🇪 [Deutsch](FAQ_de.md) | 🇪🇸 **Español** | 🇫🇷 [Français](FAQ_fr.md) | 🇯🇵 [日本語](FAQ_ja.md) | 🇨🇳 [中文](FAQ_zh-Hans.md)

# FAQ de Trackless Links

**Preguntas frecuentes y guía de usuario**

¡Bienvenido! Esta guía te ayudará a sacar el máximo partido a Trackless Links y resuelve las dudas más habituales.

---

## Contexto: por qué importa tener URLs limpias

Cuando Tim Berners-Lee inventó la World Wide Web en 1989, las URLs se diseñaron como direcciones simples: una forma de localizar un documento en un servidor. Una URL como `tienda.com/zapatos` te decía exactamente a dónde ibas.

Hoy, las URLs se han convertido en herramientas de vigilancia.

### La economía oculta de tus clics

Cada vez que haces clic en un enlace de un correo, tocas una publicación en redes sociales o sigues un resultado de búsqueda, se añade código adicional a la URL. Esos parámetros de seguimiento convierten una dirección simple en un informe detallado sobre ti:

```
shop.com/shoes?utm_source=newsletter&utm_campaign=spring_sale&utm_medium=email&fbclid=IwAR3x...&mc_eid=abc123
```

Esta única URL le revela a varias empresas:
- Que llegaste desde una newsletter (no directamente desde la web)
- Que respondiste a la campaña "spring sale"
- Que Facebook sabe que has hecho clic en ese enlace concreto
- Que la plataforma de email marketing ha registrado tu ID de suscriptor

Nada de esto cambia la página que ves. Solo cambia lo que las empresas aprenden sobre ti.

### Cómo funcionan los parámetros de seguimiento

El signo de interrogación (?) en una URL separa la dirección de la página de sus parámetros. Todo lo que va después del interrogante son metadatos, y las empresas los han estandarizado para crear un sistema de vigilancia:

| Parámetro | Quién lo usa | Qué revela |
|-----------|--------------|------------|
| `utm_source` | Marketers en general | Qué web o plataforma te envió |
| `utm_campaign` | Marketers en general | Qué anuncio o correo concreto has clicado |
| `fbclid` | Facebook/Meta | Tu ID de usuario de Facebook y tu comportamiento de clic |
| `gclid` | Google | Tu perfil publicitario de Google |
| `mc_eid` | Mailchimp | Tu identidad como suscriptor de correo |
| `ttclid` | TikTok | Tu perfil publicitario de TikTok |
| `msclkid` | Microsoft/Bing | Tu perfil publicitario de Microsoft |

Cuando compartes un enlace con tus amigos, a menudo compartes también esos parámetros, dejando que las empresas no solo te rastreen a ti, sino a todos los que hagan clic en el enlace que has reenviado.

### El coste para tu privacidad

Este seguimiento ocurre de forma invisible, pero las consecuencias son reales:

**Perfilado entre sitios**: Empresas como Facebook y Google ven tu actividad en millones de sitios y construyen perfiles detallados sobre tus intereses, compras y hábitos.

**Discriminación de precios**: Algunos comercios usan datos de seguimiento para mostrar precios distintos según la disposición a pagar que perciben en cada usuario.

**Burbujas de filtros**: Las plataformas publicitarias deciden qué contenido te muestran basándose en tu historial de clics, lo que puede limitar tu exposición a puntos de vista diversos.

**Brechas de datos**: Cualquier empresa que almacene tus datos de seguimiento es un posible objetivo. Cuantos menos datos se recolectan, menos pueden ser robados.

### Lo que hace Trackless Links

Trackless Links intercepta las URLs antes de que se carguen y elimina los parámetros de seguimiento. La URL limpia te lleva a la misma página, pero sin emitir tu huella digital.

Antes: `amazon.com/dp/1119737281?tag=influencer-20&ref=pd_sl_abc&utm_source=instagram`

Después: `amazon.com/dp/1119737281`

Esto sucede automáticamente para cada enlace en Safari, devolviendo a las URLs lo que siempre debieron ser: direcciones simples, nada más.

---

## Primeros pasos

### ¿Cómo activo la extensión de Safari?

Después de instalar la app:

1. Abre **Safari** en tu dispositivo
2. Toca el icono **AA** (o el botón **Extensiones** en Mac) en la barra de direcciones
3. Toca **Gestionar extensiones**
4. Encuentra **Trackless Links** y actívala
5. Concede los permisos necesarios

La extensión ya está activa y empezará a limpiar URLs automáticamente.

### ¿Por qué no funciona la extensión?

Asegúrate de que:
- Has activado la extensión en los ajustes de Safari (ver arriba)
- Has concedido los permisos necesarios cuando se te pidieron
- La extensión necesita permiso para acceder al contenido de las páginas web

En Mac, también puede que tengas que ir a **Ajustes del Sistema > Privacidad y seguridad > Extensiones** y activar Trackless Links.

### ¿Tengo que configurar algo para empezar a usarla?

No. Trackless Links funciona de inmediato con valores predeterminados sensatos:
- Los parámetros de seguimiento se eliminan automáticamente
- Más de 20 redirecciones predefinidas están listas para usar (puedes activar las que quieras)
- Todos los tweaks son opcionales, así que activa solo lo que necesites

---

## Privacidad y filtros de seguimiento

### ¿Qué parámetros de seguimiento elimina?

Trackless Links elimina códigos de seguimiento habituales como:
- `utm_source`, `utm_medium`, `utm_campaign` (atribución de marketing)
- `fbclid` (identificador de clic de Facebook)
- `gclid` (identificador de clic de Google)
- `msclkid` (identificador de clic de Microsoft/Bing)
- Y muchos más

Puedes ver la lista completa en la pestaña **Filtros** y añadir tus propios parámetros.

### ¿Cómo añado un parámetro de seguimiento personalizado?

1. Abre la app de Trackless Links
2. Ve a la pestaña **Filtros**
3. Toca el botón **+**
4. Introduce el nombre del parámetro (por ejemplo, `mi_tracker`)
5. Toca **Guardar**

La próxima vez que visites una URL con ese parámetro, se eliminará automáticamente.

### ¿Puedo desactivar temporalmente la eliminación de seguimiento?

Sí. En la pestaña **Filtros** puedes activar o desactivar filtros individuales. También puedes desactivar toda la limpieza desactivando todos los filtros.

---

## Redirecciones

### ¿Qué son las redirecciones y por qué usarlas?

Muchas webs populares recolectan grandes cantidades de datos sobre sus usuarios. Las redirecciones te permiten enrutarte automáticamente hacia alternativas que respetan tu privacidad y ofrecen el mismo contenido sin la vigilancia.

**Frontends respetuosos con la privacidad**: Proyectos como Nitter (para Twitter/X), Invidious (para YouTube) y Libreddit (para Reddit) muestran contenidos de las grandes plataformas sin iniciarte sesión ni rastrearte. Tú obtienes el contenido, ellos no obtienen tus datos.

**Preferencias de interfaz**: old.reddit.com ofrece la interfaz clásica que muchos prefieren. Algunas webs de noticias tienen versiones móviles más limpias. Las redirecciones te llevan siempre a tu versión preferida.

**Enrutamiento regional**: Redirige automáticamente dominios internacionales a tu versión local, o al revés.

### ¿Cómo activo una redirección predefinida?

1. Abre la app y ve a **Redirecciones**
2. Explora la lista de reglas predefinidas
3. Activa el interruptor junto a la regla que quieras
4. La redirección se aplica al instante, sin reiniciar nada

### ¿Cómo creo una redirección personalizada?

1. Ve a la pestaña **Redirecciones**
2. Toca el botón **+**
3. Introduce:
   - **Patrón**: La URL DESDE la que quieres redirigir (por ejemplo, `reddit.com`)
   - **Reemplazo**: A dónde redirigir (por ejemplo, `old.reddit.com`)
   - **Título** (opcional): Un nombre amistoso para la regla
4. Toca **Guardar**

Puedes usar coincidencias exactas o expresiones regulares (regex) para patrones avanzados.

### ¿Puedo usar grupos de captura regex y variables?

Sí. Envuelve entre paréntesis `()` la parte del patrón que quieras conservar y referénciala en el reemplazo con `$1`, `$2`, etc.

**Ejemplo: abrir enlaces de trabajo en Microsoft Edge**

- Patrón: `(https?://.*midominioacorporativo.*)`
- Reemplazo: `microsoft-edge:$1`

Esto captura toda la URL coincidente en el grupo 1 y la pega después de `microsoft-edge:`, abriendo el enlace en Edge en lugar de Safari.

**Ejemplo: forzar el dominio Amazon España**

- Patrón: `https://www\.amazon\.com/(.*)`
- Reemplazo: `https://www.amazon.es/$1`

Puedes usar varios grupos de captura en la misma regla (`$1`, `$2`, ...). Así Trackless Links funciona como Velja para enrutar enlaces a navegadores o apps por dominio.

### ¿Puedo reordenar mis reglas de redirección?

Sí. El orden importa porque gana la primera regla coincidente. Para reordenarlas:

1. Ve a **Redirecciones**
2. Mantén pulsada una regla y arrástrala
3. La prioridad se guarda automáticamente

### Mi redirección no funciona. ¿Qué pasa?

Comprueba estos puntos habituales:

- ¿Está la regla **activada**? (interruptor en on)
- ¿Es correcto el patrón? (prueba primero con una coincidencia exacta sencilla)
- ¿Hay otra regla que coincide antes? (revisa el orden)
- ¿Estás probando en Safari? (la extensión solo funciona en Safari, no en otros navegadores)

---

## Tweaks

### ¿Qué son los tweaks?

Las webs modernas suelen restringir lo que puedes hacer en tu propio navegador. Desactivan la selección de texto para que no copies, autoplay para inflar métricas y muestran popups intrusivos para que no te vayas.

Los tweaks te devuelven el control. Trackless Links incluye más de 20 modificaciones de navegador organizadas en seis categorías.

Todos los tweaks son opcionales, así que tú decides cuáles activar.

### Lista completa de tweaks

#### Lectura e interacción

| Tweak | Qué hace |
|-------|----------|
| **Permitir selección y copia de texto** | Reactiva selección, copia, pegado y menús contextuales en sitios que intentan bloquearlos. Imprescindible para investigar y tomar notas. |
| **Desactivar diálogos de salida** | Evita los molestos avisos "¿Seguro que quieres salir?" al navegar a otra página o cerrar una pestaña. |
| **Desactivar nuevas pestañas forzadas** | Impide que los sitios fuercen los enlaces a abrirse en pestañas nuevas (target="_blank"). Los enlaces se abren por defecto en la misma pestaña. |
| **Ignorar fragmentos de texto** | Elimina los fragmentos #:~:text= estilo Chrome de las URLs para que las páginas no salten automáticamente al texto resaltado. |
| **Permitir arrastrar y soltar** | Restaura el comportamiento por defecto de arrastrar texto y archivos en sitios que lo bloquean. |

#### Gestión de banners de cookies (Experimental)

Trackless Links ofrece una gestión inteligente del consentimiento de cookies con tres modos:

| Modo | Comportamiento |
|------|---------------|
| **Off** | Sin intervención sobre los banners de cookies |
| **Solo ocultar** | Oculta visualmente los banners sin pulsar nada |
| **Rechazar automáticamente** | Pulsa automáticamente botones de "rechazar" o "solo esenciales" y oculta los banners restantes |

La función de rechazo automático admite varios idiomas y funciona con Google, los frameworks de consentimiento más comunes y muchas webs populares.

#### Controles de medios

| Tweak | Qué hace |
|-------|----------|
| **Mostrar siempre los controles de play/pause** | Fuerza los controles nativos del navegador en reproductores de audio y vídeo, aunque los sitios los oculten. |
| **Bloquear autoplay** | Evita que vídeos y audios se reproduzcan automáticamente al cargar la página. |
| **Aplicar velocidad por defecto** | Ajusta todos los medios a tu velocidad de reproducción preferida (de 0,5x a 3,0x). |
| **Bloquear velocidad de reproducción** | Impide que los sitios reseteen la velocidad que has elegido. |
| **Pausar todo al cargar la página** | Pausa cada elemento de audio y vídeo cuando se carga una página. |
| **Activar Picture-in-Picture** | Restaura la funcionalidad PiP en sitios que intentan desactivarla. En YouTube, desliza al inicio o bloquea el dispositivo para iniciar PiP automáticamente, o mantén pulsado el vídeo durante medio segundo. |

#### Privacidad y limpieza

| Tweak | Qué hace |
|-------|----------|
| **Limpiar URLs al copiar** | Elimina automáticamente los parámetros de seguimiento de cualquier enlace que copies al portapapeles. |
| **Saltar redirectores comunes** | Desempaqueta URLs acortadas (como t.co o bit.ly) y va directo al destino. |
| **Abrir en Safari** *(novedad en 4.1)* | Fuerza que los enlaces de los dominios configurados se abran en Safari en lugar de saltar a la app instalada. Incluye una lista por dominio con Instagram, X (Twitter), YouTube, TikTok, Reddit, LinkedIn, Pinterest y Spotify. Todas las entradas están desactivadas por defecto. También puedes añadir dominios personalizados. |

#### Tweaks adicionales

| Tweak | Qué hace |
|-------|----------|
| **Desactivar límites de zoom** | Quita las restricciones de zoom en sitios poco amigables con el móvil. |
| **Forzar modo oscuro** | Aplica una inversión inteligente de colores para crear temas oscuros en cualquier web. Conserva imágenes y vídeos mientras transforma textos y fondos. |
| **Desactivar animaciones** | Reduce o elimina las animaciones y transiciones CSS. Útil para accesibilidad y concentración. |

#### Avanzado (puede romper algunos sitios)

| Tweak | Qué hace |
|-------|----------|
| **Forzar barras de desplazamiento visibles** | Hace que las barras de scroll estén siempre visibles en lugar de ocultarse. Puede entrar en conflicto con algunos diseños. |
| **Bloquear window.close()** | Impide que las webs cierren tu pestaña o ventana mediante JavaScript. |

### ¿Cómo activo los tweaks?

1. Ve a la pestaña **Tweaks**
2. Explora las opciones disponibles
3. Activa o desactiva cada tweak
4. Los cambios se aplican al instante

### ¿Por qué un tweak no funciona en una web concreta?

Algunas webs combaten activamente las modificaciones. Si un tweak no funciona:

- Puede que el sitio use técnicas anti-modificación agresivas
- Prueba a desactivar otras extensiones para descartar conflictos
- Reporta el problema en GitHub. Mejoramos la compatibilidad continuamente.

### ¿Cuál es la diferencia entre "Forzar controles de medios" y "Bloquear autoplay"?

- **Forzar controles de medios**: Muestra los controles estándar de vídeo/audio del navegador aunque la web los oculte
- **Bloquear autoplay**: Impide que vídeos y audios se reproduzcan automáticamente al cargar una página

Puedes usarlos juntos para máximo control.

---

## Credibilidad de la fuente

### ¿Qué es la credibilidad de la fuente?

La credibilidad de la fuente es un sistema opcional de avisos que te ayuda a identificar webs conocidas por desinformación, fake news o teorías conspirativas antes de perder el tiempo en ellas.

Trackless Links usa **CRED-1**, un conjunto de datos abierto y revisado por pares con dominios señalados. Cuando está activo, Safari puede mostrar un banner de aviso antes o durante tu visita a esos sitios.

### ¿La credibilidad de la fuente está activa por defecto?

No. La credibilidad de la fuente está **desactivada por defecto**.

Puedes activarla cuando quieras en la pestaña **Credibilidad**. La función opcional **Auto-actualización de CRED-1** también está desactivada por defecto y debe habilitarse por separado.

### ¿Cómo funcionan las auto-actualizaciones de CRED-1?

Si activas las auto-actualizaciones de CRED-1, Trackless Links comprobará periódicamente si hay una nueva versión publicada de CRED-1 y actualizará el conjunto de datos en tu dispositivo.

Detalles importantes:
- Las auto-actualizaciones son **opt-in**
- La app sigue incluyendo un conjunto CRED-1 empaquetado para que la credibilidad de la fuente funcione sin descarga inicial
- Las comprobaciones y consultas se mantienen **en el dispositivo** durante la navegación normal; Trackless Links no envía tu historial a ningún sitio
- Puedes desactivar las auto-actualizaciones cuando quieras desde la pestaña **Credibilidad**

## Búsqueda en archivos

### ¿Qué es la búsqueda en archivos?

La web no es permanente. Hay páginas que se borran, artículos que se modifican y webs enteras que desaparecen. La Wayback Machine del Internet Archive y servicios similares conservan instantáneas de la web, creando un registro histórico de lo que existía en cada momento.

La búsqueda en archivos te da acceso instantáneo a esas versiones conservadas:

- Encuentra contenido borrado o ve cómo era una página antes de cambiar
- Accede a páginas cuando un sitio está caído temporalmente
- Investiga cómo han evolucionado las webs y sus afirmaciones a lo largo del tiempo
- Verifica citas y referencias que podrían haber sido alteradas

### ¿Cómo busco en un archivo?

**Desde Safari:**
1. Toca el icono **AA** o el botón **Extensiones**
2. Selecciona **Trackless Links**
3. Toca el servicio de archivo que quieras (por ejemplo, Wayback Machine)
4. La página actual se buscará en ese archivo

**Desde cualquier app (Hoja para compartir):**
1. Comparte un enlace desde cualquier app
2. Elige **Buscar en archivo**
3. Selecciona tu servicio de archivo preferido

### ¿Puedo añadir más servicios de archivo?

Sí. Puedes añadir servicios personalizados:

1. Ve a **Tweaks**, luego **Búsqueda en archivos** y luego **Configurar servicios**
2. Toca **+** para añadir un servicio
3. Introduce el patrón URL del servicio
4. El servicio ya está disponible en el popup

### ¿Debería activar "Quitar parámetros de consulta"?

Recomendado: Sí. Esta opción elimina los códigos de seguimiento y otros parámetros antes de buscar en los archivos, lo que suele dar mejores coincidencias. Desactívala solo si necesitas buscar una URL con parámetros específicos intactos.

---

## Integración con la hoja para compartir

### ¿Cómo uso la hoja para compartir para limpiar enlaces?

Cuando compartes enlaces desde otras apps, los parámetros de seguimiento van con ellos. La extensión para la hoja para compartir te permite limpiar los enlaces antes de compartirlos:

1. En cualquier app (Safari, Reddit, X, etc.), toca el botón **Compartir**
2. Desplázate y encuentra **Limpiar con Trackless Links**
3. La URL limpia se copia al portapapeles

Ahora puedes compartir un enlace limpio que no revela dónde lo has encontrado ni rastrea a quien haga clic.

### ¿Puedo compartir a archivos desde otras apps?

Sí. Usa la misma hoja para compartir:

1. Toca **Compartir** en cualquier enlace
2. Elige **Buscar en archivo**
3. Selecciona tu servicio de archivo
4. Safari se abrirá con los resultados de la búsqueda en el archivo

---

## Sincronización con iCloud

### ¿Cómo funciona la sincronización con iCloud?

Tus ajustes de privacidad viajan contigo. Al activar la sincronización con iCloud, tu configuración se sincroniza automáticamente entre iPhone, iPad y Mac mediante tu cuenta personal de iCloud:

- **Filtros** (parámetros de seguimiento)
- **Redirecciones** (reglas personalizadas y estado)
- **Tweaks** (todos los ajustes)
- **Servicios de archivo** (los que has configurado)

Las estadísticas de privacidad (como el número de rastreadores bloqueados) se mantienen específicas de cada dispositivo y no se sincronizan.

### ¿Tengo que activar la sincronización con iCloud?

Es opcional. La sincronización con iCloud está desactivada por defecto. Para activarla:

1. Ve a **Ajustes** en la app
2. Busca **Sincronización con iCloud**
3. Actívala

Tus ajustes se sincronizarán entre todos los dispositivos conectados a la misma cuenta de iCloud.

### Mis cambios no se sincronizan entre dispositivos. ¿Qué pasa?

Comprueba lo siguiente:

- ¿Está la sincronización con iCloud **activada** en ambos dispositivos?
- ¿Están ambos dispositivos conectados a la **misma cuenta de iCloud**?
- ¿Está iCloud Drive activado en **Ajustes del Sistema** (Mac) o **Ajustes** (iOS)?
- ¿Tienen ambos dispositivos conexión a internet?
- Prueba a forzar el cierre y reabrir la app

Si la sincronización sigue sin funcionar, prueba a desactivarla y volverla a activar.

### ¿Puedo usar Trackless Links sin iCloud?

Sí. La sincronización con iCloud es totalmente opcional. La app funciona perfectamente guardando todos los ajustes de forma local en cada dispositivo.

---

## Trucos y consejos

### ¿Cómo veo qué parámetros de seguimiento se han eliminado?

Consulta las **Estadísticas** del panel principal. Allí verás:
- Total de URLs limpiadas
- Redirecciones aplicadas

### ¿Puedo exportar mis ajustes?

Los ajustes se guardan en iCloud (si está activado) o localmente en tu dispositivo. Todos los datos están bajo tu control y nunca se envían a servidores de terceros.

### ¿Trackless Links ralentiza la navegación?

No. La extensión es extremadamente ligera y procesa las URLs en milisegundos antes de que las páginas terminen de cargar. No notarás impacto en el rendimiento.

### ¿Puedo usar Trackless Links con otras extensiones de Safari?

Sí. Trackless Links está pensada para coexistir con otras extensiones. Si notas conflictos, prueba a ajustar el orden de ejecución en los ajustes de extensiones de Safari.

### ¿Cuál es la diferencia entre Trackless Links y Trackless Links Pro?

| Función | Trackless Links | Trackless Links Pro |
|---------|----------------|---------------------|
| iPhone y iPad | Sí | Sí |
| App para Mac | No | Sí |
| Sincronización iCloud | Sí | Sí |
| Precio | Compra única (solo iOS) | Compra universal (todas las plataformas) |

Trackless Links Pro es una compra universal. Cómprala una vez y úsala en iPhone, iPad y Mac.

---

## Solución de problemas

### No encuentro la extensión en Safari

Asegúrate de que:
- Has instalado la app desde el App Store
- Has abierto la app al menos una vez
- Las extensiones de Safari están activadas en los ajustes del sistema

### Los enlaces no se limpian

Comprueba:
- ¿Está la extensión **activada** en Safari?
- ¿Concediste los permisos necesarios?
- ¿Hay filtros **activos** en la pestaña Filtros?

### Mi redirección personalizada no funciona

- Revisa la sintaxis del patrón (prueba primero con una coincidencia exacta)
- Asegúrate de que la regla está **activa**
- Comprueba que ninguna otra regla coincide antes (el orden importa)
