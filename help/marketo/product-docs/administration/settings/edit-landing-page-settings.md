---
unique-page-id: 2359918
description: Cómo editar el nombre de dominio, la página de reserva, el relleno previo del formulario y otras opciones de página de aterrizaje.
title: Editar configuración de página de destino
exl-id: 019b4651-3a66-46f9-8722-66af30194380
feature: Administration, Landing Pages
TQID: https://experienceleague.adobe.com/dOvxpv09JPPBMNjqA0JTe-L4wIWUtkEELLl-PCs4CME
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 236
ht-degree: 5%

---

# Editar configuración de página de destino {#edit-landing-page-settings}

Puede editar su nombre de dominio y página de reserva, habilitar o deshabilitar el rellenado previo del formulario, evitar el uso indebido de su página de aterrizaje y mucho más. Siga los pasos a continuación.

>[!NOTE]
>
>**Se requieren permisos de administrador**

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
   | [!UICONTROL Nombre de dominio para páginas de aterrizaje] | Este es su CNAME. Un CNAME es la primera parte de la dirección URL que proporciona a las personas para páginas de aterrizaje. Por ejemplo, en `https://go.yourCompany.com`, la palabra &quot;ir&quot; es el CNAME. Puede tener varios, pero la mayoría de las personas solo utilizan uno. |
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

   Las páginas de aterrizaje ahora tienen la información correcta y deben comenzar a funcionar inmediatamente.
