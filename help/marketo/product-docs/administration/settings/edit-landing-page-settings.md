---
unique-page-id: 2359918
description: 'Editar configuración de página de aterrizaje: documentos de Marketo, documentación del producto'
title: Editar configuración de página de aterrizaje
exl-id: 019b4651-3a66-46f9-8722-66af30194380
feature: Administration, Landing Pages
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Editar configuración de página de aterrizaje {#edit-landing-page-settings}

Puede editar su nombre de dominio y página de reserva, habilitar o deshabilitar el rellenado previo del formulario, evitar el uso indebido de su página de aterrizaje y mucho más. Así es como.

>[!NOTE]
>
>**Permisos de administración necesarios**

1. Vaya a la **[!UICONTROL Administrador]** área.

   ![](assets/edit-landing-page-settings-1.png)

1. Clic **[!UICONTROL Páginas de aterrizaje]**.

   ![](assets/edit-landing-page-settings-2.png)

1. En el **[!UICONTROL Páginas de aterrizaje]** , haga clic en **[!UICONTROL Editar]**.

   ![](assets/edit-landing-page-settings-3.png)

1. Introduzca su dominio y la información de la página.

   ![](assets/edit-landing-page-settings-4.png)

   | Término | Definición |
   |---|---|
   | [!UICONTROL Nombre de dominio para páginas de aterrizaje] | Este es su CNAME. Un CNAME es la primera parte de la dirección URL que proporciona a las personas para páginas de aterrizaje. Por ejemplo, en `https://go.yourCompany.com`, la palabra &quot;go&quot; es el CNAME. Puede tener varios, pero la mayoría de las personas solo utilizan el uno. |
   | [!UICONTROL Página de reserva] | Aquí es donde debe ir si la página de aterrizaje no existe o está caída. Más información sobre [páginas de reserva](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | [!UICONTROL Página principal] | Introduzca la URL de su sitio corporativo. |

1. Compruebe la **[!UICONTROL Relleno previo de formulario]** casilla de verificación para permitir que los formularios rellenen previamente información de personas conocidas (cookies). Desmarque para bloquear.

   ![](assets/edit-landing-page-settings-5.png)

1. Si desea evitar que un sitio malintencionado aparentemente aloje su contenido, consulte la **[!UICONTROL No permitir que las páginas de Marketo se incrusten en páginas web externas]** casilla de verificación

   ![](assets/edit-landing-page-settings-6.png)

   >[!NOTE]
   >
   >Si desea el relleno previo `<script>` etiqueta para que aparezca al final del `<head>` en el código, marque la **[!UICONTROL Inyectar script de relleno previo al final del encabezado]** cuadro. Deje sin marcar si desea que aparezca al principio.
   >
   >Marque **[!UICONTROL Eliminar vínculos de favoritos predeterminados]** para evitar que Marketo inserte vínculos de favicon en el código.

1. Después de realizar las selecciones, haga clic en **[!UICONTROL Guardar]**.

   ![](assets/edit-landing-page-settings-7.png)

   ¡bueno trabajo! Las páginas de aterrizaje ahora tienen la información correcta y deben empezar a funcionar de inmediato.
