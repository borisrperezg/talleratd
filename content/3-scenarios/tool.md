---
title : "Rebel"
weight : 32
chapter : false
pre : "<b>3.2 </b>"
---

Rebel es una herramienta semiautomática, basada en modelos, que se enfoca en la construcción de un modelo de clasificación binaria para la identificación de ATD, a partir de los artefactos producidos durante la etapa de diseño de la arquitectura del sistema. Este modelo identificará automáticamente items candidatos de ATD y el arquitecto será el responsable de aceptar o rechazar los candidatos. 

Esta propuesta se centra en la TD a nivel de arquitectura, sin tener en cuenta el código fuente. Se espera que funcione con equipos de software que manejen varias versiones de la arquitectura y varios artefactos heterogéneos. 

El elemento central de esta propuesta es el Bloque de Interés (BoI). Un BoI representa la evolución de los elementos de la arquitectura durante el diseño del software. Una BoI se compone de hechos (facts), donde cada hecho (fact) representa un cambio en la relación de elemento arquitectónico, o de sus propiedades. Por ejemplo, si en la versión 1 de un modelo existen los componentes C1 y C2, y en la versión 2 se crea una relación entre ellos, entonces esta relación corresponderá a un Hecho (Fact). Del mismo modo, los componentes C1 y C2 corresponderán a Hechos (Facts).

La idea de Rebel, es que un hecho es la mínima expresión de un item de ATD, y por lo tanto, esta propuesta busca describir todos los hechos, a partir de las versiones de modelos, para que el arquitecto pueda realizar una marcación manual de items de ATD. A partir de esta marcación manual, se entrena un modelo, para ser usado en nuevos BoIs para identificar de forma automática la ATD sobre los hechos de esos modelos. Es importante mencionar que en la medida que se tengan más datos de Proyectos y ATD identificadas, más candidatos confirmados/rechazados por arquitectos, el modelo irá mejorando su precisión.

Lo que se busca al marcar cada uno de estos Hechos como ATD, es permitirle al modelo que aprenda sobre comportamientos o estructuras que deben inferirse en nuevos modelos. Esto es, si al interior de una empresa de software está establecido que las dependencias cíclicas son ATD, y así mismo se entrena un modelo con esta información, entonces, cada nuevo BoI donde se presenten dependencias cíclicas serán considerados ATD.

Las tres etapas contempladas en Rebel son: 

* **Preparación:** En esta etapa se deben cargar los artefactos producidos durante la etapa de diseño de la arquitectura, tales como modelos en Archimate, modelos Componente y Conector (C&C), chats, emails, decisiones de arquitectura, y logs de commits.
* **Entrenamiento:** En esta etapa el arquitecto crear un BoI a partir de un modelo de Archimate, y marca todos los hechos (facts) que considera como items de ATD. Adicionalmente, debe justificarlos.
* **Identificación:** En esta etapa el arquitecto deberá crear un BoI y el modelo entrenado de identificación se encargará de marcar como items candidatos de ATD a todos aquellos hechos (facts) que cumplan con determinadas características.