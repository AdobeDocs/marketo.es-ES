---
unique-page-id: 2359807
description: Personalizar estilos de sorteo - Documentos de Marketo - Documentación del producto
title: Personalizar estilos de sorteos
exl-id: 2b1437d9-a424-4d05-b614-7502c12e6ba2
source-git-commit: 2671f81f62658447e4b2a3dc2e02a4e0927443e8
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Personalizar estilos de sorteos {#customize-sweepstakes-styles}

Cuando usted [crear un sorteo](/help/marketo/product-docs/demand-generation/social/sweepstakes/create-sweepstakes.md), puede personalizar el aspecto de la página de aterrizaje.

>[!AVAILABILITY]
>
>No todos los usuarios de Marketo Engage han adquirido esta funcionalidad. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

1. Ir a **Actividades de marketing**.

![](assets/login-marketing-activities-1.png)

1. Seleccione el sorteo y haga clic en **Editar borrador**.

   ![](assets/image2014-9-25-17-3a51-3a45.png)

1. En el editor de Sorteos, vaya a **Configuración de aplicación** > **Aspecto**.

   ![](assets/image2014-9-25-17-3a51-3a59.png)

1. Edite el texto del botón de registro y el vínculo de progreso.

   ![](assets/image2014-9-25-17-3a52-3a22.png)

1. Para cada elemento que desee personalizar, introduzca sus propiedades CSS personalizadas.

   ![](assets/image2014-9-25-17-3a52-3a37.png)

   Ejemplo de CSS para **Botón Entrar**:
   `<pre>border: 5px solid #7B68EE; background-color: purple; padding: 10px; font: 16px; color: #FFFFFF; text-align: center;</pre>`

   Imagen de ejemplo para **Botón Entrar**:
   `<pre>background:url(https://app.marketo.com/images/public-site/button_sign-up-now.png) no-repeat center center; width:275px; height:95px; margin:auto; display:block;</pre>` `<pre>`

   >[!NOTE]
   >
   >Si utiliza una imagen con texto, recuerde quitar el texto del **Botón Entrar** en Texto, más arriba.

1. A medida que realiza cada cambio, el resultado se muestra en la vista previa Ver y editar.

   ![](assets/image2014-9-25-17-3a55-3a3.png)

   >[!NOTE]
   >
   >Pruebe el botón en varios exploradores diferentes, incluidas versiones anteriores.

   >[!MORELIKETHIS]
   >
   >El siguiente paso es añadir [inscríbete y envía correos electrónicos a tus sorteos](/help/marketo/product-docs/demand-generation/social/social-functions/use-emails-in-social-promotions.md).
