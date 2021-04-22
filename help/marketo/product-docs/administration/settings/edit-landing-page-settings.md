---
unique-page-id: 2359918
description: 'Editar la configuración de la página de aterrizaje: documentos de Marketo: documentación del producto'
title: Editar la configuración de la página de aterrizaje
exl-id: 019b4651-3a66-46f9-8722-66af30194380
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# Editar la configuración de la página de aterrizaje {#edit-landing-page-settings}

Puede editar el nombre de dominio y la página de reserva, habilitar o deshabilitar el cumplimentado previo del formulario, evitar el uso indebido de la página de aterrizaje, etc. Así es como.

>[!NOTE]
>
>**Se requieren permisos de administrador**

1. En **Administración**, haga clic en **Páginas de aterrizaje**.

   ![](assets/image2014-9-10-9-3a47-3a40.png)

1. En la sección **Páginas de aterrizaje**, haga clic en **Editar**.

   ![](assets/image2014-9-10-9-3a47-3a12.png)

1. Introduzca la información de su dominio y página.

   | Término | Definición |
   |---|---|
   | Nombre de dominio para páginas de aterrizaje | Este es su CNAME. Un CNAME es la primera parte de la dirección URL que se proporciona a las personas para las páginas de aterrizaje. Por ejemplo, en `https://go.yourCompany.com`, la palabra &quot;go&quot; es el CNAME. Se pueden tener múltiples, pero la mayoría de las personas solo usan la una. |
   | Página de reserva | Aquí es donde debe ir si la página de aterrizaje no existe o no está activa. Obtenga más información sobre [páginas de reserva](/help/marketo/product-docs/administration/settings/set-a-fallback-page.md). |
   | Página principal | Introduzca la dirección URL del sitio corporativo. |

   ![](assets/three.png)

1. Marque la casilla **Form Prefill** para permitir que los formularios rellenen previamente la información de personas conocidas (con cookies). Desmarque para bloquear.

   ![](assets/four.png)

1. Si desea evitar que un sitio malintencionado aparentemente aloje su contenido, marque la casilla **No permitir que las páginas de Marketo se incrusten en páginas web externas**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Si desea que la etiqueta `<script>` de relleno previo aparezca al final de la etiqueta `<head>` en el código, marque la casilla **Inyectar script de relleno previo al final del cabezal**. Deje sin marcar si desea que aparezca al principio.
   >
   >Marque **Remove default favicon links** para evitar que Marketo inserte vínculos de favoritos en el código.

1. Después de realizar las selecciones, haga clic en **Guardar.**

   ![](assets/six.png)

   ¡bueno trabajo! Las páginas de aterrizaje ahora tienen la información correcta y deben empezar a funcionar de inmediato.
