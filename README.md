# Deslim Fleet - App Android para checklist limpieza y desinfección flota barcos

Deslim Fleet es una app para móviles Android creada en lenguaje Kotlin y usando JetPack Compose para la UI. Se desarrolló para el proyecto de fin de ciclo de Desarrollo de Aplicaciones Multiplataforma (DAM) a raíz de la idea de un amigo que tiene una empresa de desinfección que trabaja en flotas de barcos. En este sentido, el propósito es automatizar el proceso típico de checklist en lápiz y papel del personal de una naviera, cuando tiene que ir estancia por estancia revisando todos los apartados.

Una vez recopilados todos los datos, esa misma persona u otra debe volcar todos los datos desde el papel a una base de datos o sistema informático. Este proceso es un trabajo tedioso para el personal de barcos realizarlo a diario y conlleva mucha probabilidad de errores.

La app Deslim Fleet soluciona todos estos problemas y automatiza este proceso. Además, tiene un modelo de IA integrada de Google (Gemini) que realiza un informe en formato pdf sobre una inspección en concreto, por lo que se proporciona un valor añadido para los usuarios administradores que revisan las inspecciones. 

Teniendo todo lo anterior en cuenta, la idea de desarrollar la app para dar solución a este problema fue tomando forma hasta el punto presentarla para el proyecto final de FP y estar actualmente en conversaciones con varios responsables de navieras para su comercialización.

### Funcionamiento

El funcionamiento de la app Deslim Fleet es muy sencillo, los usuarios se loguean y, dependiendo del rol del usuario, tendrán acceso a una pantalla de generación de informes (administradores) o a la pantalla de estado de las revisiones de la flota de barcos (usuarios normales). 

Los usuarios con rol administrador acceden directamente a la pantalla de revisiones, seleccionan un barco, zona y fecha concretos. En caso de haber revisión, la app carga automáticamente un fichero .pdf con información de la revisión generada por Gemini, que se puede descargar, enviar por mail o compartir por mensajería instantánea.

Los usuarios ven los diferentes barcos y las zonas que ya han sido inspeccionadas ese día y las que no, por lo que si quieren iniciar una nueva revisión pasan a la siguiente pantalla, seleccionan el barco, la zona del barco y ya van rellenando la pantalla del checklist de la revisión propiamente dicha. Dicho checklist está dividido entre secciones y subsecciones de una zona del barco, y se puede indicar si está o no limpia y desinfectada, si hay plaga, si se requiere reparación, añadir comentarios o fotos. Una vez marcados todos los check de sí/no, se habilitará el botón para crear la revisión y guardarla en nuestra base de datos (Plataforma Firebase). 

### Comercialización y despliegue de la app

Como se ha indicado al principio, se mantienen conversaciones con responsables de algunas navieras que trabajan en España para comercializar y distribuir la app. Está previsto que se despliegue en Google Play, o bien con una monetización de suscripción o por pago por descarga por cada dispositivo. 

Para mayor información, se puede visitar el vídeo explicativo de cómo se realiza una revisión de una zona de un barco en Youtube: [(https://youtu.be/T_02t57-XPM)]
