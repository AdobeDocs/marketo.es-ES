---
description: Suscripción a las notificaciones de estado del sistema - Documentos de Marketo Engage - Documentación del producto
title: Suscribirse a notificaciones de estado del sistema
feature: Getting Started
hide: true
hidefromtoc: true
source-git-commit: cf60167b9e9ee2ea2a2861a3cd3c661781dbf0b0
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# Suscribirse a las notificaciones de estado del sistema {#subscribe-to-system-status-notifications}

TEXTO DE INTRODUCCIÓN

>[!PREREQUISITES]
>
>Para poder crear una suscripción de, primero debe identificar en qué centro de datos y pod/servidor se encuentra su suscripción.

## Identificación del centro de datos {#identify}

+++Identificación del centro de datos y del pod/servidor

1. En la sección **Admin** de Marketo Engage, haga clic en **Mi cuenta**.

   ![](assets/subscribe-to-system-status-notifications-1.png)

1. Desplácese hacia abajo hasta _Información de soporte técnico_.

   ![](assets/subscribe-to-system-status-notifications-2.png)

En el campo _Centro de datos_, las letras son el centro de datos y los números son el pod. En el ejemplo anterior, el usuario se encuentra en nuestro centro de datos de Ashburn en el pod 49.

En el paso 7 de [creación de una suscripción](#create-a-subscription), este usuario seleccionaría la ubicación regional **Marketo Ashburn** y el pod **ab49**.

<table style="width:225px;">
  <tr>
    <th colspan="2">Abreviaciones del centro de datos</th>
  </tr>
  <tr>
    <td style="width:25%;">ab</td>
    <td>Asquemar</td>
  </tr>
  <tr>
    <td style="width:25%;">sj</td>
    <td>San Jose</td>
  </tr>
  <tr>
    <td style="width:25%;">sn</td>
    <td>Sídney</td>
  </tr>
  <tr>
    <td style="width:25%;">lon</td>
    <td>Londres</td>
  </tr>
  <tr>
    <td style="width:25%;">nld</td>
    <td>Ámsterdam</td>
  </tr>
</table>

>[!TIP]
>
>Este método también se puede utilizar para identificar en qué pod/servidor de Real Time Personalization (RTP) se encuentra su suscripción.

+++

## Creación de una suscripción {#create-a-subscription}

Después de [identificar su centro de datos y pod/servidor](#identify), siga los pasos a continuación para crear una suscripción.

1. En [status.adobe.com](https://status.adobe.com/es), haga clic en **Administrar suscripciones**.

   ![](assets/subscribe-to-system-status-notifications-3.png)

1. Inicia sesión (si aún no lo haces) con tus credenciales de Adobe o haz clic en **Crear una cuenta** si no la tienes.

   ![](assets/subscribe-to-system-status-notifications-4.png)

1. Manténgase en la ficha _Descripciones de productos_ y haga clic en **Crear suscripciones**.

   ![](assets/subscribe-to-system-status-notifications-5.png)

1. Haz clic en el icono de ![signo más](assets/icon-plus-sign.png) junto a _Experience Cloud_ para expandir el menú. Haz lo mismo para _Adobe Marketo Engage_.

   ![](assets/subscribe-to-system-status-notifications-6.png){width="800" zoomable="yes"}

1. Seleccione las ofertas o servicios de productos que desee y reciba las notificaciones correspondientes. A continuación, haga clic en **Continuar**.

   >[!TIP]
   >
   >Marque _Adobe Marketo Engage_ para seleccionar todo.

   ![](assets/subscribe-to-system-status-notifications-7.png){width="800" zoomable="yes"}

1. Seleccione los tipos de eventos que desee.

   ![](assets/subscribe-to-system-status-notifications-8.png)

   <table style="width:600px;">
   <tr>
   <td style="width:30%;"><b>Problema de servicio importante</b></td>
   <td>No disponibilidad del servicio o degradación grave del rendimiento para varios usuarios en sistemas de producción.</td>
   </tr>
   <tr>
   <td style="width:30%;"><b>Problema de servicio menor</b></td>
   <td>Falta de disponibilidad parcial del servicio o degradación moderada del rendimiento para varios usuarios en sistemas de producción.</td>
   </tr>
   <tr>
   <td style="width:30%;"><b>Mantenimiento de servicio</b></td>
   <td>Texto</td>
   </tr>
   <tr>
   <td style="width:30%;"><b>Anuncios</b></td>
   <td>Anuncios relacionados con...</td>
   </tr>
   </table>

1. Seleccione la ubicación y el entorno regionales que desee. Haga clic en **Continuar**.

   ![](assets/subscribe-to-system-status-notifications-9.png){width="800" zoomable="yes"}

1. Elige tu preferencia de suscripción, **Correo electrónico** o **Slack**, y haz clic en **Continuar**.

   ![](assets/subscribe-to-system-status-notifications-10.png)

1. Revisa tus selecciones y haz clic en **Confirmar preferencias**.

   ![](assets/subscribe-to-system-status-notifications-11.png)
