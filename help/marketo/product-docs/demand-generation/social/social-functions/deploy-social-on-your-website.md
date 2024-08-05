---
unique-page-id: 2950524
description: 'Implementar Social en el sitio web: Documentos de Marketo: documentación del producto'
title: Implementar Social en el sitio web
exl-id: bccfa461-29c1-4cf1-8e6a-2186c36bdf7e
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---

# Implementar Social en el sitio web {#deploy-social-on-your-website}

Incruste aplicaciones sociales en páginas que no sean de Marketo.

>[!IMPORTANT]
>
>El 31 de julio de 2024, empezamos el proceso de dejar de utilizar esta función. No va a poder crear nuevos recursos. Los recursos existentes seguirán funcionando hasta el 31 de enero de 2025. [Más información](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

>[!AVAILABILITY]
>
>No todos los usuarios de Marketo Engage han adquirido esta funcionalidad. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

Puede implementar aplicaciones sociales en su propio sitio web para atraer a su audiencia y llevar a todos a la conversación más amplia en las redes sociales. A medida que las personas comparten sus promociones y contenido con sus amigos en las redes sociales, genera más tráfico en el sitio.

1. Seleccione una aplicación social aprobada, como un vídeo de YouTube o un botón social.

   ![](assets/image2015-5-12-11-3a43-3a24.png)

1. Seleccione **Código incrustado** de las acciones de aplicaciones sociales.

   ![](assets/image2015-5-12-12-3a59-3a46.png)

1. Copie el código para el encabezado de página del sitio (`<head>`) y el cuerpo (`<body>`).

   ![](assets/image2015-5-12-13-3a3-3a34.png)

1. Pegue el primer fragmento de código en el encabezado de página del sitio web.

   ![](assets/socialonsite-embedhead.png)

1. Pegue el segundo fragmento de código en cada página, donde desee que aparezca la aplicación social en la página.

   ![](assets/socialonsite-embedwidget.png)

1. Si necesita establecer el tamaño de la aplicación social en dimensiones específicas de la página, agregue las opciones **outerHeight** y **outerWidth** al segundo fragmento de código. Por ejemplo, puede agregar `options='{"outerHeight":400, "outerWidth":600}'`, como en:

   ![](assets/socialonsite-resizewidget2.png)

   La aplicación social de Marketo ahora agrega contenido e interactividad al sitio web e invita a los seguidores, visitantes y clientes existentes a correr la voz sobre usted. Al mismo tiempo, agrega sus datos de perfil a la base de datos y realiza un seguimiento de las métricas de influencia social.

   >[!MORELIKETHIS]
   >
   >* [Personalizar botón de aplicación social](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)
   >* [Establecer requisito de uso compartido en redes sociales](/help/marketo/product-docs/demand-generation/social/social-functions/set-social-share-requirement.md)
   >* [Páginas de aterrizaje de Publish en Facebook](/help/marketo/product-docs/demand-generation/facebook/publish-landing-pages-to-facebook.md)
