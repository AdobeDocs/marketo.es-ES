---
description: Cómo habilitar el permiso Reglas de validación de formularios de Access y crear reglas globales para bloquear el envío de dominios específicos a formularios de Marketo Engage.
title: Reglas de formulario de validación global
exl-id: a44db893-00b5-40d2-8be3-41d52b2fd7b5
feature: Administration
source-git-commit: c06481152e88b8760a4539842a91aea90ab07fa1
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 2%

---

# Reglas de formulario de validación global {#global-form-validation-rules}

Esta función le permite bloquear dominios específicos para que no se envíen a formularios Marketo Engage.

## Cómo activar el acceso {#how-to-enable-access}

Para poder utilizar esta función, debe habilitar su permiso para cada función deseada.

1. En Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/global-form-validation-rules-1.png)

1. Haga clic en **[!UICONTROL Usuarios y funciones]**.

   ![](assets/global-form-validation-rules-2.png)

1. Haga clic en la ficha **[!UICONTROL Roles]**.

   ![](assets/global-form-validation-rules-3.png)

1. Haga doble clic en la función a la que desee conceder permisos.

   ![](assets/global-form-validation-rules-4.png)

1. Haga clic en el signo **+** junto a **Administrador de acceso**.

   ![](assets/global-form-validation-rules-5.png)

1. Desplácese hacia abajo y seleccione **[!UICONTROL Reglas de validación de formularios de acceso]** y haga clic en **[!UICONTROL Guardar]**.

   ![](assets/global-form-validation-rules-6.png)

## Crear nueva regla de validación de formulario {#create-new-form-validation-rule}

>[!IMPORTANT]
>
>Estas reglas se aplicarán a todos los formularios de las suscripciones de Marketo Engage.

1. En Marketo, haga clic en **[!UICONTROL Administrador]**.

   ![](assets/global-form-validation-rules-7.png)

1. Haga clic en **[!UICONTROL Regla de validación de formulario global]**.

   ![](assets/global-form-validation-rules-8.png)

1. Haga clic en **[!UICONTROL Nueva regla de validación de formulario]**.

   ![](assets/global-form-validation-rules-9.png)

   >[!NOTE]
   >
   >La lista desplegable [!UICONTROL Acciones de regla de validación de formulario] le permite eliminar o editar las reglas existentes.

1. Asigne un nombre a la regla, asígnele una descripción opcional e introduzca el mensaje de error que desea que vean los visitantes del formulario. Escriba uno o varios dominios que desee bloquear en el cuadro de reglas, seleccione **[!UICONTROL Activar regla]** y haga clic en **[!UICONTROL Crear]**.

   ![](assets/global-form-validation-rules-10.png)

>[!NOTE]
>
>Marketo Engage tiene una lista de bloqueados definida de dominios de correo electrónico de consumidor libre que se bloquean al utilizar la regla precargada &quot;Lista de bloqueados de dominio de correo electrónico de consumidor&quot;. [Ver esa lista aquí](/help/marketo/product-docs/administration/settings/assets/freemaildomains.csv) (para descargarla, asegúrate de que tu navegador esté actualizado y de que acepte descargas).

## Cómo deshabilitar el acceso por formulario{#how-to-disable-access-per-form}

Una vez activadas, las reglas se aplican a todos los formularios. Sin embargo, si tiene un formulario con requisitos específicos y no desea que se rechace nada, puede deshabilitar [!UICONTROL Reglas globales de validación de formularios] en la configuración del formulario.

1. En el formulario que desee, haga clic en **[!UICONTROL Configuración del formulario]** y luego en **[!UICONTROL Configuración]**.

   ![](assets/global-form-validation-rules-11.png)

1. Haga clic en el menú desplegable **[!UICONTROL Reglas de validación de formulario global]** y elija **[!UICONTROL Deshabilitado]**.

   ![](assets/global-form-validation-rules-12.png)

Cuando apruebe y publique el formulario, se omitirán las [!UICONTROL reglas globales de validación de formularios].
