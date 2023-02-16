---
unique-page-id: 2359918
description: 'Editar la configuración de la página de aterrizaje: documentos de Marketo: documentación del producto'
title: Editar la configuración de la página de aterrizaje
exl-id: 019b4651-3a66-46f9-8722-66af30194380
source-git-commit: 07899e541b3624e99e0ead59d898ced2ab4e57af
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Editar la configuración de la página de aterrizaje {#edit-landing-page-settings}

Puede editar el nombre de dominio y la página de reserva, habilitar o deshabilitar el cumplimentado previo del formulario, evitar el uso indebido de la página de aterrizaje, etc. Así es como.

>[!NOTE]
>
>**Se requieren permisos de administrador**

1. Vaya a la **Administrador** .

   ![](assets/edit-landing-page-settings-1.png)

1. Haga clic en **Páginas de aterrizaje**.

   ![](assets/edit-landing-page-settings-2.png)

1. En el **Páginas de aterrizaje** , haga clic en **Editar**.

   ![](assets/edit-landing-page-settings-3.png)

1. Introduzca la información de su dominio y página.

   ![](assets/edit-landing-page-settings-4.png)

   | Término | Definición |
   |---|---|
   | Nombre de dominio para páginas de aterrizaje | Este es su CNAME. Un CNAME es la primera parte de la dirección URL que se proporciona a las personas para las páginas de aterrizaje. Por ejemplo, en `https://go.yourCompany.com`, la palabra &quot;go&quot; es el CNAME. Se pueden tener múltiples, pero la mayoría de las personas solo usan la una. |
   | Página de reserva | Aquí es donde debe ir si la página de aterrizaje no existe o no está activa. Más información sobre [páginas de reserva](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | Página principal | Introduzca la dirección URL del sitio corporativo. |

1. Marque la **Form Prefill** casilla de verificación para permitir que los formularios rellenen previamente la información para personas conocidas (con cookies). Desmarque para bloquear.

   ![](assets/edit-landing-page-settings-5.png)

1. Si desea evitar que un sitio malintencionado aparentemente aloje su contenido, consulte la **No permitir que las páginas de Marketo se incrusten en páginas web externas** casilla de verificación.

   ![](assets/edit-landing-page-settings-6.png)

   >[!NOTE]
   >
   >Si desea rellenar previamente `<script>` para que aparezca al final del `<head>` en el código, marque la casilla **Inyectar la secuencia de comandos de prellenado al final de la cabeza** en la ventana Deje sin marcar si desea que aparezca al principio.
   >
   >Marque **Eliminar vínculos de favoritos predeterminados** para evitar que Marketo inserte vínculos de favoritos en el código.

1. Después de realizar las selecciones, haga clic en **Guardar.**

   ![](assets/edit-landing-page-settings-7.png)

   ¡bueno trabajo! Las páginas de aterrizaje ahora tienen la información correcta y deben empezar a funcionar de inmediato.
