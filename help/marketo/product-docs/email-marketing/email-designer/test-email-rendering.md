---
solution: Marketo Engage
product: marketo
title: Prueba de representación de correo electrónico con Litmus
description: Aprenda a probar el procesamiento de correo electrónico en clientes con Litmus. Integre su cuenta de Litmus para previsualizar el contenido en varios clientes de correo electrónico.
level: Beginner, Intermediate
feature: Email Designer
exl-id: ccef36af-362a-4ac0-9030-492e9d7f10b5
TQID: https://experienceleague.adobe.com/HDelTp-9vepH8-TeDRN6FyAe-Nik-hfegvHrakdYDT4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 395
ht-degree: 3%

---

# Prueba de representación de correo electrónico con Litmus {#test-email-rendering-with-litmus}

Use su cuenta de [Litmus](https://www.litmus.com/email-testing) en Marketo Engage para ver al instante cómo se procesa su correo electrónico en los clientes de correo electrónico más populares.

>[!AVAILABILITY]
>
>Esta función está disponible para todos los usuarios de Marketo Engage que tengan una cuenta activa de Litmus.

## Usuarios de Litmus Enterprise {#litmus-enterprise}

Los siguientes pasos son para usuarios del [Plan Litmus Enterprise](https://www.litmus.com/pricing/enterprise){target="_blank"}.

1. En la pantalla _Editar contenido de correo electrónico_, haga clic en el botón **Simular contenido**.

   ![](assets/test-email-rendering-with-litmus-1.png)

1. Seleccione el destinatario de la prueba y haga clic en el botón **Procesar correo electrónico**.

   ![](assets/test-email-rendering-with-litmus-2.png){width="800" zoomable="yes"}

1. Si aún no lo ha hecho, **conecte su cuenta Litmus**. Si ya lo ha hecho, vaya al paso 6.

   ![](assets/test-email-rendering-with-litmus-3.png){width="800" zoomable="yes"}

1. Escriba sus credenciales de Litmus y haga clic en **Iniciar sesión**.

   >[!IMPORTANT]
   >
   >Al conectar su cuenta de Litmus a Marketo Engage, acepta que los correos electrónicos de prueba se envíen a Litmus. Después de enviar, Adobe ya no administra esos correos electrónicos de prueba. Como tal, la política de correo electrónico de retención de datos de Litmus se aplica a esos correos electrónicos, incluidos los datos de personalización que se pueden incluir en ellos.

1. Haga clic en **Conectar** para completar la integración.

   ![](assets/test-email-rendering-with-litmus-4.png)

1. Haga clic en el botón **Ejecutar prueba** para generar vistas previas de correo electrónico.

1. Consulte el aspecto del contenido en clientes de correo electrónico populares basados en web, móviles y equipos de escritorio. Haga clic en tantas miniaturas como desee previsualizar.

   ![](assets/test-email-rendering-with-litmus-5.png){width="800" zoomable="yes"}

   >[!NOTE]
   >
   >Aprenda a [personalizar la lista de clientes de correo electrónico predeterminada](https://help.litmus.com/article/227-change-your-default-email-clients-list).

1. Cuando termine de probar, haga clic en la flecha hacia atrás de la esquina superior izquierda para volver a la pantalla _Simular contenido_.

   ![](assets/test-email-rendering-with-litmus-6.png)

**PASO OPCIONAL**: si decide realizar cambios en su correo electrónico, después de hacer clic en **Procesar correo electrónico** para verlos, asegúrese de hacer clic también en el botón **Reintentar** en la parte superior derecha de la pantalla de Litmus _Vistas previas de correo electrónico_.

![](assets/test-email-rendering-with-litmus-7.png)

## Usuarios principales de Litmus {#litmus-core}

Los siguientes pasos son para usuarios del [Plan básico Litmus](https://www.litmus.com/pricing/){target="_blank"}.

1. En su cuenta de Litmus, recupere la dirección de correo electrónico de la prueba haciendo clic en el botón **Copiar dirección de la prueba** en la pantalla _Prueba_.

   ![](assets/test-email-rendering-with-litmus-8.png){width="800" zoomable="yes"}

1. En Marketo Engage, vaya a la pantalla _Editar contenido de correo electrónico_ del correo electrónico deseado y haga clic en el botón **Simular contenido**.

   ![](assets/test-email-rendering-with-litmus-9.png){width="600" zoomable="yes"}

1. Seleccione los destinatarios de la prueba y haga clic en el botón **Enviar prueba**.

   ![](assets/test-email-rendering-with-litmus-10.png){width="800" zoomable="yes"}

1. Escriba la dirección de correo electrónico de Litmus que copió en el paso 1 y haga clic en **Enviar prueba** de nuevo.

   ![](assets/test-email-rendering-with-litmus-11.png)

1. Revise el correo electrónico dentro de su cuenta de Litmus (en la carpeta correspondiente a la dirección de correo electrónico que copió de Litmus).

   ![](assets/test-email-rendering-with-litmus-12.png){width="800" zoomable="yes"}
