---
unique-page-id: 14352508
description: Creación de campos dinámicos personalizados - Documentos de Marketo - Documentación del producto
title: Crear campos dinámicos personalizados
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Crear campos dinámicos personalizados {#create-custom-dynamic-fields}

Existen dos formas de crear campos dinámicos personalizados.

## Guardar campos personalizados para uno o varios contactos {#saving-custom-fields-for-one-or-a-few-contacts}

1. Haga clic en el nombre de un contacto en la página Personas.

1. Elija la lista desplegable junto a Cancelar suscripción y seleccione **Editar**.

1. Desplácese hacia abajo hasta la parte inferior de la página de edición. A continuación, puede crear un nombre y un valor para el campo.

1. Haga clic en **Guardar**.

## Guardar campos personalizados para muchos contactos {#saving-custom-fields-for-many-contacts}

1. Cree una hoja de cálculo CSV con los campos personalizados en su propia columna.

1. Siga las [proceso normal de carga de CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md), deteniendo en la pantalla de asignación de campos.

1. En lugar de uno de los campos preestablecidos, seleccione **Agregar un nuevo campo personalizado** en la lista desplegable .

1. Escriba el nombre del campo deseado y haga clic en **OK**.

1. Termine de cargar el CSV. Sus contactos aparecerán con el campo personalizado añadido.

>[!NOTE]
>
>Después de crear el campo personalizado, puede tardar unos 30 minutos en aparecer en la lista desplegable de campos dinámicos del editor de plantillas.

## Cómo usar los campos personalizados en una plantilla {#how-to-use-your-custom-fields-in-a-template}

Una vez que los campos personalizados se hayan almacenado utilizando los métodos anteriores, podrá hacer referencia a ellos en las plantillas.

1. [Creación de una plantilla](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md) y haga clic en el botón **Campos dinámicos** como lo haría normalmente.

1. Select **Campos personalizados** en la lista desplegable que aparece.

1. Verá los campos personalizados prealmacenados y podrá seleccionar uno para rellenarlo en la plantilla.
