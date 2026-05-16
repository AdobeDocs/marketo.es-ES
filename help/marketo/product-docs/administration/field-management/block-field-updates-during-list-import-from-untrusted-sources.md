---
unique-page-id: 2360335
description: Impida que los campos clave se sobrescriban durante las importaciones de listas de fuentes que no son de confianza para proteger los datos existentes.
title: Bloquear actualizaciones de campos durante la importación de listas desde orígenes que no son de confianza
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
feature: Field Management
TQID: https://experienceleague.adobe.com/cT1pOoWjR-UdHLqNJwhwgR9R12ciIa95q1xHPTf7rBY
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 205
ht-degree: 10%

---

# Bloquear actualizaciones de campos durante la importación de listas desde orígenes que no son de confianza {#block-field-updates-during-list-import-from-untrusted-sources}

Puede confiar más en los datos de algunas listas que en otras. A veces, los datos son cuestionables y se desea aceptar si el campo está en blanco, pero no si existe un valor. Para ello, bloquee las actualizaciones de los campos de los campos clave.

>[!NOTE]
>
>**Se requieren permisos de administrador**

## Bloqueo De Actualizaciones De Campos De Fuentes Que No Son De Confianza {#blocking-field-updates-from-untrusted-sources}

1. Vaya al área de **[!UICONTROL Admin]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Haga clic en **[!UICONTROL Administración de campos]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Busque el campo que desee, selecciónelo y en **[!UICONTROL Acciones de campo]**, haga clic en **[!UICONTROL Bloquear actualizaciones de campo]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Compruebe el origen de **[!UICONTROL Importación de lista que no es de confianza]** y haga clic en **[!UICONTROL Aplicar]**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>Puede mantener los campos a salvo de todas las listas, de confianza y no de confianza, comprobando también **[!UICONTROL Importar lista de origen de confianza]**.

Repita los pasos anteriores para cualquier otro campo que desee proteger de listas que no sean de confianza.

## Ejecución de una importación de lista que no es de confianza {#running-an-untrusted-list-import}

1. Al ejecutar la importación de la lista, asegúrese de seleccionar **[!UICONTROL No es de confianza]** si desea que todos los campos que configuró en el paso anterior sean seguros.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Para obtener instrucciones detalladas sobre cómo importar listas, consulte [Importar una lista de personas](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

Los campos clave ahora están protegidos de las importaciones de listas que no son de confianza.
