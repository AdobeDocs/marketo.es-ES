---
unique-page-id: 1900597
description: 'Definir una audiencia mediante la importación de una lista: Documentos de Marketo: Documentación del producto'
title: Definir una audiencia mediante la importación de una lista
exl-id: 9a63f4a5-1d76-4671-9622-19eb368d196f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 1%

---

# Definir una audiencia mediante la importación de una lista {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[Creación de un correo electrónico para un programa de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

Una vez que haya creado un programa de correo electrónico, querrá decirle a quién enviar el correo electrónico. Puede hacerlo de [creación de una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) o importando una lista. Así se consigue importando una lista.

>[!NOTE]
>
>La definición de la audiencia solo funcionará cuando el programa de correo electrónico no se apruebe.
>
>Cualquier campo de fecha y hora que se importe se tratará como Hora central. Si tiene campos de fecha y hora en un huso horario diferente, puede utilizar una fórmula de Excel para transformarla a la hora central (América/Chicago).

1. Vaya a **Actividades de marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Seleccione su programa de correo electrónico y, a continuación, haga clic en Importar lista en el mosaico Audiencia .

   ![](assets/importlist.png)

1. Se abrirá la ventana de importación de lista, haga clic en **Examinar** y seleccione el archivo que desea importar. Una vez que haya seleccionado la lista de personas, haga clic en **Siguiente**.

   ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >Asegúrese de que la lista esté codificada con UTF-8, UTF-16, Shift-JIS o EUC-JP, y que no supere los 50 MB de tamaño de archivo.

1. Compruebe que los campos del archivo estén asignados correctamente y haga clic en **Siguiente**.

   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo recordará las asignaciones para futuras importaciones.

1. Escriba un **Nombre** para la lista y haga clic en **Importar**.

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. Una vez completada la importación, vuelva a la pestaña principal del programa. Verá cuántas personas calificarán.

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**Definición**
>
>¿Viste el número bloqueado? Este número es un subconjunto de personas cualificadas y representa a las personas a las que no se puede enviar este correo electrónico porque:
>
>* Suscripción cancelada
>* Marketing suspendido
>* Está en la lista de bloqueos
>* Email no válido
>* Correo electrónico vacío
>
>Haga clic en el número para obtener una lista detallada de las personas bloqueadas del correo.
>
>Utilice la variable ![—](assets/image2014-10-23-16-3a32-3a36-1.png) en el **Audiencia** para ver cuántas personas cumplen los requisitos para recibir el correo electrónico según los criterios de la lista inteligente. Reste el número bloqueado del número Personas para obtener el número total de personas que recibirán el correo electrónico.

>[!TIP]
>
>No es necesario esperar a que finalice la importación de la lista. Puedes seguir trabajando si quieres.

¡Fantástico! Ahora es el momento de elegir un correo electrónico ya existente o crear un nuevo correo electrónico para enviarlo a estas personas.

>[!MORELIKETHIS]
>
>* [Elegir un correo electrónico existente](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [Creación de un correo electrónico para un programa de correo electrónico](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

