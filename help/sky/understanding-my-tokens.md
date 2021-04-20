---
title: comprensión-mis-tokens
description: Explicación de mis tokens
exl-id: d56748e2-d742-45dd-96a8-dd80e30d9d8b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# Explicación de mis tokens

<br> 

Mis tokens son variables personalizadas que puede crear y utilizar en sus programas o carpetas de campaña. Se ven así: `{{_my.Name of Token_}}`

## Ejemplos

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

Para acceder a My Tokens y crearlos, seleccione la carpeta de su programa o campaña y vaya a la pestaña [!UICONTROL My Tokens]. Arrastre y suelte cualquier token en el lienzo [!UICONTROL Tokens locales].

![Imagen uno](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-1.png)

>[!CAUTION]
>
>Los nombres de mis tokens no se pueden cambiar una vez guardados, por lo que elija con cuidado.

>[!NOTE]
>
>Mis tokens no se resolverán al enviar un correo electrónico desde Sales Insight en Microsoft Dynamics o Salesforce; solo se rellenarán los tokens estándar (posible cliente, empresa, etc.). Sin embargo, los valores predeterminados para los tokens funcionarán.

>[!NOTE]
>
>Los tokens de vínculo no funcionan en los correos electrónicos de solo texto.

## Anidado de tokens

Cuando se crea un nuevo token, otros objetos del árbol pueden hacer referencia a él. Puede anular las variables globales en los niveles inferiores del árbol. Hay una estructura de nombres para la que el token se creó para facilitar la administración.

* **Token local:** el token se creó directamente en ese programa o carpeta.
* **[Token ignorado:](/help/sky/override-an-inherited-my-token.md)** el token se heredó, pero se hizo una excepción en este programa o carpeta.
* **Token heredado:** el token se creó en el árbol en algún lugar de un programa o carpeta de nivel superior.

Puede encontrar estos tres tipos en la pestaña **[!UICONTROL My Tokens]** de su programa o carpeta de campaña.

![Imagen dos](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-2.png)

Mover programas y carpetas también afecta a los tokens. Compruebe siempre que las referencias no estén rotas durante el movimiento.

>[!NOTE]
>
>Si el correo electrónico enviado desde un programa de participación es un correo electrónico secundario de un programa predeterminado (es decir, no local para el programa de participación), cualquier My Tokens utilizado en el correo electrónico se resuelve desde el programa predeterminado en el que reside el correo electrónico secundario.

## Uso del token

Seleccione cualquier token y, a continuación, haga clic en el icono de uso que hay en la esquina superior derecha para ver una lista de recursos que contienen dicho token.

![Imagen tres](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-3.png)

![Imagen Cuatro](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-4.png)

**Análisis profundo**

Obtenga más información sobre cada uno de los Mis tokens:

* [Campaña CRM](/help/sky/my-token-crm-campaign.md)
* [Fecha](/help/sky/my-token-date.md)
* [Archivo de calendario](/help/sky/my-token-calendar-file.md)
* [Imagen](/help/sky/my-token-image.md)
* [Vínculo](/help/sky/my-token-link.md)
* [Número](/help/sky/my-token-number.md)
* [Texto enriquecido](/help/sky/my-token-rich-text.md)
* [Puntuación](/help/sky/my-token-score.md)
* [Script de correo electrónico](/help/sky/my-token-email-script.md)
* [Texto](/help/sky/my-token-text.md)
