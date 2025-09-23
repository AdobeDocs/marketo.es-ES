---
unique-page-id: 14352477
description: 'Insertar en  [!DNL Sales Connect] : documentos de Marketo: documentación del producto'
title: Insertar en  [!DNL Sales Connect]
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '170'
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
   >[!DNL Sales Connect] agregará este grupo con el título &quot;SFDC-...&quot; a la página Relaciones en la [aplicación web](https://toutapp.com/login).

1. Seleccione **[!UICONTROL Enviar correo electrónico a todo el grupo]** para enviar este correo electrónico de grupo.
