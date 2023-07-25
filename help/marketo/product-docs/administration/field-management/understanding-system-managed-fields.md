---
unique-page-id: 5472615
description: Explicación de los campos administrados por el sistema - Documentos de Marketo - Documentación del producto
title: Explicación de los campos administrados por el sistema
exl-id: 4a58d41f-c2f5-4bcc-93ef-10a31e5475fd
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 15%

---

# Explicación de los campos administrados por el sistema {#understanding-system-managed-fields}

Es posible que haya notado que la [página de detalles de persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"} tiene una serie de campos no editables creados por Marketo. Estos datos provienen de varias fuentes y hay infinidad de valores que podrían mostrarse.

## Tipos de campo {#field-types}

| **Nombre del campo** | **Definición** |
|---|---|
| Tipo de origen original | La ubicación en la que se descubrió por primera vez una persona o visitante de un sitio web (Ejemplo: importación de lista, visita de página web) |
| Información de origen original | Detalles específicos sobre esa ubicación (Ejemplo: Nombre de la lista, URL de la página web) |
| Motor de búsqueda original | Si procede, el motor de búsqueda que refirió a la persona a la fuente de entrada original |
| Frase de búsqueda original | Si procede, el término de búsqueda utilizado que refirió a la persona a la fuente de entrada original |
| Referente original | URL que alojó el origen de entrada original |
| Tipo de origen del registro | La ubicación de una actividad se convirtió en una persona por primera vez (Ejemplo: importación de lista, visita de página web) |
| Información de origen del registro | Detalles específicos sobre esa ubicación (Ejemplo: Nombre de la lista, URL de la página web) |
| IP anónima | Indica la dirección IP de una persona |
| Compañía inferida | Mejor estimación de Marketo (basada en la dirección IP) de la compañía de la persona |
| Ciudad inferida | Mejor estimación de Marketo (basada en la dirección IP) de la ciudad de la persona |
| Región del estado inferida | Mejor estimación de Marketo (basada en la dirección IP) del estado o la región de la persona |
| Código postal inferido | Mejor estimación de Marketo (basada en la dirección IP) del código postal de la persona |
| País inferido | Mejor estimación de Marketo (basada en la dirección IP) del país de la persona |
| Área metropolitana inferida | Mejor estimación de Marketo (basada en la dirección IP) del área metropolitana de la persona |
| Código de área telefónico inferido | Mejor estimación de Marketo (basada en la dirección IP) del código de área de la persona |

## Valores posibles para el tipo de origen original y de registro {#possible-values-for-original-and-registration-source-type}

A continuación se muestran algunos valores posibles y lo que significan.

| **Tipo de origen original** | **Definición** |
|---|---|
| Salesforce.com | La persona se ha descubierto a partir de un [!DNL Webhook] sincronizar |
| Visitas a páginas web | La persona se ha descubierto desde una página web |
| Rellenado de formulario web | La persona se descubrió después de rellenar un formulario |
| Lista de importación | Se descubrió una persona a partir de una importación de lista |
| Nueva persona | La persona se ha introducido manualmente en la base de datos |
| Clic en vínculo web | Se descubrió una persona después de hacer clic en un vínculo |
| Correo electrónico de ventas | Se envió a la persona por correo electrónico mediante [!DNL Sales Insight] Complemento de correo electrónico |
| Persona | La persona se ha sincronizado desde [!DNL Salesforce] como persona |
| Contacto | La persona se ha sincronizado desde [!DNL Webhook] como contacto |
| [!DNL Munchkin] API | El Marketo Engage descubrió la persona [!DNL Munchkin] API |
| Aplicación social | La persona fue descubierta por un widget social |
| Servicio Web API | Una API de servicio web descubrió la persona |
| Socio del evento | La persona se ha descubierto mediante un servicio de seminario web sincronizado |
| Asociar posible cliente | Persona que se fusionó mediante la llamada a la API de Associate Lead |

| **Tipo de origen del registro** | **Definición** |
|---|---|
| Lista de importación | Se convirtió en una persona a través de una importación de lista |
| Salesforce.com | Se convirtió en una persona a través de un [!DNL Webhook] sincronizar |
| Rellenado de formulario web | Se convierte en persona después de rellenar un formulario |
| Correo electrónico de ventas | Se envió a la persona por correo electrónico mediante [!DNL Webhook] Complemento de correo electrónico |
| Servicio Web API | La persona se ha creado mediante la API de SOAP/REST |
| Nueva persona | La persona se ha introducido manualmente en la base de datos |
| [!DNL Munchkin] API | Marketo Hágase persona a través del [!DNL Munchkin] API |
| Aplicación social | Convertirse en una persona a través de un widget social |
| Socio del evento | Convertirse en persona mediante un servicio de seminario web vinculado |
