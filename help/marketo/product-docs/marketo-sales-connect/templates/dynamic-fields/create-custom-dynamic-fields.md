---
unique-page-id: 14352508
description: Aprenda a crear campos dinámicos personalizados en plantillas de Sales Connect. Agregue campos de combinación que extraigan datos de contactos o usuarios en los correos electrónicos.
title: Crear campos dinámicos personalizados
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/uKq11AriHch77Qu0zRmjnJYAS4IZJP3UYOnyrnq0zi8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 256
ht-degree: 3%

---

# Crear campos dinámicos personalizados {#create-custom-dynamic-fields}

Existen dos formas de crear campos dinámicos personalizados.

## Guardar campos personalizados para uno o varios contactos {#saving-custom-fields-for-one-or-a-few-contacts}

1. Haga clic en el nombre de un contacto en la página [!UICONTROL Personas].

1. Elige la lista desplegable junto a [!UICONTROL Cancelar la suscripción] y selecciona **[!UICONTROL Editar]**.

1. Desplácese hacia abajo hasta la parte inferior de la página de edición. A continuación, puede crear un nombre y un valor para el campo.

1. Haga clic en **[!UICONTROL Guardar]**.

## Guardar campos personalizados para muchos contactos {#saving-custom-fields-for-many-contacts}

1. Cree una hoja de cálculo CSV con los campos personalizados en su propia columna.

1. Siga el [proceso normal de carga de CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md), deteniéndose en la pantalla de asignación de campos.

1. En lugar de uno de los campos preestablecidos, elija **[!UICONTROL Agregar nuevo campo personalizado]** en la lista desplegable.

1. Escriba el nombre de campo que desee y haga clic en **[!UICONTROL Aceptar]**.

1. Termine de cargar el CSV. Los contactos se completarán con el campo personalizado agregado.

>[!NOTE]
>
>Una vez creado el campo personalizado, puede tardar unos 30 minutos en aparecer en la lista desplegable de campo dinámico del editor de plantillas.

## Cómo utilizar los campos personalizados en una plantilla {#how-to-use-your-custom-fields-in-a-template}

Una vez almacenados los campos personalizados con los métodos anteriores, podrá hacer referencia a ellos en las plantillas.

1. [Cree una plantilla](/help/marketo/product-docs/marketo-sales-connect/templates/manage-templates.md#create-a-template) y haga clic en el botón **[!UICONTROL Campos dinámicos]** como lo haría normalmente.

1. Seleccione **[!UICONTROL Campos personalizados]** de la lista desplegable que aparece.

1. Verá sus campos personalizados prealmacenados y podrá seleccionar uno para rellenar en la plantilla.
