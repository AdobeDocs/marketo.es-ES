---
unique-page-id: 5472615
description: 'Explicación de los campos administrados por el sistema: documentos de Marketo: documentación del producto'
title: Explicación de los campos administrados por el sistema
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Explicación de los campos administrados por el sistema {#understanding-system-managed-fields}

Es posible que haya notado que la [página de detalles de la persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) tiene una serie de campos no editables creados por Marketo. Estos datos provienen de varias fuentes y hay innumerables valores que podrían mostrarse.

## Tipos de campo {#field-types}

| **Nombre del campo** | **Definición** |
|---|---|
| Tipo de origen original | Se descubrió por primera vez la ubicación de una persona o visitante del sitio web (Ejemplo: Importación de lista, Visita a página web) |
| Información del origen original | Detalles sobre esa ubicación (Ejemplo: Nombre de la lista, URL de la página web) |
| Motor de búsqueda original | Si corresponde, el motor de búsqueda que remitió a la persona a la fuente de entrada original |
| Frase de búsqueda original | Si corresponde, el término de búsqueda utilizado que remitió a la persona a la fuente de entrada original |
| Referente original | URL que alojaba el origen de la entrada original |
| Tipo de origen de registro | La ubicación en la que una actividad se convirtió por primera vez en una persona (ejemplo: Importación de lista, Visita a página web) |
| Información del origen de registro | Detalles sobre esa ubicación (Ejemplo: Nombre de la lista, URL de la página web) |
| IP anónima | Indica la dirección IP de una persona |
| Empresa vinculada | Mejor conjetura de Marketo (basada en la IP) de la empresa de la persona |
| Ciudad vinculada | Mejor conjetura de Marketo (basada en IP) de la ciudad de la persona |
| Región Estado Inferior | Mejor conjetura de Marketo (basada en la IP) del estado o región de la persona |
| Código postal adjunto | Mejor suposición de Marketo (basada en IP) del código postal de la persona |
| País afectado | Mejor conjetura de Marketo (basada en la IP) del país de la persona |
| Área metropolitana vinculada | Mejor conjetura de Marketo (basada en IP) del área metropolitana de la persona |
| Código de área de teléfono insertado | Mejor conjetura de Marketo (basada en IP) del código de área de la persona |

## Valores posibles del tipo de origen original y de registro {#possible-values-for-original-and-registration-source-type}

A continuación se muestran algunos valores posibles y lo que significan.

| **Tipo de origen original** | **Definición** |
|---|---|
| Salesforce.com | Se descubrió a una persona a partir de una sincronización de Salesforce |
| Visitas a páginas web | Se descubrió a una persona en una página web |
| Archivo de formulario web | Se descubrió a una persona después de rellenar un formulario |
| Importación de lista | Se descubrió a una persona de una importación de lista |
| Nueva persona | La persona se introdujo manualmente en la base de datos |
| Clic en vínculo web | Se descubrió a una persona después de hacer clic en un vínculo |
| Correo electrónico de ventas | Se envió un correo electrónico a la persona mediante el complemento de correo electrónico de perspectiva de ventas |
| Persona | La persona se ha sincronizado desde Salesforce como una persona |
| Contacto | La persona se sincronizó desde Salesforce como contacto |
| API de Munchkin | La API Munchkin de Marketo descubrió a una persona |
| Aplicación social | La persona fue descubierta por un widget social |
| API de servicio web | La persona ha sido descubierta por una API de servicio web |
| Socio de evento | Se descubrió a una persona a través de un servicio de seminarios web sincronizado |
| Asociar posible cliente | Persona que se fusionó mediante la llamada a la API de posible cliente asociada |

| **Tipo de origen de registro** | **Definición** |
|---|---|
| Importación de lista | Se ha convertido en una persona a través de una importación de lista |
| Salesforce.com | Se convirtió en una persona a través de una sincronización de Salesforce |
| Archivo de formulario web | Se convirtió en una persona después de rellenar un formulario |
| Correo electrónico de ventas | Se envió un correo electrónico a la persona mediante el complemento de correo electrónico de perspectiva de ventas |
| API de servicio web | La persona se creó mediante la API de SOAP/REST |
| Nueva persona | La persona se introdujo manualmente en la base de datos |
| API de Munchkin | Se convirtió en una persona a través de la API Munchkin de Marketo |
| Aplicación social | Se convirtió en una persona a través de un widget social |
| Socio de evento | Se convirtió en una persona a través de un servicio de seminarios web vinculado |
