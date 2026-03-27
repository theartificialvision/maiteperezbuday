# Proyecto: Web inmersiva para locutora

**Perfil:** Locutora rioplatense/uruguaya radicada en Barcelona.  
**Enfoque:** Web simple, oscura y contemporánea, centrada en la escucha.  
**Dirección visual:** Dark mode, diseño espacial, capas translúcidas, lenguaje digital sobrio.  
**Requisito clave:** Integrar una visualización de audio reactiva que responda en tiempo real a la reproducción.

---

## 1. Criterio general

La web debe ser más bien contenida, no recargada.  
No busco una estética futurista exagerada ni una demo de efectos.  
La experiencia tiene que transmitir:

- presencia
- técnica
- sensibilidad sonora
- una interfaz actual, limpia y con personalidad

La voz es el centro. Todo lo demás acompaña.

---

## 2. Estructura base

La web tendrá una estructura sencilla, con foco en dos demos principales:

- **Demo Publicidad**
- **Demo Audiolibro**

Ambas deben convivir dentro del mismo universo visual, pero la parte de audiolibro puede tener una capa extra de textura, más narrativa, más envolvente, sin dejar de combinar con el resto del sitio.

Además, la web debe permitir crecer fácilmente para sumar nuevas ideas o secciones más adelante sin romper la lógica general.

---

## 3. Stack sugerido

- **Framework:** React
- **Estilos:** Tailwind CSS
- **Animación:** Framer Motion
- **Audio reactivo:** Web Audio API
- **Visualización de waveform:** Wavesurfer.js o implementación custom con `AnalyserNode` + SVG / Canvas

Si se busca más control visual y menos apariencia de librería, conviene una solución custom.

---

## 4. Componente central: visualizador de voz

Este es el núcleo visual de la home.  
No debe sentirse como una barra de reproducción estándar, sino como una presencia gráfica integrada en la interfaz.

### Estado en pausa
- Línea fina, horizontal y estable.
- Aparición limpia, sutil, con un leve resplandor.
- Debe insinuar que hay sonido, aunque todavía no esté activo.

### Estado en reproducción
- La línea se transforma en una onda orgánica viva.
- La animación responde al audio real en tiempo real.
- Las frecuencias bajas ensanchan y profundizan la forma.
- Las frecuencias altas generan tensión, detalle y pequeños picos.

### Reacción del entorno
Cuando el audio entra en reproducción:

- el fondo puede variar levemente en brillo o temperatura
- algunas sombras o halos pueden respirar con el volumen
- ciertos bordes o capas de interfaz pueden reaccionar de forma casi imperceptible

La clave es que se note, pero no moleste.

---

## 5. Arquitectura de secciones

### A. Header
- Estructura flotante o muy liviana
- Logo o naming simple
- Navegación mínima
- CTA principal orientado a escuchar

Ejemplo de CTA:
- Escuchar demo
- Reproducir muestra
- Escuchar voz

No hace falta un menú pesado.

---

### B. Home / Hero
- Titular claro, breve y elegante
- Subtítulo sin frases hechas ni eslóganes vacíos
- Reproductor principal integrado en la composición
- Selector visible para cambiar entre:
  - Publicidad
  - Audiolibro

La transición entre ambos demos debe ser fluida, sin cortar la sensación de continuidad.

---

### C. Demo Publicidad
Esta parte debe sentirse más precisa, limpia y directa.

- Interfaz más nítida
- Menos textura
- Más sensación de estudio, agencia, pieza comercial
- Ideal para mostrar registro, timing, intención y claridad

Puede incluir:
- una breve descripción del tipo de locución
- estilos o usos posibles
- botón para reproducir

---

### D. Demo Audiolibro
Esta sección sí puede diferenciarse un poco más.

Debe tener:
- algo más de textura visual
- una atmósfera más narrativa
- una profundidad más sensorial

Pero cuidado: no convertirla en “otra web”.  
Tiene que sentirse como una variación dentro del mismo sistema.

Recursos posibles:
- fondos con más grano o relieve digital
- portadas o piezas editoriales
- bloques visuales con más cuerpo
- transiciones más lentas o más envolventes

Acá la experiencia puede ser un poco más íntima.

---

### E. Sobre mí
Bloque breve y bien escrito.

Objetivo:
- presentar perfil
- ubicar procedencia y base actual
- transmitir tono, experiencia y criterio

No hace falta una biografía larga.  
Mejor pocas líneas con peso.

---

### F. Estudio / ficha técnica
Una sección compacta para mostrar solvencia técnica sin caer en exhibicionismo.

Puede incluir:
- micrófono
- interfaz
- software
- edición
- formatos de entrega
- tiempos de respuesta

Idealmente en un bloque modular claro, tipo grid.

---

### G. Contacto
Formulario simple y funcional.

Campos sugeridos:
- Nombre
- Email
- Tipo de proyecto
- Mensaje
- Presupuesto estimado

Tiene que verse integrado, no como una sección genérica al final.

---

## 6. Sistema visual

### Base
- fondo oscuro
- gradientes lentos
- capas translúcidas
- bordes suaves
- iluminación controlada

### Lenguaje
- más “interfaz editorial de audio” que “futurismo decorativo”
- más precisión que espectáculo
- más ritmo que efecto

### Audiolibro
La parte de audiolibro puede sumar:
- textura
- densidad
- una atmósfera un poco más táctil o narrativa

Pero siempre manteniendo:
- misma paleta base
- misma lógica tipográfica
- misma arquitectura de interacción

---

## 7. Animación

- entradas suaves en scroll
- hover muy contenidos
- cambios de estado claros entre pausa y play
- continuidad entre secciones
- nada de gestos exagerados, rebotes ni recursos de plantilla

La animación tiene que acompañar el audio, no competir con él.

---

## 8. Criterios funcionales

- SPA clara y rápida
- responsive real, especialmente en móvil
- audio estable
- carga liviana
- posibilidad de ampliar la web con nuevas categorías o demos
- reproductor bien integrado en toda la navegación

---

## 9. Dirección de implementación para IA

Actúa como un desarrollador frontend senior experto en React, Tailwind CSS, Framer Motion y Web Audio API.

Desarrolla una SPA para una locutora rioplatense radicada en Barcelona.  
La web debe ser oscura, limpia, contemporánea y centrada en la escucha.

La estructura inicial debe incluir:

- Header ligero
- Hero principal con visualizador de voz reactivo
- Dos demos principales:
  - Publicidad
  - Audiolibro
- Sección Sobre mí
- Sección técnica del estudio
- Formulario de contacto

El reproductor principal debe analizar el audio en tiempo real mediante Web Audio API y traducirlo a una visualización orgánica en SVG o Canvas.

La sección de audiolibro debe diferenciarse visualmente con más textura y atmósfera, pero sin romper la coherencia del sistema general.

Priorizar:
- claridad visual
- movimiento sutil
- buena jerarquía
- integración real entre audio e interfaz
- posibilidad de crecimiento futuro sin rehacer la arquitectura