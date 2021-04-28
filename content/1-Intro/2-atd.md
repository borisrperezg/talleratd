---
title: "ATD"
chapter: false
weight: 3
disableToc: true
pre : "<b>1.2 </b>"
---

**La Deuda Técnica en Arquitectura (ATD)** es una metáfora utilizada para expresar el conjunto de decisiones de arquitectura que buscan favorecer ciertos objetivos a corto plazo, pero causando un impacto negativo en la calidad interna del sistema, como la mantenibilidad y capacidad de evolución. Típicamente, la ATD incluye Architecural Smells, uso de anti-patrones de arquitectura, violaciones de buenas prácticas arquitecturales, entre otros.

El problema de la deuda aparece cuando no se documenta, y por lo tanto, se pierde de vista. Cuando no se controla la deuda, esta puede afectar o ralentizar la incorporación de nuevo valor al producto. A raíz de esto, se vuelve clave que los equipos de software, encabezados por los arquitectos de software, puedan realizar seguimiento y gestión a los ítems de deuda técnica inyectados en el sistema. Para lograrlo, es indispensable partir por su identificación. Una vez identificada, el equipo de desarrollo podrá cuantificar su impacto, hacerle seguimiento, priorizarlos y eventualmente tomar la decisión de pagar la deuda (refactorizar o reescribir el código). La identificación, y subsecuente gestión, de la ATD permite que se reconozcas sus beneficios, como por ejemplo, salir a producción más rápido, acelerar procesos de codificación, agilizar la comunicación entre componentes, entre otros. Estas acciones inyectarán deuda, pero se tendrá conocimiento de ésta, y se podrá hacer seguimiento.

Los enfoques actuales para la identificación de la ATD se basan principalmente en la revisión del código fuente, para identificar tipos de ATD, como la falta de modularización. Sin embargo, no es del todo conveniente que el equipo de software deba esperar a tener la aplicación implementada para identificar casos de ATD. Otro enfoque de identificación de ATD consiste en organizar reuniones con los arquitectos en las cuales se revisen las decisiones tomadas y la deuda inyectada con cada una de estas. Este proceso es bastante exhaustivo y completo, pero consume mucho tiempo, y por lo tanto, no sería del todo conveniente para algunas organizaciones.