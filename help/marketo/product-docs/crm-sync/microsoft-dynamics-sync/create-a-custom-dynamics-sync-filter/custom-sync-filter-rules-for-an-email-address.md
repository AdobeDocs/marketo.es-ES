---
unique-page-id: 10095307
description: 'Reglas de filtro de sincronización personalizadas para una dirección de correo electrónico: Documentos de Marketo: Documentación del producto'
title: Reglas de filtro de sincronización personalizadas para una dirección de correo electrónico
exl-id: d1d51310-0c59-447c-818c-b25aa281c15c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# Reglas de filtro de sincronización personalizadas para una dirección de correo electrónico {#custom-sync-filter-rules-for-an-email-address}

Para evitar la sincronización de registros que no tengan una dirección de correo electrónico, siga estas reglas.

* Cuando se crea un posible cliente O cuando se actualiza el campo de dirección de correo electrónico del posible cliente, compruebe si el posible cliente tiene una dirección de correo electrónico y, en caso afirmativo, cambie Sincronizar a Mkto a **True**. De lo contrario, cambie a **False**

* Cuando se crea un contacto O cuando se actualiza el campo de dirección de correo electrónico del contacto, compruebe si el contacto tiene una dirección de correo electrónico y, en caso afirmativo, cambie Sincronizar a Mkto a **True** y cambie Sincronizar a Mkto a **True** en el registro de cuenta. De lo contrario, cambie a **False**

* Cuando se actualice el campo Nombre de la empresa (parentcustomerid) del contacto, compruebe si el campo Sincronizar con Mkto del contacto es verdadero. Si es así, cambie Sincronizar a Mkto en la cuenta a **True** también
* Cuando se actualice el campo Cliente potencial (customerid) de la oportunidad o Contacto (parentcontactid), compruebe si el campo Sincronizar con Mkto de la cuenta es verdadero o si el campo Sincronizar con Mkto del contacto es verdadero. Si es así, cambie Sincronizar a Mkto en la oportunidad a **True** también
