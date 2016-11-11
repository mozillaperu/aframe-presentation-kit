<!-- .slide: data-background="media/img/aframe.jpg" -->

<div class="talk-title">
  <h1>A-Frame</h1>
  <p>Un framework web para construir experiencias VR</p>
  <p class="talk-info">
    @AngelFQC | Mozilla Perú | **aframe.io**
  </p>
</div>

<!-- NOTES -->
- Abordar en el 3D y el mundo VR a los desarrolladores con herramientas de fácil uso
- Experiencias de prototipado en WebVR de manera rápida

------

# Realidad Virtual

<!-- .slide: data-background-video="media/video/virtualreality.mp4" data-background-video-loop="true" data-state="state--bg-dark" -->

<!-- NOTES -->
- Preguntar cuántos han probado VR.
- La realidad virtual es una plataforma tecnológica que te transporta a entornos 3D realistas, interactivos e inmersivos
- Es la próxima plataforma, va a cambiar la forma de trabajar + jugar + comunicarse digitalmente, la cara de la sociedad

---

# ¡Diversión!

<!-- .slide: data-background="media/img/vrshooting.jpg" data-state="state--bg-dark" -->

<!-- NOTES -->
- Cuente historias interesantes sobre sus experiencias con VR.

---

<div class="image-row">
  <div><img data-src="media/img/google-cardboard.png"></div>
  <div><img data-src="media/img/google-daydream.png"></div>
  <div><img data-src="media/img/samsung-gearvr.png"></div>
</div>

<div class="image-row">
  <div><img data-src="media/img/oculus-rift.png"></div>
  <div><img data-src="media/img/playstation-vr.png"></div>
  <div><img data-src="media/img/htc-vive.png"></div>
</div>

<!-- NOTES -->
- Respaldado por las corporaciones más grandes del mundo, todo el mundo lo quiere
- Rango de barato a caro, atado y sin ataduras, controlladores, seguimiento
- HTC Vive con Steam ofrece actualmente las experiencias más atractivas, pero nunca se sabe
- Se ven un montón de diferentes dispositivos, sistemas, plataformas compitiendo entre sí ...

---

## Fricción de los Ecosistemas VR

<div class="captioned-image-row">
  <div>
    <img data-src="media/img/gatekeeper.png">
    <i>Control</i>
  </div>
  <div>
    <img data-src="media/img/downloads-installs.png">
    <i>Instalaciones</i>
  </div>
  <div>
    <img data-src="media/img/closed-door.png">
    <i>Entorno cerrado</i>
  </div>
</div>

<!-- NOTES -->
- Las tiendas de aplicaciones y las corporaciones controlan la distribución: pueden eliminar o bloquear contenido
- Las descargas / instalaciones son una barrera para el consumo: páginas de pequeñas empresas
- Un ecosistema cerrado: motores patentados, curvas de aprendizaje abruptas, experiencias de aisladas, fragmentación
- Queremos que VR tenga éxito, por lo que queremos una plataforma sin estos puntos de fricción. La respuesta es WebVR ...

------

# WebVR

Una plataforma abierta de realidad virtual con las ventajas de **la Web**

<div class="captioned-image-row">
  <div>
    <img data-src="media/img/web-is-open.png">
    <i>Abierta</i>
  </div>
  <div>
    <img data-src="media/img/web-is-connected.png">
    <i>Conectada</i>
  </div>
  <div>
    <img data-src="media/img/web-is-instant.png">
    <i>Al instante</i>
  </div>
</div>

<!-- NOTES -->
WebVR es... la realidad virtual en el navegador, potenciada por la Internet

Open:
- Cualquiera puede publicar
- Cultura de Código Abierto con estándares abiertos

Conectada:
- Atravesar mundos

Al instante:
- Hacer click en un enlace en Twitter o Weibo, experiencias VR de inmediato
- Sin instalaciones
- Imagina para grandes expriencias: compras y espacios personales
- Ideal para experiencias de mucho tiempo

Transición:
- La web tiene ventajas que la hacen la mejor plataforma para las personas
- Necesitamos actuar para hacerla realidad, no podemos esperar a que la VR se cocine y cristalice
- ¡Involúcrate!

---

<img class="stretch" data-src="media/img/webvr.png">

Las API del navegador son las que permiten renderizar WebGL a los auriculares y acceder a los sensores VR

https://w3c.github.io/webvr/

<!-- NOTES -->
API:
- Una ruta optimizada para los auriculares
- Acceso a los datos de posición y rotación

Historia:
- API initial de WebVR API por Mozilla
- Una trabajo con el grupo de la comunidad de W3C
- Mozilla, Google, Samsung, Microsoft, y la comunidad actualmente están iterando en la API WebVR 1.0

No es sólo una especificación, está implementada...

---

<div class="captioned-image-row">
  <div>
    <img data-src="media/img/firefox-nightly.png">
    <i>Firefox Nightly</i>
  </div>
  <div>
    <img data-src="media/img/chromium.png">
    <i>Chromium (Experimental)</i>
  </div>
  <div>
    <img data-src="media/img/samsung-browser.png">
    <i>Samsung Internet</i>
  </div>
  <div>
    <img data-src="media/img/google-cardboard.png">
    <i>Mobile Polyfill</i>
  </div>
</div>

<!-- NOTES -->
- Firefox + Chrome WebVR 1.0 alcanzarán los canales de lanzamiento estable a inicios del 2017
- Actualmente detrás de Nightly, versiones personalizadas...
- Mobile Polyfill: Utilizar sensores de orientación / movimiento de dispositivos para ser compatible a los smartphones
- Con todos los navegadores detrás...

---

## Metaverso

<!-- .slide: data-background="media/img/metaverse.png" -->

<!-- NOTES -->
- Espacios virtuales colectivos persistentes compartidos
- Alterna la realidad digital que el mundo puede vivir, trabajar, jugar
- Debe ser descentralizado / abierto / conectado, la web es la mejor plataforma para realizar completamente
- ¿Por dónde comenzamos?
- three.js abstrae WebGL, 3D, y WebVR, Pero todavía podemos hacerlo más accessible

---

Es un poco difícil crear experiencias WebVR...

---

<!-- .slide: data-background-video="media/video/boilerplate.mp4" data-state="state--bg-dark" -->

<div class="slide__boilerplate">
  <p>Importar WebVR polyfill</p>
  <p>Configurar camera</p>
  <p>Configurar luces</p>
  <p>Initializar escena</p>
  <p>Declarar y pasar al lienzo</p>
  <p>Controlar redimesión de ventana</p>
  <p>Instalar VREffect</p>
  <p>Instanciar renderizado</p>
  <p>Crear bucle de renderizado</p>
  <p>Precargar recursos</p>
  <p>Determinar la capacidad de respuesta</p>
  <p>Tratar con metatags y móviles</p>
</div>

<!-- NOTES -->
- Todavía es demasiado difícil crear experiencias de WebVR
- Enorme obstáculo si se hacen pequeños prototipos y experimentos
- Boilerplate necesita actualizarse con las nuevas versiones de WebVR, three.js, y peculiaridades del navegador
- Encapsular todo esto dentro de una sola línea...

------

# A-Frame

<!-- .slide: data-background="media/img/aframe-rendered-full.png" -->

Un framework declarativo para construir experiencias de realidad virtual en la Web

<!-- NOTES -->
- Lanzado en diciembre pasado
- ¿Por qué?:
  - Fácil para los desarrolladores web crear contenido VR, sin conocimientos gráficos
  - Prototipar y experimentar WebVR y VR UX más rápido
  - Vehículo para arrancar el ecosistema WebVR

---

## Hola Mundo

<!-- .slide: data-background="media/img/aframe.png" data-transition="slide-in none" -->

```html
<html>
  <script src="https://aframe.io/releases/0.3.2/aframe.min.js"></script>
  <a-scene>





  </a-scene>
</html>
```
<!-- .element: class="stretch" -->

<!-- NOTES -->
- Sólo HTML
- Poner una etiqueta de script, sin pasos de construcción
- Usando Custom HTML Elements
- Una línea de HTML `<a-scene>` maneja
  - lienzo, cámara, renderiador, luces, controles, bucle de renderizado, WebVR polyfill, VREffect
- Poner las cosas de nuestra escena...

---

## Hola Mundo

<!-- .slide: data-background="media/img/aframe.png" data-transition="fade-in slide-out" -->

```html
<html>
  <script src="https://aframe.io/releases/0.3.2/aframe.min.js"></script>
  <a-scene>
    <a-box color="#4CC3D9" position="-1 0.5 -3" rotation="0 45 0"></a-box>
    <a-cylinder color="#FFC65D" position="1 0.75 -3" radius="0.5" height="1.5"></a-cylinder>
    <a-sphere color="#EF2D5E" position="0 1.25 -5" radius="1.25"></a-sphere>
    <a-plane color="#7BC8A4" position="0 0 -4" rotation="-90 0 0" width="4" height="4"></a-plane>
    <a-sky color="#ECECEC"></a-sky>
  </a-scene>
</html>
```
<!-- .element: class="stretch" -->

<!-- NOTES -->
- Elementos primitivos de 3D Básico con Custom Elements
- Legible: HTML es posiblemente el lenguaje más accesible en computación
- Encapsulado: copiar-y-pegar HTML en cualquier lugar y todavía funciona sin estado o variables
- Mira rápidamente un ejemplo en vivo...

---

## Hola Metaverso

<i>por Ada Rose Edwards (@lady_ada_king)</i>

<!-- .slide: data-background="media/img/metaverse.png" -->

<div class="stretch" data-aframe-scene="scenes/80s.html"></div>

<!-- NOTES -->
- Una escena hecha por Ada Rose Edwards ejecutándose dentro de mis diapositiva HTML
- Funciona en escritorio, Android, iOS, Samsung Gear VR, Oculus Rift, HTC Vive
- Podría abrir el Inspector de DOM para cambiar los valores en vivo
- Ya que es sólo HTML...

---

<!-- .slide: data-background="media/img/aframe.jpg" -->

## Funciona en todo

<div class="captioned-image-row">
  <div>
    <img data-src="media/img/d3.png">
    <i>d3.js</i>
  </div>
  <div>
    <img data-src="media/img/vue.png">
    <i>Vue.js</i>
  </div>
  <div>
    <img data-src="media/img/react.png">
    <i>React</i>
  </div>
  <div>
    <img data-src="media/img/redux.png">
    <i>Redux</i>
  </div>
  <div>
    <img data-src="media/img/jquery.png">
    <i>jQuery</i>
  </div>
  <div>
    <img data-src="media/img/angular.png">
    <i>Angular</i>
  </div>
</div>

<!-- NOTES -->

- Basado en HTML, compatible con todas las librarías/frameworks existentes
- Buena razón para tener HTML como capa intermediaria entre WebGL/three.js
- Todas las herramientas fueron pensadas con la noción de HTML
- Bajo el capó, A-Frame es un framework extensible y declarativo para three.js...

------

# Entidad-Componente-Sistema

<!-- .slide: data-background="media/img/minecraft-blocks.png" -->

<!-- NOTES -->
- Es un framework de entidad-componente
- Popular en el desarrollo de juegos, usado por Unity
- Todos los objetos en la escena son **entidades** que vacían objetos inherentemente. Conectar
  **componentes** para adjuntar apariencia / comportamiento / funcionalidad
- La web 2D en donde cada elemento estaba fijo
- 3D/VR es diferente, objetos de tipos infinitos y complejidades, se necesita una manera fácil de construir diferentes tipos de objetos

---

<!-- .slide: data-background="media/img/minecraft-blocks.png" data-transition="slide-in none" -->

## Composición de una entidad

```html
<a-entity>
```
<!-- .element: class="stretch" -->

<!-- NOTES -->
- Empezar con un `<a-entity>`
- Por si mismo, no tiene apariencia, comportamiento o funcionalidad
- Conectar componentes para agregar apariencia, comportamiento, funcionalidad

---

## Composición de una entidad

<!-- .slide: data-background="media/img/minecraft-blocks.png" data-transition="none" -->

```html
<a-entity
  geometry="primitive: sphere; radius: 1.5"
  material="color: #343434; roughness: 0.4; sphericalEnvMap: #texture">
```
<!-- .element: class="stretch" -->

<!-- NOTES -->
- Sintaxis similar a los estilos CSS
- Nombre de componentes como atributos HTML
- Propiedades de componentes y valores como atributos HTML

---

## Composición de una entidad

<!-- .slide: data-background="media/img/minecraft-blocks.png" data-transition="none" -->

```html
<a-entity
  geometry="primitive: sphere; radius: 1.5"
  material="color: #343434; roughness: 0.4; sphericalEnvMap: #texture"
  position="-1 2 4" rotation="45 0 90" scale="2 2 2">
```
<!-- .element: class="stretch" -->

---

## Composición de una entidad

<!-- .slide: data-background="media/img/minecraft-blocks.png" data-transition="none" -->

```html
<a-entity
  geometry="primitive: sphere; radius: 1.5"
  material="color: #343434; roughness: 0.4; sphericalEnvMap: #texture"
  position="-1 2 4" rotation="45 0 90" scale="2 2 2"
  animation="property: rotation; loop: true; to: 0 360 0"
  movement-pattern="type: spline; speed: 4">
```
<!-- .element: class="stretch" -->

---

## Composición de una entidad

<!-- .slide: data-background="media/img/minecraft-blocks.png" data-transition="none" -->

```html
<a-entity
  json-model="src: #robot"
  position="-1 2 4" rotation="45 0 90" scale="2 2 2"
  animation="property: rotation; loop: true; to: 0 360 0"
  movement-pattern="type: spline; speed: 4">
```
<!-- .element: class="stretch" -->

---

## Composición de una entidad

<!-- .slide: data-background="media/img/minecraft-blocks.png" data-transition="none" -->

```html
<a-entity
  json-model="src: #robot"
  position="-1 2 4" rotation="45 0 90" scale="2 2 2"
  animation="property: rotation; loop: true; to: 0 360 0"
  movement-pattern="type: attack; target: #player"
  explode="on: hit">
```
<!-- .element: class="stretch" -->

---

## Escribiendo un Componente

<!-- .slide: data-background="media/img/minecraft-blocks.png" data-transition="none" -->

```js
AFRAME.registerComponent('my-component', {
  schema: {
    foo: {type: 'selector'},
    bar: {default: 256}
  },

  init: function () { // ... },
  update: function () { // ... },
  remove: function () { // ... },
  tick: function () { // ... }
});
```
<!-- .element: class="stretch" -->

```html
<a-box my-component="foo: #box; bar: 300"></a-box>
```

<!-- NOTES -->
- `schema`: define cómo los datos son parseados desde HTML
- Métodos del ciclo de vida:
  - `init`: agregar componente, como `componenteSeMonta`
  - `update`: actualizar datos del componente, como `componenteRecibePropiedades`
  - `remove`: separar componente, como `componentSeDesmonta`
  - `tick`: ejecutar en cada frame
- Propiedades:
  - `el`: referencia al elemento de la entidad
  - `data`: datos del componente parseados desde HTML
  - `object3D`: objeto de three.js

---

<!-- .slide: data-background="media/img/standard-components.png" data-background-size="contain" -->

<!-- NOTES -->
- Estos son algunos de los componentes que se incluyen con A-Frame
- A-Frame es completamente extensible en su núcleo...

---

<!-- .slide: data-background="media/img/community-components.png" data-background-size="contain" -->

<!-- NOTES -->
- Comunidad ha llenado el ecosistema con toneladas de componentes
- Los componentes puede hacer lo que quieran, tienen acceso completo a three.js y las Web API
- El ecosistema componente es el elemento vital de A-Frame
- Física, movimiento de salto, sistemas de partículas, visualizaciones de audio, océanos
- Poner estos elementos como etiquetas script y usarlas directamente desde HTML
- Desarrolladores avanzados que potencian a otros desarrolladores
- Trabajando en la recolección de estos componentes...

---

<div class="icon-title">
  <img data-src="media/img/registry.png" width="64">
  <h2>Registro</h2>
</div>

<!-- .slide: data-background="media/img/aframe-side.png" -->

Una gran colección de componentes/sombreadores de A-Frame.

<a class="stretch" href="https://aframe.io/aframe-registry">
  <video loop data-src="media/video/registrypreview.mp4" data-autoplay></video>
</a>

<!-- NOTES -->
- Obtenerlos desde el registro de A-Frame
- Como una tienda de componentes que nos asegura que funcionen bien
- Las personas pueden navegar y buscar componentes o instalarlos....

---

## Inspector

<!-- .slide: data-background="media/img/inspector.png" data-state="state--bg-dark" -->

La herramienta visual para A-Frame. Sólo `<ctrl>+<alt>+i`.

<div class="stretch" data-aframe-scene="scenes/80s.html"></div>

------

<!-- .slide: data-background-video="media/video/a-painter.mp4" data-background-video-muted="true" data-state="state--bg-dark" -->

## A-Painter

Pintar en VR en el navegador.

<!-- NOTES -->
- A-Frame es una herramienta poderosa
- 90+fps a escala de una sala experiencia de TiltBrush en pocas semanas con sólo A-Frame

---

# aframe.io

<div class="captioned-image-row">
  <div>
    <img data-src="media/img/github.png">
    <i>75 contribuidores 3500 soñadores</i>
  </div>
  <div>
    <img data-src="media/img/slack.png">
    <i>1750 miembros en Slack</i>
  </div>
  <div>
    <img data-src="media/img/scene-collage-circle.png">
    <i>100+ proyectos destacados</i>
  </div>
</div>

<!-- NOTES -->
- Proyecto de código abierto e inclusivo
- La mayoría de trabajos están en GitHub
- Comunidad activa en Slack para compartir proyectos, interactuar, reunirse, buscar ayuda
- Proyectos destacados en el repositorio `awesome-aframe` y en el blog *A Week of A-Frame*
