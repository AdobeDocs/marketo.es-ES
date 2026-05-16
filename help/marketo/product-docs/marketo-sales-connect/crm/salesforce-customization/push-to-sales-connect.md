---
unique-page-id: 14352477
description: Aprenda a utilizar el botón Insertar en Sales Connect de Salesforce. Añadir posibles clientes o contactos de Salesforce a Sales Connect con un solo clic.
title: Insertar en  [!DNL Sales Connect]
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/piy3bPtiO48FQhWEmpu5qo4denlJ8v1ZU-VXBlWh0Mg
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 190
ht-degree: 0%

---

# Insertar en [!DNL Sales Connect] {#push-to-sales-connect}

Nuestro botón [!UICONTROL Insertar en la salida] tomará una lista de tus posibles clientes/contactos en [!DNL Salesforce] y los insertará en un grupo en [!DNL Sales Connect]. A continuación, puede enviar rápidamente un correo electrónico de grupo personalizable con seguimiento de Tout adjunto.

## Requisitos {#requirements}

* Paquete [!DNL Sales Connect Salesforce] instalado por el administrador [!DNL Salesforce]

* [!UICONTROL Botón Insertar en conexión de ventas] instalado en la vista de lista por el administrador de [!DNL Salesforce]

* [!DNL Salesforce] conexión realizada con [!DNL Sales Connect] para el usuario que realiza la notificación push

## Cómo. {#how-to}

1. Haga clic en la ficha **[!UICONTROL Posible cliente/Contacto]** de [!DNL Salesforce].
1. Cambie a la vista de lista que desee insertar en [!DNL Sales Connect] junto al botón [!UICONTROL Ir].
1. Haga clic en **[!UICONTROL Ir]**.
1. Seleccione todos los posibles clientes o contactos a los que desee enviar un mensaje de exclusión.
1. Seleccione **[!UICONTROL Insertar en MSE]**.
1. Aparecerá una nueva ventana que verifica el número de posibles clientes/contactos que desea insertar. Seleccione **[!UICONTROL Continuar con el grupo]**.[!DNL Sales Connect] no insertará ningún contacto marcado como [!UICONTROL exclusión de correo electrónico] en [!DNL Salesforce] o [!UICONTROL canceló la suscripción] en [!DNL Sales Connect].

   >[!NOTE]
   >
   >[!DNL Sales Connect] agregará este grupo titulado &quot;SFDC-...&quot; a la página Relaciones en la [aplicación web](https://toutapp.com/login).

1. Seleccione **[!UICONTROL Enviar correo electrónico a todo el grupo]** para enviar este correo electrónico de grupo.
