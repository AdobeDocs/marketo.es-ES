---
unique-page-id: 7514898
description: 'Configuración de una campaña inteligente de Déclencheur para ventas con "Se solicita una campaña": documentos de Marketo, documentación del producto'
title: Configuración de una campaña inteligente de activador para ventas con “La campaña está solicitada”
exl-id: ed6d7c27-d54b-48e3-af67-19503da4ef56
feature: Smart Campaigns
source-git-commit: 65d607e279fb86b0816ccaec2f4bf3c69e309cb9
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 8%

---

# Configuración de una campaña inteligente de activador para ventas con “La campaña está solicitada” {#setting-up-a-trigger-smart-campaign-for-sales-using-campaign-is-requested}

Una de las mejores características de Marketo es la capacidad de permitir que los vendedores participen en el esfuerzo de marketing. Están en primera línea, interactuando con la gente. Los representantes de ventas deben tener la capacidad de dirigir el marketing en la dirección correcta.

>[!NOTE]
>
>Ejemplos de campañas inteligentes para solicitar:
>
>1. **Nutrición a largo plazo**: cuando no tengan presupuesto para este año y solo quieras mantenerte al tanto
>1. **Ciclo de ventas activo**: cuando el vendedor no desea ningún mensaje para la persona, excepto el suyo propio. (utilice el indicador suspendido de marketing para cancelar la suscripción temporalmente)
>
>Sé creativo. ¿Qué desea automatizar el vendedor? ¡Solo pídeles y ponlo en contacto!

1. Cree una campaña inteligente.

   ![](assets/setting-up-a-trigger-smart-campaign-for-sales-1.png)

1. Busque y arrastre el déclencheur **[!UICONTROL Se ha solicitado la campaña]** al lienzo.

   ![](assets/setting-up-a-trigger-smart-campaign-for-sales-2.png)

1. Las opciones de fuente indican qué tipo de solicitud se aceptará. Para la funcionalidad de Salesforce, asegúrate de elegir **[!UICONTROL Sales Insight]**.

   >[!TIP]
   >
   >Los operadores de origen son para la seguridad. Puede restringir la campaña a solicitudes realizadas únicamente por fuentes específicas, como otras campañas inteligentes o desarrolladores. Elija **[!UICONTROL Is Any]** en el primer cuadro si desea permitir solicitudes de todos los orígenes.
   >
   >_Recuerda_, al elegir Sales Insight, aparecerá por arte de magia en el cuadro de ventas. No te excedas. Demasiados serán ignorados por ellos.

   ![](assets/setting-up-a-trigger-smart-campaign-for-sales-3.png)

Esta es una excelente manera de ampliar su alcance de marketing a otros departamentos. Configure todo tipo de campañas para automatizar.

>[!TIP]
>
>No olvide nombrar claramente sus campañas inteligentes. Aparecerán en Sales Insight exactamente como les pongas nombre.
