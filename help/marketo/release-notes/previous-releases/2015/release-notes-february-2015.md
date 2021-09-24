---
unique-page-id: 6094890
description: 'Notas de la versión, febrero de 2015: Documentación del producto de Marketo'
title: Notas de la versión, febrero de 2015
exl-id: a7ce88dc-a4d2-4ccb-9fe5-61130334d24d
source-git-commit: 74effe9f8078f8d71e6de01d6e737ddc86978abb
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# Notas de la versión: Febrero de 2015 {#release-notes-february}

La versión de febrero de 2015 incluye las siguientes funciones. Compruebe la disponibilidad de las funciones en Marketo Edition. Después de la versión, asegúrese de volver para encontrar vínculos a artículos detallados para cada función. Rodaje de tambor...

## Mejoras en la automatización de marketing {#marketing-automation-enhancements}

**[Mover la campaña inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/move-a-smart-campaign.md)**

¡Regocijaos! Ahora puede mover campañas inteligentes dentro y fuera de programas mediante arrastrar y soltar o la función Mover del árbol.

**[Dynamics 2015 (Online)](https://docs.marketo.com/display/docs/microsoft+dynamics+2013+on-premises)** : compatible

**Cambios en los certificados HTTPS**

Para proteger la confidencialidad y la integridad de los datos de los clientes y los servicios SaaS, Marketo sigue las prácticas recomendadas del sector SaaS

y reemplazarán los protocolos de seguridad utilizados actualmente (SHA-1 y SSL) con versiones más seguras (SHA-2 (también conocidos como SHA-256) y TLS) para los siguientes dominios:

* [marketing.net](https://marketo.net)  (tráfico de Munchkin cifrado)

* [marketo.com](https://marketo.com)  (aplicaciones SaaS principales)

Esto sucederá poco después de esta versión. El protocolo SHA-1 se admitirá temporalmente en el dominio [mktoapi.com](https://mktoapi.com) hasta diciembre de 2015 para permitir a los propietarios de sistemas y aplicaciones heredados actualizar sus sistemas con compatibilidad con SHA-2.

**Secure Munchkin**

Eliminamos nuestra compatibilidad con SSL3. Hasta ahora hemos mantenido SSL3 para mantener la compatibilidad con exploradores web antiguos, pero en 2015 ya no vemos tráfico web significativo de esos exploradores. Esto solo afectaría a Munchkin cuando se usa en páginas seguras, y se desplegará lentamente después de la versión de febrero.

## Mejoras en la personalización en tiempo real {#real-time-personalization-enhancements}

**[Dirección URL de destino de campañas](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/adding-a-target-url-to-a-web-campaign.md)**

Seleccione las páginas en las que desea que su campaña en tiempo real se muestre al usar &quot;Agregar una dirección URL de destino&quot;. Esta función funciona con todos los tipos de campaña (Dialogue, In Zone, Widgets), pero es especialmente valiosa para las campañas In Zone en las que una campaña se renderiza en el ID de zona solo para la URL de destino seleccionada. Admite la adición de varias direcciones URL para dirigirse a diferentes páginas web.

![](assets/image2015-2-19-11-3a0-3a30.png)

**País y estado agregados a la segmentación basada en cuentas**

Ahora se puede agregar País y Estado a las Listas de cuentas con nombre. Segmente los posibles clientes de cuentas clave de ubicaciones específicas.
