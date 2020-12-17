---
title: comprensión-mis-tokens
description: Explicación de mis tokens
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---


# Explicación de mis tokens

<br> 

Mis tokens son variables personalizadas que se pueden crear y utilizar en las carpetas de programas o campañas. Se ven así: `{{_my.Name of Token_}}`

## Ejemplos

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

Para acceder a Mis tokens y crearlos, seleccione el programa o la campaña y vaya a la ficha [!UICONTROL Mis tokens]. Arrastre y suelte cualquier token en el lienzo [!UICONTROL Tokens locales].

![Imagen uno](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-1.png)

>[!CAUTION]
>
>Los nombres de Mis tokens no se pueden cambiar después de guardarlos, por lo que debe elegir con cuidado.

>[!NOTE]
>
>Mis tokens no se resolverán al enviar un correo electrónico desde Sales Insight en Microsoft Dynamics o Salesforce; solo se rellenarán los tokens estándar (posible cliente, Compañía, etc.). Sin embargo, los valores predeterminados para los tokens funcionarán.

>[!NOTE]
>
>Los tokens de vínculo no funcionan en correos electrónicos de solo texto.

## Anidado de tokens

Al crear un nuevo token, otros objetos del árbol pueden hacer referencia a él. Puede anular las variables globales en los niveles inferiores del árbol. Hay una estructura de nombres para la que se creó el token para facilitar la administración.

* **Token local:** el token se creó directamente en ese programa o carpeta.
* **[Token anulado:](/help/sky/override-an-inherited-my-token.md)** el token se heredó, pero se hizo una excepción en este programa o carpeta.
* **Token heredado:** el token se creó en el árbol en algún lugar de un programa o carpeta de nivel superior.

Puede encontrar estos tres tipos en la ficha **[!UICONTROL Mis tokens]** de su programa o campaña.

![Imagen dos](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-2.png)

Mover programas y carpetas también afecta a los tokens. Compruebe siempre que las referencias no estén rotas durante el movimiento.

>[!NOTE]
>
>Si el correo electrónico enviado desde un programa de participación es un correo electrónico secundario de un programa predeterminado (es decir, no local para el programa de participación), todos los tokens utilizados en el correo electrónico se resuelven a partir del programa predeterminado en el que reside el correo electrónico secundario.

## Uso del token

Seleccione cualquier token y, a continuación, haga clic en el icono de uso situado en la esquina superior derecha para ver una lista de recursos que contengan dicho token.

![Imagen tres](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-3.png)

![Imagen Cuatro](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-4.png)

**Buceo profundo**

Obtenga más información sobre cada uno de los Mis tokens:

* [CAMPAÑA CRM](/help/sky/my-token-crm-campaign.md)
* [Fecha](/help/sky/my-token-date.md)
* [Archivo de calendario](/help/sky/my-token-calendar-file.md)
* [Imagen](/help/sky/my-token-image.md)
* [Vínculo](/help/sky/my-token-link.md)
* [Número](/help/sky/my-token-number.md)
* [Texto enriquecido](/help/sky/my-token-rich-text.md)
* [Puntuación](/help/sky/my-token-score.md)
* [Secuencia de comandos de correo electrónico](/help/sky/my-token-email-script.md)
* [Texto](/help/sky/my-token-text.md)
