---
unique-page-id: 6094890
description: 'Notas de la versión, febrero de 2015, Documentos de Marketo: documentación del producto'
title: Notas de la versión, febrero de 2015
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Notas de la versión: febrero de 2015 {#release-notes-february}

En la versión de febrero de 2015 se incluyen las siguientes funciones. Compruebe la disponibilidad de las funciones en Marketo Edition. Después del lanzamiento, asegúrese de volver para encontrar vínculos a artículos detallados para cada función. Rollo de tambor...

## Mejoras en la automatización de marketing {#marketing-automation-enhancements}

**[Mover campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

¡Alégrate! Ahora puede mover campañas inteligentes dentro y fuera de los programas mediante arrastrar y soltar o la función Mover del árbol.

**[[!DNL Dynamics] 2015 (En línea)](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)** - ¡Compatible!

**Cambios en el certificado HTTPS**

Para proteger la confidencialidad y la integridad de los datos de los clientes y los servicios SaaS, Marketo sigue las prácticas recomendadas del sector SaaS

y reemplazarán los protocolos de seguridad utilizados actualmente (SHA-1 y SSL) con versiones más seguras (SHA-2 (también conocido como SHA-256) y TLS) para los siguientes dominios:

* marketo.net (tráfico [!DNL Munchkin] cifrado)

* [marketo.com](https://marketo.com) (aplicaciones SaaS principales)

Esto sucederá poco después de esta versión. El protocolo SHA-1 se admitirá temporalmente en el dominio [mktoapi.com](https://mktoapi.com) hasta diciembre de 2015 para permitir que los propietarios de aplicaciones y sistemas heredados actualicen sus sistemas con compatibilidad con SHA-2.

**Proteger[!DNL Munchkin]**

Estamos eliminando nuestro soporte para SSL3. Hemos mantenido SSL3 hasta ahora para mantener la compatibilidad con navegadores web antiguos, pero en 2015 ya no vemos tráfico web significativo de esos navegadores. Esto solo afectaría a [!DNL Munchkin] cuando se utilice en páginas seguras y se implementará lentamente después de la versión de febrero.

## Mejoras de Real-Time Personalization {#real-time-personalization-enhancements}

**[URL de destino para campañas](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

Seleccione las páginas en las que desea que se muestre su campaña en tiempo real usando &quot;Añadir URL de Target&quot;. Esta función funciona con todos los tipos de campañas (diálogo, zona de entrada, widgets), pero es especialmente valiosa para las campañas de la zona de entrada en las que una campaña se renderiza en el ID de zona solo para la URL de destino seleccionada. Admite la adición de varias direcciones URL para dirigirse a diferentes páginas web.

![](assets/image2015-2-19-11-3a0-3a30.png)

Se agregó **país y estado a la segmentación basada en cuentas**

Ahora se pueden agregar el país y el estado a las listas de cuentas con nombre. Segmente a los posibles clientes de cuentas clave desde ubicaciones específicas.
