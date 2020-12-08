---
unique-page-id: 5472615
description: Explicación de los campos administrados por el sistema - Documentos de marketing - Documentación del producto
title: Explicación de los campos administrados por el sistema
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---


# Explicación de los campos administrados por el sistema {#understanding-system-managed-fields}

Es posible que haya notado que la página [de detalles de la](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) persona tiene una serie de campos no editables creados por Marketing. Estos datos provienen de varias fuentes y hay innumerables valores que podrían mostrarse.

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

## Tipos de campos {#field-types}

| **Nombre del campo** | **Definición** |
|---|---|
| Tipo de origen original | La ubicación en la que se descubrió por primera vez un visitante de persona o sitio web (ejemplo: Importación de listas, Visita a página Web) |
| Información de origen original | Detalles sobre esa ubicación (Ejemplo: Nombre de la lista, dirección URL de la página web) |
| Motor de búsqueda original | Si corresponde, el motor de búsqueda que dirigió a la persona a la fuente de entrada original |
| Frase de búsqueda original | Si corresponde, el término de búsqueda utilizado que dirigió a la persona a la fuente de entrada original |
| Remitente del reenvío original | Dirección URL que alojó el origen de entrada original |
| Tipo de origen de registro | La ubicación en la que una actividad se convirtió por primera vez en una persona (ejemplo: Importación de listas, Visita a página Web) |
| Información de origen de registro | Detalles sobre esa ubicación (Ejemplo: Nombre de la lista, dirección URL de la página web) |
| IP anónima | Indica la dirección IP de una persona |
| Compañía referida | La mejor conjetura del comerciante (basada en la IP) de la compañía de la persona |
| Ciudad afectada | La mejor conjetura del comerciante (basada en IP) de la ciudad de la persona |
| Región de estado indirecto | La mejor conjetura del comerciante (basada en la IP) del estado o región de la persona |
| Código postal adjunto | La mejor conjetura del comerciante (basada en la IP) del código postal de la persona |
| País afectado | La mejor conjetura del comerciante (basada en la IP) del país de la persona |
| Área metropolitana vinculada | La mejor conjetura del comerciante (basada en IP) del área metropolitana de la persona |
| Código de área telefónica inducida | La mejor conjetura del comerciante (basada en la IP) del código de área de la persona |

## Valores posibles para el tipo de origen original y de origen de registro {#possible-values-for-original-and-registration-source-type}

Debajo hay algunos valores posibles y lo que significan.

| **Tipo de origen original** | **Definición** |
|---|---|
| Salesforce.com | Se descubrió a una persona a partir de una sincronización de Salesforce |
| Visitas a páginas Web | Se descubrió a una persona en una página web |
| Archivo de formulario Web | Se descubrió a una persona después de rellenar un formulario |
| Importación de listas | Se descubrió a una persona a partir de una importación de listas |
| Nueva persona | La persona se introdujo manualmente en la base de datos |
| Clic en vínculo Web | Se descubrió a una persona después de hacer clic en un vínculo |
| Correo electrónico de ventas | Se envió un mensaje de correo electrónico a la persona mediante el Añada de correo electrónico de perspectiva de ventas |
| Persona | Persona que se ha sincronizado desde Salesforce como persona |
| Contacto | La persona se ha sincronizado desde Salesforce como contacto |
| API de Munchkin | La persona fue descubierta por la API Munchkin de Marketo |
| Aplicación social | Una persona fue descubierta por una utilidad social |
| API de servicio Web | Persona descubierta por una API de servicio Web |
| Socio de evento | Se descubrió a una persona a través de un servicio de seminario web sincronizado |
| Asociar posible cliente | Persona que se combinó mediante la llamada a la API de posible cliente asociada |

| **Tipo de origen de registro** | **Definición** |
|---|---|
| Importación de listas | Se convirtió en una persona a través de una importación de listas |
| Salesforce.com | Se convirtió en una persona a través de una sincronización de Salesforce |
| Archivo de formulario Web | Se convirtió en una persona después de rellenar un formulario |
| Correo electrónico de ventas | Se envió un mensaje de correo electrónico a la persona mediante el Añada de correo electrónico de perspectiva de ventas |
| API de servicio Web | Persona creada mediante la API SOAP/REST |
| Nueva persona | La persona se introdujo manualmente en la base de datos |
| API de Munchkin | Se convirtió en una persona a través de la API Munchkin de Marketo |
| Aplicación social | Se convirtió en una persona a través de una utilidad social |
| Socio de evento | Se convirtió en una persona a través de un servicio de seminario web vinculado |

