---
unique-page-id: 10095307
description: Obtenga información sobre cómo configurar reglas de filtro de sincronización personalizadas para direcciones de correo electrónico en Dynamics. Utilice flujos de trabajo para establecer la sincronización con Mkto en función de si el posible cliente o el contacto tiene un correo electrónico.
title: Reglas de filtro de sincronización personalizado para una dirección de correo electrónico
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
TQID: https://experienceleague.adobe.com/SPEV9J4rabu7tMrPEOW8JYg2r7ihtTzE6OmJZvkOIZ4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 221
ht-degree: 7%

---

# Reglas de filtro de sincronización personalizado para una dirección de correo electrónico {#custom-sync-filter-rules-for-an-email-address}

Para evitar la sincronización de registros que no tienen una dirección de correo electrónico, siga estas reglas.

* Cuando se crea un posible cliente O cuando se actualiza el campo de la dirección de correo electrónico del posible cliente, comprueba si el posible cliente tiene una dirección de correo electrónico y, si es así, cambia Sincronizar a Mkto a **[!UICONTROL Verdadero]**. De lo contrario, cambie a **[!UICONTROL False]**

* Cuando se crea un contacto O cuando se actualiza el campo de la dirección de correo electrónico del contacto, comprueba si el contacto tiene una dirección de correo electrónico y, si es así, cambia Sincronizar a Mkto a **[!UICONTROL True]** y cambia Sincronizar a Mkto a **[!UICONTROL True]** en el registro de la cuenta. De lo contrario, cambie a **[!UICONTROL False]**

* Cuando se actualiza el campo Nombre de empresa (parentcustomerid) del contacto, compruebe si el campo Sincronizar con Mkto del contacto es verdadero. Si es así, cambie Sincronizar a Mkto en la cuenta a **[!UICONTROL True]** también
* Cuando se actualice el campo Cliente potencial (customerid) de la oportunidad o Contacto (parentcontactid), compruebe si el campo Sincronizar con Mkto de la cuenta es verdadero o si el campo Sincronizar con Mkto del contacto es verdadero. Si es así, cambie Sincronizar a Mkto en la oportunidad a **[!UICONTROL True]** también
