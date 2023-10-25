---
unique-page-id: 10095307
description: Reglas de filtro de sincronización personalizadas para una dirección de correo electrónico - Documentos de Marketo - Documentación del producto
title: Reglas de filtro de sincronización personalizadas para una dirección de correo electrónico
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Reglas de filtro de sincronización personalizadas para una dirección de correo electrónico {#custom-sync-filter-rules-for-an-email-address}

Para evitar la sincronización de registros que no tienen una dirección de correo electrónico, siga estas reglas.

* Cuando se crea un posible cliente O cuando se actualiza el campo de la dirección de correo electrónico del posible cliente, compruebe si el posible cliente tiene una dirección de correo electrónico y, si la tiene, cambie Sincronizar a Mkto a **[!UICONTROL Verdadero]**. De lo contrario, cambie a **[!UICONTROL Falso]**.

* Cuando se crea un contacto O cuando se actualiza el campo de la dirección de correo electrónico del contacto, compruebe si el contacto tiene una dirección de correo electrónico y, si es así, cambie Sincronizar a Mkto a **[!UICONTROL Verdadero]** y cambiar Sincronizar a Mkto por **[!UICONTROL Verdadero]** en el registro de cuenta. De lo contrario, cambie a **[!UICONTROL Falso]**.

* Cuando se actualiza el campo Company Name (parentcustomerid) del contacto, compruebe si el campo Sync to Mkto del contacto es verdadero. Si es así, cambie Sincronizar a Mkto en la cuenta a **[!UICONTROL Verdadero]** también.

* Cuando se actualice el campo Cliente potencial (customerid) de la oportunidad o Contacto (parentcontactid), compruebe si el campo Sincronizar con Mkto de la cuenta es verdadero o si el campo Sincronizar con Mkto del contacto es verdadero. Si es así, cambie Sincronizar a Mkto si tiene la oportunidad de **[!UICONTROL Verdadero]** también.
