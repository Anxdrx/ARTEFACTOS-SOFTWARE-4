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

