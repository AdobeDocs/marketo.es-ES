---
unique-page-id: 1900597
description: 'Definición de una audiencia mediante la importación de una lista: documentos de Marketo, documentación del producto'
title: Definir una audiencia mediante la importación de una lista
exl-id: 9a63f4a5-1d76-4671-9622-19eb368d196f
feature: Email Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 1%

---

# Definir una audiencia mediante la importación de una lista {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[Creación de un correo electrónico para un programa de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

Una vez que haya creado un programa de correo electrónico, querrá decirle a quién enviar el correo electrónico. Puede hacer esto por [creación de una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) o importando una lista. A continuación se indica cómo hacerlo importando una lista.

>[!NOTE]
>
>La definición de la audiencia solo funciona cuando el programa de correo electrónico no está aprobado.
>
>Los campos de fecha y hora que se importen se tratarán como Hora central. Si tiene campos de fecha y hora en una zona horaria diferente, puede utilizar una fórmula de Excel para transformarla a la hora central (América/Chicago).

1. Ir a **Actividades de marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Seleccione el programa de correo electrónico y, a continuación, haga clic en Importar lista en el mosaico Audiencia.

   ![](assets/importlist.png)

1. Se abrirá la ventana de importación de listas, haga clic en **Examinar** y seleccione el archivo que desea importar. Una vez seleccionada la lista de personas, haga clic en **Siguiente**.

   ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >Asegúrese de que la lista tenga la codificación UTF-8, UTF-16, Shift-JIS o EUC-JP y de que no supere los 50 MB de tamaño de archivo.

1. Compruebe que los campos del archivo estén asignados correctamente y haga clic en **Siguiente**.

   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo recordará las asignaciones para futuras importaciones.

1. Introduzca una **Nombre** para la lista y haga clic en **Importar**.

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. Una vez completada la importación, vuelva a la pestaña principal del programa. Verá cuántas personas cumplen los requisitos.

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**Definición**
>
>¿Te diste cuenta del número bloqueado? Este número es un subconjunto de las personas cualificadas y representa a las personas que no pueden recibir este correo electrónico porque:
>
>* Suscripción cancelada
>* Marketing suspendido
>* Está en la lista de bloqueos
>* Email no válido
>* Correo electrónico vacío
>
>Haga clic en el número para obtener una lista detallada de las personas bloqueadas de los envíos de correo.
>
>Utilice el ![—](assets/image2014-10-23-16-3a32-3a36-1.png) botón en el **Audiencia** mosaico para ver cuántas personas cumplen los requisitos para recibir el correo electrónico en función de los criterios de la lista inteligente. Reste el número Bloqueado del número Personas para obtener el número total de personas que recibirán el correo electrónico.

>[!TIP]
>
>No tiene que esperar a que finalice la importación de la lista. Puedes seguir trabajando si lo deseas.

¡Fantástico! Ahora es el momento de elegir un correo electrónico que ya existe o de crear uno nuevo para enviarlo a estas personas.

>[!MORELIKETHIS]
>
>* [Elegir un correo electrónico existente](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [Creación de un correo electrónico para un programa de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)
