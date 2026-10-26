<div class="portada">

<img src="img/logo.png" alt="Logo NotaRA" width="180">

# NotaRA

## Sistema de Gestión de Resultados de Aprendizaje

**Documento consolidado de artefactos del proyecto**

Ingeniería de Software IV · Universidad Católica de Oriente\
Profesora: Luz Mery Ríos

**Integrantes**

Iván Daniel Naranjo Botero\
María Andrea Avendaño Jurado\
Maicol Oviedo Quintero\
María Salome González Blandón\
Tomas Gómez Cifuentes\
Alejandro Arbelaez\
Tomás Marín Estrada

Rionegro, septiembre de 2026

</div>

<div class="salto"></div>

## Contenido

1. [Visión del proyecto](#1-visión-del-proyecto)
2. [Mapa de impacto](#2-mapa-de-impacto)
3. [Especificación de requisitos (SRS)](#3-especificación-de-requisitos-srs)
4. [Historias de usuario y criterios de aceptación](#4-historias-de-usuario-y-criterios-de-aceptación)
5. [Mapas de historias de usuario](#5-mapas-de-historias-de-usuario)
6. [Modelo de dominio](#6-modelo-de-dominio)
7. [Diagrama de clases de dominio](#7-diagrama-de-clases-de-dominio)
8. [Diagrama de datos](#8-diagrama-de-datos)
9. [Arquitectura](#9-arquitectura)
10. [Diagrama de componentes](#10-diagrama-de-componentes)
11. [Diagrama de paquetes](#11-diagrama-de-paquetes)

> Cada artefacto se abre y se cierra con clic en **▶**.
>
> Cada sección incluye también el desplegable **💡 Ver explicación para el usuario**, que explica en lenguaje sencillo qué es el artefacto, cómo se lee y qué significa cada parte.
>
> **RA (Resultado de Aprendizaje):** lo que un estudiante debe saber o saber hacer al terminar una asignatura. Es el concepto central de NotaRA.

<div class="salto"></div>

## 1. Visión del proyecto

Define el público objetivo, la necesidad, el beneficio principal y la diferenciación del producto.

| Herramienta | Abrir en línea | Archivo |
|---|---|---|
| Word (SharePoint) | [🔗 Abrir](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7BA2E56781-938C-40B1-AA6B-861D2F022AF8%7D&file=Vision_Proyecto.docx&action=default&mobileredirect=true) | [PDF](anexos/A2_Vision_Proyecto.pdf) |

<details>
<summary><b>📄 Ver documento (2 páginas)</b></summary>

<div class="pagina">

[![Visión – página 1](img/vision/vision-1.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7BA2E56781-938C-40B1-AA6B-861D2F022AF8%7D&file=Vision_Proyecto.docx&action=default&mobileredirect=true)

*Página 1 de 2*

</div>

<div class="pagina">

[![Visión – página 2](img/vision/vision-2.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7BA2E56781-938C-40B1-AA6B-861D2F022AF8%7D&file=Vision_Proyecto.docx&action=default&mobileredirect=true)

*Página 2 de 2*

</div>


</details>

<details>
<summary><b>💡 Ver explicación para el usuario</b></summary>

**¿Qué es este documento?** Es la carta de presentación de NotaRA. En dos páginas explica, sin tecnicismos, por qué existe el sistema y para quién se construye. Es el punto de partida de todos los demás artefactos de este documento.

**¿Qué preguntas responde?**

**Público objetivo:** ¿a quién está dirigido NotaRA?

**Necesidad:** ¿qué problema tienen hoy esas personas?

**Beneficio principal:** ¿qué ganan al usar el sistema?

**Diferenciación:** ¿en qué se distingue NotaRA de otras alternativas?

**¿Cuándo leerlo?** Es el mejor documento para entender NotaRA en pocos minutos. Los requisitos, las historias de usuario y los diagramas que vienen después desarrollan en detalle lo que aquí se plantea.

</details>

<div class="salto"></div>

## 2. Mapa de impacto

Relaciona el objetivo del proyecto con los actores, los impactos esperados, los entregables y las historias de usuario.

| Herramienta | Abrir en línea |
|---|---|
| Figma | [🔗 Abrir](https://www.figma.com/make/T7M6YdUiBXzHYP5DHBsVgf/Mapa-de-Impacto-Cognipath?t=CtKpGkCl4GerlKfm-1) |

<details>
<summary><b>👤 Administrador</b></summary>

[![Mapa de impacto – Administrador](img/mapa-impacto-administrador.png)](https://www.figma.com/make/T7M6YdUiBXzHYP5DHBsVgf/Mapa-de-Impacto-Cognipath?t=CtKpGkCl4GerlKfm-1)

</details>

<details>
<summary><b>👤 Docente</b></summary>

[![Mapa de impacto – Docente](img/mapa-impacto-docente.png)](https://www.figma.com/make/T7M6YdUiBXzHYP5DHBsVgf/Mapa-de-Impacto-Cognipath?t=CtKpGkCl4GerlKfm-1)

</details>

<details>
<summary><b>👤 Estudiante</b></summary>

[![Mapa de impacto – Estudiante](img/mapa-impacto-estudiante.png)](https://www.figma.com/make/T7M6YdUiBXzHYP5DHBsVgf/Mapa-de-Impacto-Cognipath?t=CtKpGkCl4GerlKfm-1)

</details>

<details>
<summary><b>💡 Ver explicación para el usuario</b></summary>

**¿Qué es este diagrama?** Es un mapa que conecta el propósito de NotaRA con lo que se va a construir. Sirve para comprobar que cada función del sistema existe por una razón concreta y que beneficia a alguien.

**¿Cómo se lee?** De izquierda a derecha, respondiendo cinco preguntas en orden. Son las cinco columnas numeradas de la parte superior:

**① Objetivo: ¿para qué existe el sistema?** Mejorar la gestión y el seguimiento de los Resultados de Aprendizaje mediante una plataforma web centralizada. Con esto se busca reducir el trabajo manual, mejorar la trazabilidad (saber quién hizo qué y cuándo) y facilitar el análisis del desempeño académico.

**② Actores: ¿a quién ayuda?** A tres tipos de personas: el administrador, el docente y el estudiante. Cada uno tiene su propio desplegable arriba.

**③ Impactos: ¿qué cambio queremos lograr en esa persona?** Por ejemplo, que el docente pueda “conocer rápidamente el desempeño de sus estudiantes y grupos”.

**④ Entregables: ¿qué vamos a construir para lograrlo?** Son las funciones concretas del sistema (los recuadros morados), como el “cálculo automático de nota del RA” o la “exportación de reportes PDF”.

**⑤ Historias de usuario: ¿cómo lo pide el usuario con sus propias palabras?** Siguen la forma “Como [rol], quiero [algo], para [beneficio]”. Su color cambia según el actor: verde para el administrador, azul para el docente y naranja para el estudiante.

**¿Qué busca cada actor?**

**Administrador** (gestiona usuarios, asignaturas, grupos y RA): administrar de forma centralizada la estructura académica y los usuarios, supervisar el desempeño académico con información consolidada y contar con información confiable y trazable.

**Docente** (planea evaluaciones, registra calificaciones, agrega observaciones y gestiona planes de mejora): planificar y ejecutar evaluaciones por cada RA, conocer rápidamente el desempeño de sus estudiantes y grupos, identificar los RA que requieren mejora y hacer seguimiento a la evolución de sus estudiantes.

**Estudiante** (consulta resultados, desempeño, observaciones e historial, y responde con contracomentarios): consultar con claridad sus calificaciones y niveles de desempeño, comprender las observaciones del docente, identificar qué RA debe mejorar y seguir su evolución académica.

**Ejemplo de lectura completa:** Objetivo → Docente → “Conocer rápidamente el desempeño de sus estudiantes y grupos” → entregable “Cálculo automático de nota del RA” → historia “Como docente, quiero que el sistema calcule automáticamente la nota del RA, para reducir errores de cálculo”.

</details>

<div class="salto"></div>

## 3. Especificación de requisitos (SRS)

Requisitos funcionales (RF-01 a RF-28), no funcionales y restricciones del sistema, bajo el estándar IEEE 830.

| Herramienta | Abrir en línea | Archivo |
|---|---|---|
| Google Docs | [🔗 Abrir](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true) | [PDF](anexos/A1_SRS_IEEE830.pdf) |

<details>
<summary><b>📄 Ver documento (29 páginas)</b></summary>

<div class="pagina">

[![SRS – página 1](img/srs/srs-01.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 1 de 29*

</div>

<div class="pagina">

[![SRS – página 2](img/srs/srs-02.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 2 de 29*

</div>

<div class="pagina">

[![SRS – página 3](img/srs/srs-03.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 3 de 29*

</div>

<div class="pagina">

[![SRS – página 4](img/srs/srs-04.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 4 de 29*

</div>

<div class="pagina">

[![SRS – página 5](img/srs/srs-05.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 5 de 29*

</div>

<div class="pagina">

[![SRS – página 6](img/srs/srs-06.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 6 de 29*

</div>

<div class="pagina">

[![SRS – página 7](img/srs/srs-07.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 7 de 29*

</div>

<div class="pagina">

[![SRS – página 8](img/srs/srs-08.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 8 de 29*

</div>

<div class="pagina">

[![SRS – página 9](img/srs/srs-09.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 9 de 29*

</div>

<div class="pagina">

[![SRS – página 10](img/srs/srs-10.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 10 de 29*

</div>

<div class="pagina">

[![SRS – página 11](img/srs/srs-11.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 11 de 29*

</div>

<div class="pagina">

[![SRS – página 12](img/srs/srs-12.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 12 de 29*

</div>

<div class="pagina">

[![SRS – página 13](img/srs/srs-13.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 13 de 29*

</div>

<div class="pagina">

[![SRS – página 14](img/srs/srs-14.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 14 de 29*

</div>

<div class="pagina">

[![SRS – página 15](img/srs/srs-15.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 15 de 29*

</div>

<div class="pagina">

[![SRS – página 16](img/srs/srs-16.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 16 de 29*

</div>

<div class="pagina">

[![SRS – página 17](img/srs/srs-17.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 17 de 29*

</div>

<div class="pagina">

[![SRS – página 18](img/srs/srs-18.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 18 de 29*

</div>

<div class="pagina">

[![SRS – página 19](img/srs/srs-19.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 19 de 29*

</div>

<div class="pagina">

[![SRS – página 20](img/srs/srs-20.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 20 de 29*

</div>

<div class="pagina">

[![SRS – página 21](img/srs/srs-21.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 21 de 29*

</div>

<div class="pagina">

[![SRS – página 22](img/srs/srs-22.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 22 de 29*

</div>

<div class="pagina">

[![SRS – página 23](img/srs/srs-23.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 23 de 29*

</div>

<div class="pagina">

[![SRS – página 24](img/srs/srs-24.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 24 de 29*

</div>

<div class="pagina">

[![SRS – página 25](img/srs/srs-25.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 25 de 29*

</div>

<div class="pagina">

[![SRS – página 26](img/srs/srs-26.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 26 de 29*

</div>

<div class="pagina">

[![SRS – página 27](img/srs/srs-27.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 27 de 29*

</div>

<div class="pagina">

[![SRS – página 28](img/srs/srs-28.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 28 de 29*

</div>

<div class="pagina">

[![SRS – página 29](img/srs/srs-29.jpg)](https://docs.google.com/document/d/19pyy0sIWytxa98GQGcBURgEOkAS2wMnu/edit?usp=sharing&ouid=115767164584929518590&rtpof=true&sd=true)

*Página 29 de 29*

</div>


</details>

<details>
<summary><b>💡 Ver explicación para el usuario</b></summary>

**¿Qué es este documento?** Es la descripción precisa de lo que NotaRA debe hacer. Funciona como un acuerdo entre quienes piden el sistema y quienes lo construyen: si algo no está aquí, no forma parte del alcance. Sus siglas vienen del inglés *Software Requirements Specification* (Especificación de Requisitos de Software).

**¿Qué contiene?**

**Requisitos funcionales (RF-01 a RF-28):** las acciones que el sistema debe permitir, cada una identificada con un código. Por ejemplo, los relacionados con usuarios y accesos (RF-01 a RF-04) o con la parte académica y de evaluación (RF-05 a RF-22).

**Requisitos no funcionales:** cómo debe comportarse el sistema mientras hace esas acciones, por ejemplo qué tan seguro, rápido, disponible o fácil de usar debe ser.

**Restricciones:** condiciones que limitan la forma de construir el sistema, como tecnologías o normas que se deben respetar.

**¿Qué es IEEE 830?** Es una norma internacional que indica cómo organizar este tipo de documento para que sea claro, completo y verificable.

**¿Para qué le sirve al lector?** Los códigos RF se repiten en los demás artefactos. Por ejemplo, el diagrama de clases agrupa sus módulos por rangos de RF. Así se puede rastrear cada requisito hasta la parte del sistema que lo cumple.

</details>

<div class="salto"></div>

## 4. Historias de usuario y criterios de aceptación

Historias de usuario HU001 a HU030, cada una con sus criterios de aceptación.

| Herramienta | Abrir en línea | Archivo |
|---|---|---|
| Word (SharePoint) | [🔗 Abrir](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true) | [PDF](anexos/A3_Historias_de_Usuario.pdf) |

<details>
<summary><b>📄 Ver documento (30 páginas)</b></summary>

<div class="pagina">

[![Historias de usuario – página 1](img/hu/hu-01.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 1 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 2](img/hu/hu-02.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 2 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 3](img/hu/hu-03.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 3 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 4](img/hu/hu-04.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 4 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 5](img/hu/hu-05.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 5 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 6](img/hu/hu-06.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 6 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 7](img/hu/hu-07.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 7 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 8](img/hu/hu-08.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 8 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 9](img/hu/hu-09.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 9 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 10](img/hu/hu-10.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 10 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 11](img/hu/hu-11.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 11 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 12](img/hu/hu-12.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 12 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 13](img/hu/hu-13.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 13 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 14](img/hu/hu-14.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 14 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 15](img/hu/hu-15.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 15 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 16](img/hu/hu-16.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 16 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 17](img/hu/hu-17.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 17 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 18](img/hu/hu-18.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 18 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 19](img/hu/hu-19.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 19 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 20](img/hu/hu-20.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 20 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 21](img/hu/hu-21.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 21 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 22](img/hu/hu-22.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 22 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 23](img/hu/hu-23.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 23 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 24](img/hu/hu-24.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 24 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 25](img/hu/hu-25.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 25 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 26](img/hu/hu-26.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 26 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 27](img/hu/hu-27.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 27 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 28](img/hu/hu-28.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 28 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 29](img/hu/hu-29.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 29 de 30*

</div>

<div class="pagina">

[![Historias de usuario – página 30](img/hu/hu-30.jpg)](https://uconet.sharepoint.com/sites/SIGRA_A/_layouts/15/Doc.aspx?sourcedoc=%7B135C4B48-F580-4581-9A44-9B6AD4B0D3D1%7D&file=Historias_usuario_sfw4%201.docx&action=default&mobileredirect=true)

*Página 30 de 30*

</div>


</details>

<details>
<summary><b>💡 Ver explicación para el usuario</b></summary>

**¿Qué es este documento?** Reúne las necesidades del sistema escritas desde el punto de vista de quien lo va a usar, no del programador. Son 30 historias, identificadas de HU001 a HU030.

**¿Cómo se lee una historia?** Se escribe con la estructura “Como [rol], quiero [acción], para [beneficio]”. Así cada función deja claro quién la usa y para qué le sirve. Por ejemplo, en el mapa de impacto aparece: “Como estudiante, quiero consultar mis notas por RA, para conocer mi desempeño”.

**¿Qué son los criterios de aceptación?** Son las condiciones concretas que deben cumplirse para dar una historia por terminada. Funcionan como una lista de chequeo: si al probar el sistema todas se cumplen, la historia está lista.

**¿Cómo se relaciona con lo demás?** El mapa de impacto explica por qué se necesitan estas historias, y los mapas de historias las organizan en tareas y entregas.

</details>

<div class="salto"></div>

## 5. Mapas de historias de usuario

Tareas de cada rol organizadas por actividad y por release (Must have, Should have y Could have).

| Rol | Abrir en línea |
|---|---|
| Estudiante | [🔗 Figma](https://www.figma.com/make/82SzFurn0roOcVHFA1WEJ3/Mapa-de-usuarios-estudiantes?t=j2iu78LdHrvgZoxq-1) |
| Administrador | [🔗 Figma](https://www.figma.com/make/agwgJZcdcDJmVYQDitD3Y0/User-history?fullscreen=1&t=jBOBEZOfg3Xl9WHe-1&code-node-id=0-6) |
| Docente | [🔗 Figma](https://www.figma.com/make/cJD75Lh1zTEKj4sg4IDmbo/map-history-user-rol-docente?t=knX2wQhD6058jyAi-1) |

<details>
<summary><b>👤 Estudiante</b></summary>

[![Mapa de historias – Estudiante](img/mapa-historias-estudiante.png)](https://www.figma.com/make/82SzFurn0roOcVHFA1WEJ3/Mapa-de-usuarios-estudiantes?t=j2iu78LdHrvgZoxq-1)

</details>

<details>
<summary><b>👤 Administrador</b></summary>

[![Mapa de historias – Administrador](img/mapa-historias-administrador.png)](https://www.figma.com/make/agwgJZcdcDJmVYQDitD3Y0/User-history?fullscreen=1&t=jBOBEZOfg3Xl9WHe-1&code-node-id=0-6)

</details>

<details>
<summary><b>👤 Docente</b></summary>

[![Mapa de historias – Docente](img/mapa-historias-docente.png)](https://www.figma.com/make/cJD75Lh1zTEKj4sg4IDmbo/map-history-user-rol-docente?t=knX2wQhD6058jyAi-1)

</details>

<details>
<summary><b>💡 Ver explicación para el usuario</b></summary>

**¿Qué es este diagrama?** Es el recorrido de cada tipo de usuario por NotaRA, dividido en tareas pequeñas y ordenado según qué se construye primero. Hay uno por cada rol: estudiante, administrador y docente.

**¿Cómo se lee?**

**De izquierda a derecha (las flechas de arriba):** las actividades grandes que hace el usuario, en el orden en que normalmente las hace.

**De arriba hacia abajo (las filas “Release”):** las entregas del sistema. La primera fila es lo que debe estar listo primero; las siguientes se agregan después.

**Cada tarjeta:** una tarea concreta, con su código (t1, t2… en administrador y docente; e01, e02… en estudiante).

**El color de la tarjeta indica su prioridad:**

| Color | Prioridad | Significado |
|---|---|---|
| Rojo | Must have | Imprescindible: sin esto el sistema no cumple su propósito. |
| Amarillo | Should have | Importante, pero puede llegar en una entrega posterior. |
| Gris | Could have | Deseable: se agrega si hay tiempo y recursos. |

**Los números de la esquina superior derecha** resumen cada mapa:

| Rol | Actividades | Tareas | Imprescindibles | Entregas |
|---|---|---|---|---|
| Administrador | 7 | 55 | 27 | Core, Gestión, Completo |
| Docente | 9 | 53 | 48 | Core, Gestión, Completo |
| Estudiante | 7 | 42 | 26 | Esencial, Complementario, Deseable |

**El recorrido de cada rol:**

**Administrador:** Acceder → Gestionar usuarios → Gestionar asignaturas → Gestionar grupos y docentes → Gestionar RA → Consultar información → Analizar y reportar.

**Docente:** Acceder → Consultar asignación → Preparar evaluación → Evaluar → Consultar resultados → Retroalimentar → Mejorar → Analizar → Reportar.

**Estudiante:** Acceder → Consultar asignaturas → Consultar evaluaciones → Consultar resultados → Recibir retroalimentación → Participar en mejoramiento → Consultar historial.

**Ejemplo:** en el mapa del docente, “Registrar calificación” (t17) es imprescindible y está en la primera entrega, mientras que “Consultar frecuencia de observaciones” (t49) llega en la segunda.

</details>

<div class="salto"></div>

## 6. Modelo de dominio

Conceptos del negocio y sus relaciones, divididos en cinco módulos.

| Herramienta | Abrir en línea | Archivo |
|---|---|---|
| draw.io (Google Drive) | [🔗 Abrir](https://drive.google.com/file/d/12y8P6U4gscZQvt_0LywSyd0txrYzCEzk/view?usp=sharing) | [.drawio](anexos/A4_Modelo_Dominio.drawio) |

<details>
<summary><b>🧩 Usuarios y Accesos</b></summary>

[![Dominio – Usuarios y Accesos](img/dominio-1-usuarios-accesos.png)](https://drive.google.com/file/d/12y8P6U4gscZQvt_0LywSyd0txrYzCEzk/view?usp=sharing)

</details>

<details>
<summary><b>🧩 Académico</b></summary>

[![Dominio – Académico](img/dominio-2-academico.png)](https://drive.google.com/file/d/12y8P6U4gscZQvt_0LywSyd0txrYzCEzk/view?usp=sharing)

</details>

<details>
<summary><b>🧩 Evaluación</b></summary>

[![Dominio – Evaluación](img/dominio-3-evaluacion.png)](https://drive.google.com/file/d/12y8P6U4gscZQvt_0LywSyd0txrYzCEzk/view?usp=sharing)

</details>

<details>
<summary><b>🧩 Mejoramiento</b></summary>

[![Dominio – Mejoramiento](img/dominio-4-mejoramiento.png)](https://drive.google.com/file/d/12y8P6U4gscZQvt_0LywSyd0txrYzCEzk/view?usp=sharing)

</details>

<details>
<summary><b>🧩 Cálculo y Trazabilidad</b></summary>

[![Dominio – Cálculo y Trazabilidad](img/dominio-5-calculo-trazabilidad.png)](https://drive.google.com/file/d/12y8P6U4gscZQvt_0LywSyd0txrYzCEzk/view?usp=sharing)

</details>

<details>
<summary><b>💡 Ver explicación para el usuario</b></summary>

**¿Qué es este diagrama?** Es el mapa de conceptos de NotaRA. Muestra las ideas principales con las que trabaja el sistema (usuario, asignatura, Resultado de Aprendizaje, nota, observación…) y cómo se relacionan, usando el lenguaje de la universidad y no el de la programación. Para que sea fácil de leer está dividido en cinco módulos, que son los cinco desplegables de arriba.

**¿Cómo se lee?**

**Cada caja** es un concepto. El nombre grande está en español y debajo, en gris, aparece el nombre que recibe en el código (por ejemplo, Asignatura / Subject).

**Cada línea** es una relación y se lee como una frase siguiendo la flecha: “Asignatura → define → Resultado de Aprendizaje”. En sentido contrario se lee la otra frase: “Resultado de Aprendizaje ← pertenece a ← Asignatura”.

**Los números en los extremos** indican cuántos: 1 = exactamente uno; 0..* = ninguno o muchos; 1..* = al menos uno; 0..1 = ninguno o uno; 5..7 = entre cinco y siete.

**Los colores** indican de qué módulo viene cada concepto. Las cajas claras pertenecen al módulo que se está viendo; las de color vienen de otro módulo (gris = Usuarios y Accesos, azul claro = Académico, verde = Cálculo y Trazabilidad, rosado = Evaluación).

**Los óvalos de los costados** representan otros módulos. La flecha punteada indica que el módulo actual los utiliza.

**¿Qué dice cada módulo?**

**Usuarios y Accesos.** Un usuario puede solicitar ninguno o varios tokens de recuperación (códigos temporales para restablecer la contraseña), y cada token pertenece a un solo usuario.

**Académico.** Cada asignatura define entre 5 y 7 Resultados de Aprendizaje y puede impartirse en varios grupos de curso. Cada grupo es dictado por un docente y tiene estudiantes inscritos. El docente también puede publicar comentarios dirigidos a todo el grupo.

**Evaluación.** Cada RA se evalúa con al menos una actividad de evaluación. Cada actividad recibe las notas de los estudiantes, y cada nota pertenece a un solo estudiante. Una nota de actividad puede tener una observación del docente. Las observaciones se clasifican en categorías y también pueden referirse a la nota de un RA.

**Mejoramiento.** Un RA puede originar planes de mejoramiento, y cada plan pertenece a un estudiante. Es la forma de acompañar a quien necesita reforzar un RA.

**Cálculo y Trazabilidad.** Aquí se consolidan las notas: cada RA se resume en una nota de RA por estudiante, y cada asignatura en una nota final. El estudiante puede escribir un contracomentario para responder a una observación (cada observación recibe como máximo una respuesta). Además, todo cambio queda guardado en el historial de cambios junto con el usuario que lo hizo.

**¿Por qué es importante?** Asegura que el equipo y el cliente entiendan los conceptos del negocio de la misma forma antes de construir. Es la base del diagrama de clases y del diagrama de datos.

</details>

<div class="salto"></div>

## 7. Diagrama de clases de dominio

Clases del dominio con sus atributos, relaciones y enumeraciones.

| Herramienta | Abrir en línea | Archivo |
|---|---|---|
| draw.io (SharePoint) | [🔗 Abrir](https://uconet.sharepoint.com/sites/SIGRA_A/Shared%20Documents/Diagrama-Clases-Dominio.drawio) | [.drawio](anexos/A5_Diagrama_Clases_Dominio.drawio) |

<details>
<summary><b>🖼️ Ver diagrama</b></summary>

[![Diagrama de clases de dominio](img/diagrama-clases-dominio.png)](https://uconet.sharepoint.com/sites/SIGRA_A/Shared%20Documents/Diagrama-Clases-Dominio.drawio)

</details>

<details>
<summary><b>💡 Ver explicación para el usuario</b></summary>

**¿Qué es este diagrama?** Es la versión detallada del modelo de dominio. Toma los mismos conceptos y muestra exactamente qué datos guarda cada uno y cómo se conectan. Es el plano que siguen los programadores; por eso los nombres están en inglés, tal como aparecen en el código.

**¿Cómo se lee?**

**Cada caja es una “clase”**, es decir, la ficha de un concepto. Tiene tres partes: arriba el nombre; en el medio los datos que guarda (por ejemplo, un usuario guarda su nombre completo, documento, correo y si está activo); y abajo las acciones que se pueden hacer con esos datos (“getter/setter” significa consultarlos y modificarlos).

**Al lado de cada dato** está su tipo: texto (String), número entero (Integer, Long), número con decimales (Double), sí/no (Boolean), fecha (LocalDate) o fecha y hora (LocalDateTime).

**Las cajas moradas («enumeration»)** son listas de opciones fijas. Por ejemplo, una actividad solo puede ser de tipo taller, sustentación, examen, quiz o exposición.

**Las líneas** unen clases relacionadas, y los números dicen cuántos (1, 0..*, 1..*, 5..7), igual que en el modelo de dominio.

**El rombo negro** significa “es parte de”: la parte no tiene sentido sin el todo. Por ejemplo, los RA son parte de una asignatura.

**La línea punteada «uses»** indica que una clase usa una de las listas de opciones.

**Los tres recuadros grises** agrupan las clases por módulo e indican qué requisitos funcionales (RF) cubre cada uno.

**¿Qué significa cada clase?**

| En el diagrama | En español | Qué representa |
|---|---|---|
| `User` | Usuario | Cualquier persona con cuenta en el sistema. Tiene un rol (`RoleEnum`: administrador, docente o estudiante) y lleva la cuenta de intentos fallidos de ingreso. |
| `PasswordResetToken` | Token de recuperación | Código temporal para restablecer la contraseña. Tiene fecha de vencimiento y queda marcado cuando se usa. |
| `Subject` | Asignatura | Materia con código, nombre y programa académico. |
| `CourseGroup` | Grupo de curso | Grupo de una asignatura en un periodo académico, con su docente y sus estudiantes. |
| `GroupComment` | Comentario grupal | Mensaje del docente para todo el grupo. Se puede editar hasta una fecha límite. |
| `LearningOutcome` | Resultado de Aprendizaje (RA) | Lo que el estudiante debe lograr en la asignatura. Tiene un porcentaje de peso en la nota. |
| `EvaluationActivity` | Actividad evaluativa | Taller, examen, quiz, etc., asociado a un RA, con su objetivo, peso y fecha tentativa. |
| `ActivityGrade` | Nota de actividad | Calificación de un estudiante en una actividad, con fecha de registro y de última modificación. |
| `Observation` | Observación | Comentario del docente sobre una nota, clasificado en una categoría. |
| `ObservationCategory` | Categoría de observación | Tipo de observación, para poder clasificarlas. |
| `ImprovementPlan` | Plan de mejoramiento | Plan de recuperación de un estudiante en un RA. Guarda la nota original y la de recuperación. |
| `LearningOutcomeGrade` | Nota del RA | Nota calculada de un estudiante en un RA, con su nivel de desempeño (`PerformanceLevelEnum`: bajo, básico, alto o superior). Puede ser parcial, y el sistema puede determinar si ese RA requiere mejoramiento. |
| `SubjectFinalGrade` | Nota final de la asignatura | Nota definitiva del estudiante en la asignatura. |
| `CounterComment` | Contracomentario | Respuesta del estudiante a una observación del docente. |
| `ChangeHistory` | Historial de cambios | Registro de cada modificación: qué se cambió, el valor anterior, el nuevo, cuándo y quién lo hizo. |

**Reglas que se pueden ver en el diagrama:** cada asignatura tiene entre 5 y 7 RA; cada RA se evalúa con al menos una actividad; los RA y las actividades tienen un porcentaje de peso; la planeación de un RA se puede cerrar (`planningClosed`); y el usuario tiene un contador de intentos fallidos y una fecha de bloqueo (`failedAttempts`, `lockExpiration`) para proteger la cuenta.

</details>

<div class="salto"></div>

## 8. Diagrama de datos

Tablas, llaves y relaciones de la base de datos PostgreSQL.

| Herramienta | Abrir en línea |
|---|---|
| Lucidchart | [🔗 Abrir](https://lucid.app/lucidchart/0ec7915a-8f30-4555-9005-5867818cbc47/edit?viewport_loc=-4487%2C-4175%2C8981%2C5313%2C0_0&invitationId=inv_0c1f38e9-63cc-4f3a-871d-fe300479712f) |

<details>
<summary><b>🖼️ Ver diagrama</b></summary>

[![Diagrama de datos](img/modelo-datos-erd.png)](https://lucid.app/lucidchart/0ec7915a-8f30-4555-9005-5867818cbc47/edit?viewport_loc=-4487%2C-4175%2C8981%2C5313%2C0_0&invitationId=inv_0c1f38e9-63cc-4f3a-871d-fe300479712f)

</details>

<details>
<summary><b>💡 Ver explicación para el usuario</b></summary>

**¿Qué es este diagrama?** Muestra cómo se guarda la información de NotaRA en su base de datos (PostgreSQL). Si el modelo de dominio es el mapa de ideas, este diagrama es el archivador: indica en qué “cajón” (tabla) va cada dato y cómo se conectan los cajones entre sí.

**¿Cómo se lee?**

**Cada recuadro es una tabla**, parecida a una hoja de Excel. El nombre está arriba (por ejemplo, ESTUDIANTE) y cada fila de adentro es una columna de esa tabla, con su tipo de dato a la derecha.

**PK (llave primaria):** el número único que identifica cada registro, como la cédula de una persona. Por ejemplo, `id_estudiante`.

**FK (llave foránea):** un dato que apunta a un registro de otra tabla para conectarlos. Por ejemplo, en NOTA_ACTIVIDAD, `id_estudiante` indica a qué estudiante pertenece la nota.

**Tipos de dato:** int (número entero), decimal (número con decimales, como una nota de 4.5), string (texto), date (fecha), datetime (fecha y hora) y boolean (sí/no).

**Las líneas** conectan tablas relacionadas y llevan un verbo que se lee como frase, por ejemplo “ASIGNATURA define RESULTADO_APRENDIZAJE”.

**Los símbolos en los extremos de las líneas** dicen cuántos registros se relacionan: dos rayitas cortas significan “exactamente uno”, un círculo significa “puede no haber ninguno” y la “pata de gallo” (tres líneas que se abren) significa “muchos”. Por ejemplo, entre PERIODO_ACADEMICO y GRUPO se lee: un periodo contiene ninguno o muchos grupos, y cada grupo pertenece a exactamente un periodo.

**Las 20 tablas, agrupadas por tema:**

| Tema | Tablas | Qué guardan |
|---|---|---|
| Personas y acceso | USUARIO, ROL, ESTUDIANTE, DOCENTE | Los datos de la cuenta (nombre, correo institucional, documento, contraseña protegida), el rol de cada usuario y la información propia de cada perfil. Cada estudiante o docente está ligado a un único usuario. |
| Estructura académica | PERIODO_ACADEMICO, ASIGNATURA, GRUPO, MATRICULA, ASIGNACION_DOCENTE | Los periodos con su fecha de inicio y fin, las asignaturas con su código y créditos, los grupos de cada periodo, qué estudiante está inscrito en qué grupo y qué docente dicta qué asignatura en qué grupo. |
| Evaluación y notas | RESULTADO_APRENDIZAJE, ACTIVIDAD_EVALUATIVA, NOTA_ACTIVIDAD, EVALUACION_RA | Los RA de cada asignatura con su porcentaje, las actividades de cada RA con su porcentaje y fecha tentativa, la nota de cada estudiante en cada actividad y la nota calculada de cada RA con su nivel de desempeño. |
| Retroalimentación | OBSERVACION, CATEGORIA_OBSERVACION, COMENTARIO_GRUPAL, COMENTARIO_ESTUDIANTE | Las observaciones del docente (sobre una nota de actividad o sobre la nota de un RA) y sus categorías, los comentarios del docente a todo el grupo y las respuestas del estudiante a una observación. |
| Mejoramiento | PLAN_MEJORA | Los planes de recuperación: estudiante, RA, docente, nota antes y después, fechas y objetivos cumplidos. |
| Trazabilidad | HISTORIAL_CAMBIO, HISTORIAL_ACCESO | Qué se modificó (valor anterior y nuevo), quién y cuándo; y qué información consultó cada usuario y cuándo. |

**Ejemplo:** cuando un docente registra la nota de un taller, se guarda una fila en NOTA_ACTIVIDAD con la actividad (`id_actividad`) y el estudiante (`id_estudiante`). Con esas notas, el sistema calcula la nota del RA y la guarda en EVALUACION_RA junto con el nivel de desempeño. Si después el docente corrige la nota, el cambio queda en HISTORIAL_CAMBIO con el valor anterior y el nuevo.

**Sobre la seguridad:** la contraseña no se guarda tal cual. La columna `password_hash` guarda una versión transformada que no se puede leer ni revertir.

</details>

<div class="salto"></div>

## 9. Arquitectura

Arquetipo tecnológico y arquitectura de referencia del sistema.

| Herramienta | Abrir en línea |
|---|---|
| draw.io (Google Drive) | [🔗 Abrir](https://drive.google.com/file/d/1CU3wY1BDdpeHpXrfaBWgoIERtzfOtxaE/view?usp=sharing) |

<details>
<summary><b>🏗️ Arquetipo</b></summary>

[![Arquetipo](img/arquetipo.png)](https://drive.google.com/file/d/1CU3wY1BDdpeHpXrfaBWgoIERtzfOtxaE/view?usp=sharing)

</details>

<details>
<summary><b>🏗️ Arquitectura de referencia</b></summary>

[![Arquitectura de referencia](img/despliegue.png)](https://drive.google.com/file/d/1CU3wY1BDdpeHpXrfaBWgoIERtzfOtxaE/view?usp=sharing)

</details>

<details>
<summary><b>💡 Ver explicación para el usuario</b></summary>

**¿Qué muestran estos diagramas?** Cómo están organizadas las grandes piezas de NotaRA y cómo viaja la información desde que el usuario abre la página hasta que los datos quedan guardados. Son dos versiones del mismo plano:

**Arquitectura de referencia:** el plano general. Dice qué piezas hay y cómo se comunican, sin decir con qué tecnología se construyen.

**Arquetipo:** el mismo plano, pero indicando la tecnología concreta que se eligió para cada pieza.

**El recorrido, de izquierda a derecha:**

**Usuario final y computador:** la persona (administrador, docente o estudiante) entra a NotaRA desde el navegador de su computador.

**Internet (HTTPS):** la información viaja por internet cifrada, con la misma protección que indica el candado en la barra del navegador.

**Docker:** el recuadro grande que envuelve las piezas del sistema. Funciona como un conjunto de contenedores: cada pieza viaja empacada con todo lo que necesita, así funciona igual en cualquier servidor.

**NotaRA Frontend:** la parte visible del sistema: pantallas, botones y formularios. Es como la vitrina de un almacén.

**API REST:** el círculo entre el frontend y el backend. Es la ventanilla por donde las pantallas le hacen pedidos al sistema (“guarda esta nota”, “muéstrame mis resultados”) y reciben las respuestas.

**NotaRA Backend:** el cerebro del sistema. Revisa permisos, aplica las reglas académicas y calcula las notas.

**Database (TCP/IP):** el archivo donde se guarda toda la información. El backend se comunica con ella por una conexión interna (TCP/IP) a la que el usuario nunca accede directamente.

**Las tecnologías del arquetipo:**

| Pieza | Tecnología | En palabras sencillas |
|---|---|---|
| Todo el sistema | Docker | Empaqueta cada pieza para que funcione igual en cualquier servidor. |
| Frontend | Angular | Herramienta para construir páginas web interactivas. |
| Backend | Java 21 y Spring Boot 3.5.6 | Lenguaje de programación y marco de trabajo con los que se construye el servidor. |
| Backend | Security, JPA, Cache y Actuator | Módulos de apoyo para la seguridad (inicio de sesión y permisos), la conexión con la base de datos, una memoria rápida para no repetir consultas y el monitoreo del estado del sistema. |
| Base de datos | PostgreSQL | Sistema para guardar y consultar la información de forma organizada. |

**Ejemplo:** cuando un docente registra una nota, la pantalla (frontend) la envía por HTTPS a la API. El backend comprueba que el docente tiene permiso y que la nota está entre 0.0 y 5.0, y la guarda en la base de datos. Cuando el estudiante consulta sus resultados, la información hace el camino de regreso hasta su pantalla.

</details>

<div class="salto"></div>

## 10. Diagrama de componentes

Componente principal del backend y sus dependencias externas.

| Herramienta | Abrir en línea |
|---|---|
| draw.io (Google Drive) | [🔗 Abrir](https://drive.google.com/file/d/1sOntz-999fuHF_35kiQ096D-f_YSPLtw/view?usp=sharing) |

<details>
<summary><b>🖼️ Ver diagrama</b></summary>

[![Diagrama de componentes](img/componentes.png)](https://drive.google.com/file/d/1sOntz-999fuHF_35kiQ096D-f_YSPLtw/view?usp=sharing)

</details>

<details>
<summary><b>💡 Ver explicación para el usuario</b></summary>

**¿Qué es este diagrama?** Muestra de qué piezas está hecho el backend, el “cerebro” de NotaRA. Así como un carro se arma con piezas de distintos fabricantes, el backend combina una parte construida por el equipo con librerías externas ya probadas, que resuelven tareas comunes.

**¿Cómo se lee?**

**Caja rosada (Sistema Gestión RA Core):** el componente propio, programado por el equipo. Contiene la lógica de NotaRA.

**Cajas azules:** componentes externos, es decir, librerías y herramientas que el equipo no programó sino que utiliza. La leyenda de la esquina inferior derecha lo indica.

**Flechas punteadas:** significan “necesita” o “depende de”. Del componente rosado salen flechas hacia cada pieza externa que utiliza, y las piezas externas a su vez apuntan a Java 21, porque todas funcionan sobre él.

**¿Para qué sirve cada pieza externa?**

| Pieza | Para qué sirve |
|---|---|
| Java 21 (jdk) | La base: el lenguaje y el motor sobre el que funciona todo. |
| spring-boot-starter-parent 3.5.6 | El “kit base” que define versiones compatibles entre sí para las demás piezas. |
| spring-boot-starter-web | Permite recibir y responder las solicitudes que llegan desde las pantallas (la API). |
| springdoc-openapi | Genera automáticamente el manual de la API: qué servicios ofrece y cómo usarlos. |
| spring-boot-starter-security | Controla quién puede entrar y qué puede hacer cada rol. |
| spring-boot-starter-oauth2-resource-server | Verifica los “pases de acceso” (tokens) que presenta el usuario después de iniciar sesión. |
| spring-boot-starter-data-jpa | Traduce entre el código y la base de datos para guardar y leer la información. |
| postgresql-42.7.3.jar | El conector que permite hablar con la base de datos PostgreSQL. |
| spring-boot-starter-cache | Una memoria rápida para no repetir consultas que ya se hicieron. |
| spring-boot-starter-webflux | Permite manejar comunicaciones web sin quedarse esperando la respuesta (de forma asíncrona). |
| spring-boot-starter-actuator | Permite revisar la “salud” del sistema: si está encendido y funcionando bien. |
| mapstruct-1.5.5.Final | Copia automáticamente la información de un formato interno a otro, sin hacerlo a mano. |

**¿Por qué es importante?** Deja claro de qué depende el sistema para funcionar. Si una librería se actualiza o presenta un problema de seguridad, se sabe de inmediato qué parte del sistema se ve afectada.

</details>

<div class="salto"></div>

## 11. Diagrama de paquetes

Organización del código del backend en las capas domain, application e infrastructure.

| Herramienta | Abrir en línea |
|---|---|
| draw.io (Google Drive) | [🔗 Abrir](https://drive.google.com/file/d/1sOntz-999fuHF_35kiQ096D-f_YSPLtw/view?usp=sharing) |

<details>
<summary><b>🖼️ Ver diagrama</b></summary>

[![Diagrama de paquetes](img/paquetes-backend.png)](https://drive.google.com/file/d/1sOntz-999fuHF_35kiQ096D-f_YSPLtw/view?usp=sharing)

</details>

<details>
<summary><b>💡 Ver explicación para el usuario</b></summary>

**¿Qué es este diagrama?** Muestra cómo está organizado el código del backend en carpetas, llamadas paquetes. Así como una empresa se divide en departamentos, el código se divide en partes con responsabilidades distintas.

**¿Cómo se lee?**

**Las carpetas exteriores com → uco → sigra** son la “dirección” del proyecto dentro del código: uco identifica a la universidad y sigra es el nombre interno del proyecto. Todo lo demás vive dentro de sigra.

**Las flechas** significan “usa” o “depende de”. Van de afuera hacia adentro: infrastructure usa a application y a domain, y application usa a domain. El dominio no depende de nadie.

**Las tres capas:**

**domain (dominio): las reglas.** Es el corazón del sistema. Contiene los conceptos y reglas académicas, separados en los mismos módulos del modelo de dominio: usuario, académico, evaluación, mejora y trazabilidad, más shared (elementos compartidos). Cada módulo tiene un port (“puerto”), que funciona como un enchufe: dice qué necesita del exterior, por ejemplo “guardar una nota”, sin decir cómo se hace.

**application (aplicación): las acciones.** Coordina lo que el usuario pide. Sus carpetas command contienen las órdenes que se pueden ejecutar en cada módulo, como registrar o actualizar información.

**infrastructure (infraestructura): las conexiones con el exterior.** Aquí está la tecnología concreta. En web está lo que conversa con las pantallas: sus carpetas dto son los “formularios” con los que se envía y recibe la información, y exception maneja los errores. En persistence está lo que guarda y lee de la base de datos (entity, repository, converter y mapper). Además están security (seguridad y permisos), email (envío de correos), config (configuración general) y event (avisos que una parte del sistema le envía a otra).

**¿Por qué está organizado así?** Porque las reglas académicas quedan protegidas en el centro. Si mañana se cambia la base de datos o la forma de mostrar la información, solo se modifica infrastructure, sin tocar las reglas del dominio. Esto hace que NotaRA sea más fácil de mantener y de probar.

</details>
