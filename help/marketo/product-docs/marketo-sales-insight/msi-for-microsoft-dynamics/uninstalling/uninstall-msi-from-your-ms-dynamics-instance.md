---
unique-page-id: 37355600
description: 'Desinstalación de MSI desde la instancia de MS Dynamics: Marketo Docs: documentación del producto'
title: Desinstalar MSI de su instancia de MS Dynamics
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# Desinstalar MSI de su instancia de MS Dynamics {#uninstall-msi-from-your-ms-dynamics-instance}

Para desinstalar MSI de su instancia de MS Dynamics, deberá realizar pasos tanto en Marketo como en MS Dynamics.

>[!PREREQUISITES]
>
>[Deshabilitar sincronización global de MS Dynamics](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. En Marketo, haga clic en **Administrador**.

   ![](assets/one-1.png)

1. Haga clic en **Perspectiva de ventas**.

   ![](assets/six.png)

1. Haga clic en **Editar sincronización de campos**.

   ![](assets/seven.png)

1. Seleccione el **Desactivar sincronización** casilla de verificación y haga clic en **Guardar**.

   >[!NOTE]
   >
   >Asegúrese de que [deshabilite la sincronización global de MS Dynamics](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md) antes de desactivar la sincronización de campos.

   ![](assets/eight.png)

## Los siguientes pasos tienen lugar en la instancia de MS Dynamics: {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. Haga clic en **Configuración avanzada**.

1. Haga clic en **Soluciones**.

1. Select **Perspectiva de ventas de Marketo** y haga clic en el icono eliminar .

1. Cuando aparezca el modal de la solución de desinstalación, haga clic en **OK**.

   La desinstalación de la solución MS Dynamics suele tardar unos 20 minutos. Sin embargo, si tiene una instancia de MS Dynamics grande, puede tardar un poco más.

   >[!NOTE]
   >
   >Recuerde activar la sincronización de Global MS Dynamics una vez que desinstale MSI.
