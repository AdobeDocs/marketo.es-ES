---
unique-page-id: 1900597
description: Definir una Audiencia importando una Lista - Documentos de marketing - Documentación del producto
title: Definir una Audiencia importando una Lista
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---


# Definir una Audiencia importando una Lista {#define-an-audience-by-importing-a-list}

>[!PREREQUISITES]
>
>[Creación de un correo electrónico para un Programa de correo electrónico](../../../../product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

Una vez que haya creado un programa de correo electrónico, querrá decirle a quién enviar el correo electrónico. Puede hacerlo [creando una lista inteligente](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) o importando una lista. Así se consigue importando una lista.

>[!NOTE]
>
>La definición de la audiencia solo funcionará cuando no se apruebe el programa de correo electrónico.
>
>Los campos de fecha y hora que se importan se tratan como Hora central. Si tiene campos de fecha y hora en un huso horario diferente, puede utilizar una fórmula de Excel para transformarla en hora central (América/Chicago).

1. Vaya a **Actividades de marketing**.

   ![](assets/login-marketing-activities-1.png)

   Seleccione el programa de correo electrónico y, a continuación, haga clic en Importar Lista en el mosaico de Audiencia.
   ![](assets/importlist.png)

1. Se abre la ventana de importación de listas, haga clic en **Examinar** y seleccione el archivo que desee importar. Una vez seleccionada la lista de personas, haga clic en Siguiente.
1. ![](assets/importlist1.png)

   >[!CAUTION]
   >
   >Asegúrese de que la lista está codificada como UTF-8, UTF-16, Shift-JIS o EUC-JP y no supera los 50 MB en tamaño de archivo.

   Compruebe que los campos del archivo estén correctamente asignados y haga clic en Siguiente.
   ![](assets/image2014-9-12-11-3a10-3a7.png)

   >[!TIP]
   >
   >Marketo recordará las asignaciones para futuras importaciones!

1. Escriba un **Nombre** para la lista y haga clic en **Importar**.

   ![](assets/image2014-9-12-11-3a10-3a13.png)

1. Una vez completada la importación, vuelva a la ficha programa principal. Verás cuántas personas calificarán.

   ![](assets/myemailprogram-1.jpg)

>[!NOTE]
>
>**Definición**
>
>¿Has notado el número Bloqueado? Este número es un subconjunto de personas cualificadas y representa a las personas a las que no se puede enviar este correo electrónico porque:
>
>* No suscrito
>* Comercialización suspendida
>* Incluido en la lista de bloqueados
>* Correo electrónico no válido
>* Correo electrónico vacío

>
>
Haga clic en el número para ver una lista detallada de las personas bloqueadas de los envíos de correo.
>
>Utilice el botón ![—](assets/image2014-10-23-16-3a32-3a36-1.png) del mosaico **Audiencia** para ver cuántas personas cumplen los requisitos para recibir el correo electrónico según los criterios de lista inteligente. Reste el número Bloqueado del número Personas para obtener el número total de personas que recibirán el correo electrónico.

>[!TIP]
>
>No tiene que esperar a que finalice la importación de listas. Puedes seguir trabajando si quieres.

¡Fantástico! Ahora es el momento de elegir un correo electrónico ya existente o de crear un nuevo correo electrónico para enviarlo a estas personas.

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Elegir un correo electrónico existente](../../../../product-docs/email-marketing/email-programs/email-program-actions/choose-an-existing-email.md)
>* [Creación de un correo electrónico para un Programa de correo electrónico](../../../../product-docs/email-marketing/email-programs/email-program-actions/create-an-email-for-an-email-program.md)

>



