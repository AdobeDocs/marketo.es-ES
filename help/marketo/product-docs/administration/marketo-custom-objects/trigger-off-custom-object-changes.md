---
unique-page-id: 11378713
description: Déclencheur De Los Cambios De Objetos Personalizados - Documentos De Marketo - Documentación Del Producto
title: Déclencheur de los cambios en objetos personalizados
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# Déclencheur de los cambios en objetos personalizados {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Esta función solo está disponible:
>
>* Para clientes en la infraestructura Orion
>* Para usar únicamente con objetos personalizados de Marketo, no con objetos personalizados sincronizados mediante la integración nativa de Salesforce o Microsoft Dynamics
>* Como déclencheur, no como filtro

>
>
Póngase en contacto con el [Soporte técnico de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para habilitar los Déclencheur de cambio de objeto personalizado.

En la lista inteligente de una campaña inteligente, puede crear un déclencheur de una acción de flujo cuando se agrega un objeto personalizado a una persona o empresa. También puede crear una lista inteligente que utilice un *cambio* en un objeto personalizado como déclencheur. Por ejemplo, utilícelo para enviar un correo electrónico cuando se actualice un nombre de curso.

>[!NOTE]
>
>No se crea una entrada de registro de actividad cuando se cambia un registro de objeto personalizado.

1. En Marketo, vaya a **Marketing Activities.**

   ![](assets/image2016-7-25-15-3a49-3a52.png)

1. Cree o abra una campaña inteligente existente y seleccione la lista inteligente.

   ![](assets/image2016-7-25-16-3a9-3a19.png)

1. Busque el déclencheur que necesita y arrástrelo al lienzo.

   ![](assets/image2016-7-25-16-3a16-3a43.png)

1. Seleccione el atributo de déclencheur.

   ![](assets/image2016-7-25-16-3a21-3a42.png)

1. Opcionalmente, defina una restricción.

   ![](assets/image2016-9-6-14-3a25-3a22.png)

1. Y ahí estás. El cambio se guarda automáticamente.

   ![](assets/image2016-9-6-14-3a25-3a54.png)

   >[!NOTE]
   >
   >* [Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Explicación de los objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

