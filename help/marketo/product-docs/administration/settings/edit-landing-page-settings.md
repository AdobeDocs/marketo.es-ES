---
unique-page-id: 2359918
description: 'Editar configuración de página de aterrizaje: documentos de Marketo, documentación del producto'
title: Editar configuración de página de aterrizaje
exl-id: 019b4651-3a66-46f9-8722-66af30194380
feature: Administration, Landing Pages
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 1%

---

# Editar configuración de página de aterrizaje {#edit-landing-page-settings}

Puede editar su nombre de dominio y página de reserva, habilitar o deshabilitar el rellenado previo del formulario, evitar el uso indebido de su página de aterrizaje y mucho más. Así es como.

>[!NOTE]
>
>**Se requieren permisos de administración**

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/edit-landing-page-settings-1.png)

1. Haga clic en **[!UICONTROL Páginas de aterrizaje]**.

   ![](assets/edit-landing-page-settings-2.png)

1. En la sección **[!UICONTROL Páginas de destino]**, haga clic en **[!UICONTROL Editar]**.

   ![](assets/edit-landing-page-settings-3.png)

1. Introduzca su dominio y la información de la página.

   ![](assets/edit-landing-page-settings-4.png)

   | Término | Definición |
   |---|---|
   | [!UICONTROL Nombre de dominio para páginas de aterrizaje] | Este es su CNAME. Un CNAME es la primera parte de la dirección URL que proporciona a las personas para páginas de aterrizaje. Por ejemplo, en `https://go.yourCompany.com`, la palabra &quot;ir&quot; es el CNAME. Puede tener varios, pero la mayoría de las personas solo utilizan el uno. |
   | [!UICONTROL Página de reserva] | Aquí es donde debe ir si la página de aterrizaje no existe o está caída. Más información sobre [páginas de reserva](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | [!UICONTROL Página principal] | Introduzca la URL de su sitio corporativo. |

1. Marque la casilla de verificación **[!UICONTROL Relleno previo de formulario]** para permitir que los formularios prerrellenen información de personas conocidas (cookies). Desmarque para bloquear.

   ![](assets/edit-landing-page-settings-5.png)

   >[!NOTE]
   >
   >Si desea que la etiqueta de relleno previo `<script>` aparezca al final de la etiqueta `<head>` en el código, marque la casilla **[!UICONTROL Insertar script de relleno previo al final del encabezado]**. Deje sin marcar si desea que aparezca al principio.
   >
   >Marque **[!UICONTROL Quitar vínculos de favicon predeterminados]** para evitar que Marketo inserte vínculos de favicon en el código.

1. Después de hacer las selecciones, haz clic en **[!UICONTROL Guardar]**.

   ![](assets/edit-landing-page-settings-6.png)

   ¡Buen trabajo! Las páginas de aterrizaje ahora tienen la información correcta y deben empezar a funcionar de inmediato.
