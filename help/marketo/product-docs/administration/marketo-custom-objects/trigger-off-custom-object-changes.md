---
unique-page-id: 11378713
description: Déclencheur De Los Cambios De Objetos Personalizados - Documentos De Marketo - Documentación Del Producto
title: Déclencheur de los cambios en objetos personalizados
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
source-git-commit: 99b11e17e9c2255a19c658b166e7b38c45cf1001
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
>Póngase en contacto con [Asistencia de Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) para tener activados los Déclencheur de cambio de objeto personalizado.

En la lista inteligente de una campaña inteligente, puede crear un déclencheur de una acción de flujo cuando se agrega un objeto personalizado a una persona o empresa. También puede crear una lista inteligente que utilice un *change* en un objeto personalizado como déclencheur. Por ejemplo, utilícelo para enviar un correo electrónico cuando se actualice un nombre de curso.

>[!NOTE]
>
>No se crea una entrada de registro de actividad cuando se cambia un registro de objeto personalizado.

1. En Marketo, vaya a **Actividades de marketing.**

   ![](assets/trigger-off-custom-object-changes-1.png)

1. Cree o abra una campaña inteligente existente y seleccione la lista inteligente.

   ![](assets/trigger-off-custom-object-changes-2.png)

1. Busque el déclencheur que necesita y arrástrelo al lienzo.

   ![](assets/trigger-off-custom-object-changes-3.png)

1. Seleccione el atributo de déclencheur.

   ![](assets/trigger-off-custom-object-changes-4.png)

1. Opcionalmente, defina una restricción.

   ![](assets/trigger-off-custom-object-changes-5.png)

1. Y ahí estás. El cambio se guarda automáticamente.

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [Crear una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Explicación de los objetos personalizados de Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

