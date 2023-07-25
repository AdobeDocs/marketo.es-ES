---
description: Preguntas frecuentes sobre la sincronización de cuentas de persona - Documentos de Marketo - Documentación del producto
title: Preguntas frecuentes sobre sincronización de cuenta de persona
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Preguntas frecuentes sobre sincronización de cuenta de persona {#person-account-sync-faq}

Marketo Engage sincroniza toda su base de datos con Veeva para el tipo de registros de cuenta de persona. Después de la sincronización, espera 5 minutos y, a continuación, se vuelve a sincronizar, todo el día, todos los días.

Las cuentas de persona se pueden configurar en Veeva para adaptarse a las necesidades de su organización.

>[!NOTE]
>
>Solo sincronizamos cuentas de nivel &quot;Professional&quot; como cuentas de persona.

**¿Qué es una cuenta de persona?**

Una cuenta de persona es muy similar al objeto de cuenta en Veeva CRM. Sin embargo, una cuenta de persona tiene acceso tanto a los campos de cuenta como a los de contacto.

**¿Qué sucede cuando se sincroniza una cuenta de persona con Marketo?**

Una cuenta de persona se sincroniza con Marketo como empresa y como persona.

>[!NOTE]
>
>Los campos personalizados de una cuenta de persona se copian tanto a la empresa como a la persona en Marketo.

**¿Cómo diferencio las cuentas de empresa y las cuentas de persona?**

Utilice el filtro de cuenta &quot;Es persona&quot; de la lista inteligente para separar las cuentas de persona de las cuentas empresariales estándar.

**¿Qué campo de correo electrónico debo usar para las cuentas de persona?**

Hay dos campos de correo electrónico para una cuenta de persona. Utilice el campo Dirección de correo electrónico de los formularios (no la dirección de correo electrónico de la persona) para garantizar que la anulación de duplicación de Marketo y otros procesos de correo electrónico funcionen correctamente.

## Dirección de sincronización {#sync-direction}

La sincronización de los campos relacionados con el contacto de la cuenta de persona es bidireccional. Si realiza cambios en un contacto en Veeva CRM o Marketo, las actualizaciones se reflejarán en ambos sistemas. Los campos de la cuenta solo se sincronizan en una dirección, de Veeva CRM a Marketo.

**¿Qué sucede si se realizan cambios en ambos sistemas a los campos Contacto en la Cuenta de persona al mismo tiempo?**

Estaríamos bien y dejaríamos que Veeva CRM ganara. Sin embargo, es raro que se produzca este tipo de colisión de datos.

**¿El tipo de registros de cliente potencial o contacto se sincroniza con Veeva CRM?**

Veeva CRM solo trata los objetos de cuenta de persona y también tiene cuentas de negocio. Los tipos tradicionales de CRM de Posible Cliente, Contactos y Oportunidades no están realmente en uso en los sistemas tradicionales de CRM de Veeva. Pueden crearse en Veeva CRM, pero no son compatibles oficialmente con este conector.

**¿Puedo convertir a una persona en un contacto en Marketo?**

No, ya que los tipos de posible cliente y contacto no son compatibles con la sincronización con Veeva CRM. Como resultado, no se admite la conversión.

**¿Puedo forzar manualmente una sincronización de un contacto?**

No, como el Contacto no es un tipo de registro independiente, no se admite la sincronización de una persona con Veeva.

**¿Se sincronizan todos y cada uno de los campos estándar con Marketo?**

No, no todos los campos estándar son útiles. Todos los campos personalizados pueden formar parte de la sincronización.

>[!NOTE]
>
>Marketo solo sincronizará los campos a los que el usuario de sincronización de Marketo tenga acceso.

**¿Marketo respetará las reglas de validación de Veeva?**

Sí, si hay un conflicto, registraremos el resultado en el registro de actividad del posible cliente.

>[!MORELIKETHIS]
>
>* [Asignación de campos Veeva predeterminada](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target="_blank"}
>* [Sincronización de mensajes de clave de llamada y llamada](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
