---
description: 'Ejecución De Campaign: Documentos De Marketo: Documentación Del Producto'
title: Ejecutar campaña
exl-id: d550cf08-b295-4289-9bb0-79d81cabc245
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 1%

---

# Ejecutar campaña {#execute-campaign}

Una campaña ejecutable, como otras campañas, contiene una lista inteligente, un flujo y un programa. A diferencia de otras campañas, en realidad no se programa ni se activa. Solo otra campaña puede llamarla a través del paso Ejecutar flujo de campaña. Los pasos de flujo de la campaña ejecutable se ejecutan en serie con la campaña principal (a diferencia de la campaña de solicitud, que se ejecuta en paralelo en una campaña de Déclencheur independiente).

>[!NOTE]
>
>Las campañas ejecutables siempre son secundarias de la campaña (principal) que las llama.

## Cuándo utilizar Ejecutar campaña {#when-to-use-execute-campaign}

Hay muchas cosas que puede hacer con una campaña ejecutable. Están diseñadas para facilitar tareas operativas comunes, como el enrutamiento de posibles clientes, la administración del ciclo vital y la puntuación (entre otras), y se pueden utilizar para ejecutar el mismo flujo de trabajo desde Lote o Campañas activadas.

También puede utilizarlos cuando necesite ejecutar un flujo independiente, pero debe depender de los resultados de ese flujo en las opciones de paso de flujo subsiguientes (es decir, si es así, hágalo).

La ejecución de la campaña supone una mejora con [Solicitar campaña](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/request-campaign.md), ya que puede ejecutarse en serie, mientras que esta última solo se ejecuta en paralelo.

>[!NOTE]
>
>Los pasos de espera y los webhooks nunca serán compatibles con las campañas ejecutables. Para ello, debe utilizar Solicitar campaña en su lugar.

## Cómo crear una campaña ejecutable {#how-to-create-an-executable-campaign}

1. Haga clic con el botón derecho en el programa deseado y seleccione **[!UICONTROL Nueva campaña inteligente]**.

   ![](assets/execute-campaign-1.png)

1. Asigne un nombre y seleccione **[!UICONTROL Ejecutable]** y haga clic en **[!UICONTROL Crear]**.

   ![](assets/execute-campaign-2.png)

1. Defina la lista inteligente y el flujo, como cualquier otra campaña inteligente.

También puede clonar una campaña inteligente existente. Si clona una campaña ejecutable existente, aún tendrá que seleccionar la variable **[!UICONTROL Ejecutable]** después de ponerle nombre.

>[!NOTE]
>
>No puede clonar una campaña que contenga déclencheur.

## Usar contexto de token de la campaña principal {#use-parent-campaign-token-context}

Cuando se establece en true, se envían los siguientes contextos de token a la campaña secundaria (la que se está ejecutando):

* Mis tokens
* Tokens de campaña
* Tokens de programa
* Tokens de miembros
* [Tokens de déclencheur](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) (si se llama desde una campaña activada)

**Interacción de API**

Al utilizar Programar o Solicitar campaña [en la API](https://developers.marketo.com/rest-api/assets/smart-campaigns/#batch), ambos permiten pasar valores para Mis tokens, que anulan los valores establecidos para esos tokens en la campaña a la que llama. Si esa campaña ejecuta otra campaña y establece &quot;Use Parent Context to True&quot;, utilizará los valores pasados a través de la API en lugar de los valores establecidos en la aplicación.

## Cosas que hay que tener en cuenta {#things-to-note}

* La lista inteligente filtrará a cualquier persona que no cumpla los requisitos. Si una persona cumple los requisitos, el registro de actividad de Campaña ejecutada resultante los enumerará como &quot;Cualificado: VERDADERO&quot; (y FALSO si no lo hace)
* Se aplican reglas de calificación de programación de campaña (Configuración de campaña inteligente en la pestaña Programar )
* No se puede llamar a las campañas ejecutables en espacios de trabajo
* Si usa el [Eliminar del flujo](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-flow.md) acción de flujo dirigida a una campaña ejecutable, se dirige tanto al elemento secundario como al principal
* Aprovechar la herencia de tokens: por ejemplo, si tiene un solo flujo de puntuación común activado por varios recursos diferentes, puede definir una puntuación de Mi token predeterminada en la campaña secundaria y en la campaña principal para que pueda anular el valor de campaña de puntuación secundaria de sus campañas principales (consulte a continuación para ver un ejemplo visual)
* Las campañas ejecutables pueden llamarse hasta tres niveles (por ejemplo, Campaña principal > Secundario > Secundario > Secundario)

>[!CAUTION]
>
>No deje nunca inválidas las listas inteligentes de Campañas ejecutables; de lo contrario _nadie_ cumplirá los requisitos para ello. La práctica recomendada es crear recursos de listas inteligentes independientes, definirlos por completo y asegurarse de que son válidos. A continuación, utilice el filtro &quot;Miembro de la lista inteligente&quot; en la campaña ejecutable para poder intercambiar la definición de la lista inteligente.

## Ejemplo de herencia de token {#token-inheritance-example}

A continuación se muestra un ejemplo visual de herencia de tokens en una campaña ejecutable y dos campañas principales: una con contexto de token establecido en **[!UICONTROL Verdadero]**, el otro a **[!UICONTROL Falso]**.

Campaña secundaria con una puntuación de cambio identificada.

![](assets/execute-campaign-3.png)

La campaña infantil es Mis tokens.

![](assets/execute-campaign-4.png)

### Ejemplo 1: Verdadero {#example-one-true}

En el paso Ejecutar flujo de campaña de la primera campaña principal, &quot;Usar contexto de token de campaña principal&quot; se establece en **Verdadero**.

![](assets/execute-campaign-5.png)

La campaña de los padres es Mis tokens.

![](assets/execute-campaign-6.png)

Los resultados: la puntuación cambió en +10.

![](assets/execute-campaign-7.png)

### Ejemplo 2: False {#example-two-false}

En el paso Ejecutar flujo de campaña de la segunda campaña principal, &quot;Usar contexto de token de campaña principal&quot; se establece en **Falso**.

![](assets/execute-campaign-8.png)

La campaña de los padres es Mis tokens.

![](assets/execute-campaign-9.png)

Resultados: la puntuación no se ha modificado porque se ha utilizado el valor de puntuación de la campaña secundaria, +0.

![](assets/execute-campaign-10.png)
