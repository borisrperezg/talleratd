---
title: "Archimate"
chapter: false
weight: 5
disableToc: true
pre : "<b>1.3 </b>"
---

**Archimate** es una especificación, para el modelado de arquitecturas empresariales. Provee un lenguaje visual con un conjunto de iconografías para describir, analizar, y comunicar aspectos de arquitectura de TI. El **objetivo** de Archimate es proveer una representación uniforme para expresar a los stakeholders, aspectos de modelado de la organización, así como decisiones de tecnología.

Una de las ventajas de ArchiMate es que proporciona una representación visual y fomenta el uso de diferentes colores para resaltar las diferentes capas de modelado. Las tres principales capas: negocio, aplicación y tecnología, pertenecen a un marco completo que puede ampliarse con capas adicionales (física, estrategia y migración). Además, los métodos de arquitectura empresarial pueden utilizarse para proporcionar la estructura organizativa, los procesos de negocio y la infraestructura informática de una empresa.
![Archimate](/images/Pic_ArchiMateFrame.png?width=500px)

#### Aplicación en Rebel

Rebel hace uso de modelos de Archimate compuestos por las capas Estrategia, Negocio y Aplicación. La capa Tecnología está contemplada para incluirse más adelante. Estas tres capas seleccionadas permiten alinear las necesidades de la organización con la arquitectura. Adicionalmente, Rebel extiende las capacidades de Archimate al permitir que se definan propiedades para las interfaces (elementos de la capa de aplicación a través de la cual un componente expone una funcionalidad). Estas propiedades se obtuvieron de la taxonomía de tipos de conectores (diagramas Componente & Conector) y sus dimensiones propuesta por Richard Taylor, entre las cuales están: Delivery, Buffering, Throughput, Synchronicity y Notification.