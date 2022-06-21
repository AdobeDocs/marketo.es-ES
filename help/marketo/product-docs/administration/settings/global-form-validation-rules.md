---
description: Reglas de validación de formularios globales - Documentos de Marketo - Documentación del producto
title: Reglas globales de validación de formularios
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
source-git-commit: 7749bd1fec7a7c1974efdb8de046eed4f34aefc4
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Reglas globales de validación de formularios {#global-form-validation-rules}

Esta función permite bloquear dominios específicos para que no se envíen a formularios de Marketo Engage.

## Cómo habilitar el acceso {#how-to-enable-access}

Para poder utilizar esta función, debe habilitar su permiso según la función que desee.

1. En Marketo, haga clic en **Administrador**.

   ![](assets/global-form-validation-rules-1.png)

1. Haga clic en **Usuarios y funciones**.

   ![](assets/global-form-validation-rules-2.png)

1. Haga clic en el **Funciones** pestaña .

   ![](assets/global-form-validation-rules-3.png)

1. Haga doble clic en la función a la que desee conceder permisos.

   ![](assets/global-form-validation-rules-4.png)

1. Haga clic en el **+** junto a Administración de acceso.

   ![](assets/global-form-validation-rules-5.png)

1. Desplácese hacia abajo y seleccione **Acceso a las reglas de validación del formulario** y haga clic en **Guardar**.

   ![](assets/global-form-validation-rules-6.png)

## Crear nueva regla de validación de formulario {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Estas reglas se aplicarán a todos los formularios de las suscripciones al Marketo Engage.

1. En Marketo, haga clic en **Administrador**.

   ![](assets/global-form-validation-rules-7.png)

1. Haga clic en **Regla de validación del formulario global**.

   ![](assets/global-form-validation-rules-8.png)

1. Haga clic en **Nueva regla de validación de formulario**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >La lista desplegable Acciones de regla de validación de formulario permite eliminar o editar las reglas existentes.

1. Asigne un nombre a la regla, asígnele una descripción opcional e introduzca el mensaje de error que desea que vean los visitantes del formulario. Introduzca los dominios que desea bloquear en el cuadro de reglas, seleccione **Activar regla** y haga clic en **Crear**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage tiene una lista de bloqueados definida de dominios de correo electrónico de consumidor gratuitos que se bloquean al utilizar nuestra regla de &quot;Lista de bloqueados de dominio de correo electrónico de consumidor&quot; precargada. [Ver la lista aquí](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv).

## Deshabilitar el acceso por formulario{#how-to-disable-access-per-form}

Una vez activada, las reglas se aplican a todos los formularios. Sin embargo, si tiene un formulario con requisitos específicos y no desea que se rechace nada, puede desactivar las reglas de validación del formulario global en la configuración de un formulario.

1. En el formulario que desee, haga clic en **Configuración de formulario**, luego **Configuración**.

   ![](assets/global-form-validation-rules-11.png)

1. Haga clic en la lista desplegable Reglas de validación de formulario globales y seleccione **Desactivado**.

   ![](assets/global-form-validation-rules-12.png)

Cuando apruebe y publique el formulario, ignorará las reglas de validación del formulario global.
