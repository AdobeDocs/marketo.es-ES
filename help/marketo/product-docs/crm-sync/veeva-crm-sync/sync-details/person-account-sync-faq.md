---
description: Preguntas frecuentes sobre la sincronización de cuentas de persona - Documentos de Marketo - Documentación del producto
title: Preguntas frecuentes sobre la sincronización de cuentas de personas
exl-id: b77bb44f-94d0-40b2-9955-9636421ac468
source-git-commit: bb020cba0bb0cb65761e15cba05147b6e9fffe50
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Preguntas frecuentes sobre la sincronización de cuentas de personas {#person-account-sync-faq}

El Marketo Engage sincroniza toda la base de datos con Veva para el tipo de cuenta de persona de registros. Después de la sincronización espera 5 minutos y luego se sincroniza de nuevo, todo el día, todos los días.

Las cuentas de personas se pueden configurar en Veva para adaptarlas a las necesidades de su organización.

>[!NOTE]
>
>Solo sincronizamos cuentas de nivel &quot;profesional&quot; como cuentas de persona.

**¿Qué es una cuenta de persona?**

Una cuenta de persona es muy similar al objeto de cuenta en Veeva CRM. Sin embargo, una cuenta de persona tiene acceso a los campos de cuenta y a los campos de contacto.

**¿Qué sucede cuando se sincroniza una cuenta de persona con Marketo?**

Una cuenta de persona se sincroniza con Marketo como empresa y como persona.

>[!NOTE]
>
>Los campos personalizados de una cuenta de persona se copian tanto en la empresa como en la persona en Marketo.

**¿Cómo diferencio las cuentas de empresa y las cuentas de persona?**

Utilice el filtro Cuenta &quot;Es una persona&quot; de su lista inteligente para separar las cuentas de persona de las cuentas empresariales estándar.

**¿Qué campo de correo electrónico debo usar para las cuentas de persona?**

Hay dos campos de correo electrónico para una cuenta de persona. Utilice el campo Dirección de correo electrónico de los formularios (no la dirección de correo electrónico de la persona) para garantizar que la deduplicación de Marketo y el procesamiento de otros correos electrónicos funcionen correctamente.

## Dirección de sincronización {#sync-direction}

La sincronización de los campos relacionados con el contacto de la cuenta de persona es bidireccional. Si realiza cambios en un contacto en Veva CRM o Marketo, las actualizaciones se reflejarán en ambos sistemas. Los campos de la cuenta solo se sincronizan en una dirección, desde Veva CRM a Marketo.

**¿Qué sucede si se realizan cambios en ambos sistemas en los campos Contacto de la cuenta de persona al mismo tiempo?**

Estaríamos bien y dejaremos que Veeva CRM gane. Sin embargo, no es habitual que se produzca este tipo de conflicto de datos.

**¿El tipo de posible cliente o contacto de registros se sincroniza con Veeva CRM?**

Veeva CRM solo trata realmente con objetos de cuenta de persona y también tiene cuentas de negocio. Los tipos tradicionales de CRM de plomo, contactos y oportunidades no se utilizan realmente en los sistemas tradicionales de Veeva CRM. Pueden crearse en Veva CRM, pero no son compatibles oficialmente con este conector.

**¿Puedo convertir una persona en un contacto en Marketo?**

No, ya que Lead y Contact no son tipos compatibles con la sincronización con Veeva CRM. Como resultado, no se admite la conversión.

**¿Puedo forzar manualmente la sincronización de un contacto?**

No, ya que Contact no es un tipo de registro independiente, no se admite la sincronización de una persona con Veeva.

**¿Se sincroniza cada campo estándar con Marketo?**

No, no todos los campos estándar son útiles. Todos los campos personalizados pueden formar parte de la sincronización.

>[!NOTE]
>
>Marketo solo sincronizará los campos a los que el usuario de sincronización de Marketo tenga acceso.

**¿Marketo respetará las reglas de validación de Veva?**

Sí, si hay un conflicto, registraremos el resultado en el registro de actividades del posible cliente.

>[!MORELIKETHIS]
>
>* [Asignación de campos de veeva predeterminada](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping.md){target=&quot;_blank&quot;}
>* [Sincronización de mensajes clave de llamada y de llamada](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}

