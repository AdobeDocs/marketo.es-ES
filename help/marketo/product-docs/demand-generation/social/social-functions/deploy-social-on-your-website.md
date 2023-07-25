---
unique-page-id: 2950524
description: 'Implementar Social en el sitio web: Documentos de Marketo: documentación del producto'
title: Implementar Social en el sitio web
exl-id: bccfa461-29c1-4cf1-8e6a-2186c36bdf7e
feature: Social
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# Implementar Social en el sitio web {#deploy-social-on-your-website}

Incruste aplicaciones sociales en páginas que no sean de Marketo.

>[!AVAILABILITY]
>
>Póngase en contacto con su representante de ventas para obtener más información.

Puede implementar aplicaciones sociales en su propio sitio web para atraer a su audiencia y llevar a todos a la conversación más amplia en las redes sociales. A medida que las personas comparten sus promociones y contenido con sus amigos en las redes sociales, genera más tráfico en el sitio.

1. Seleccione una aplicación social aprobada, como un vídeo de YouTube o un botón social.

   ![](assets/image2015-5-12-11-3a43-3a24.png)

1. Seleccionar **Código incrustado** en Acciones de aplicación social.

   ![](assets/image2015-5-12-12-3a59-3a46.png)

1. Copie el código del encabezado de página del sitio (`<head>`) y cuerpo (`<body>`).

   ![](assets/image2015-5-12-13-3a3-3a34.png)

1. Pegue el primer fragmento de código en el encabezado de página del sitio web.

   ![](assets/socialonsite-embedhead.png)

1. Pegue el segundo fragmento de código en cada página, donde desee que aparezca la aplicación social en la página.

   ![](assets/socialonsite-embedwidget.png)

1. Si necesita establecer el tamaño de la aplicación social en dimensiones específicas de la página, agregue la variable **outerHeight** y **outerWidth** al segundo fragmento de código. Por ejemplo, puede agregar lo siguiente `options='{"outerHeight":400, "outerWidth":600}'`, como en:

   ![](assets/socialonsite-resizewidget2.png)

   La aplicación social de Marketo ahora agrega contenido e interactividad al sitio web e invita a los seguidores, visitantes y clientes existentes a correr la voz sobre usted. Al mismo tiempo, agrega sus datos de perfil a la base de datos y realiza un seguimiento de las métricas de influencia social.

   >[!MORELIKETHIS]
   >
   >* [Botón Personalizar aplicación social](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)
   >* [Establecer requisito de uso compartido social](/help/marketo/product-docs/demand-generation/social/social-functions/set-social-share-requirement.md)
   >* [Publicación de páginas de aterrizaje en Facebook](/help/marketo/product-docs/demand-generation/facebook/publish-landing-pages-to-facebook.md)
