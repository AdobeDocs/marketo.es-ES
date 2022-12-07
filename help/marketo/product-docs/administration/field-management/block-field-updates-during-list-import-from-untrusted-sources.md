---
unique-page-id: 2360335
description: Bloquear actualizaciones de campos durante la importación de listas desde fuentes no confiables - Documentos de Marketo - Documentación del producto
title: Bloquear actualizaciones de campo durante la importación de lista desde fuentes que no son de confianza
exl-id: 0fd59f0c-6cb9-442c-937b-da18a4466873
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Bloquear actualizaciones de campo durante la importación de lista desde fuentes que no son de confianza {#block-field-updates-during-list-import-from-untrusted-sources}

Puede confiar más en los datos de algunas listas que en otras. A veces, los datos son dudosos y se desea tomar si el campo está en blanco, pero no si hay un valor existente. Esto se puede lograr bloqueando las actualizaciones de campos en campos clave.

>[!NOTE]
>
>**Se requieren permisos de administrador**

## Bloqueo De Actualizaciones De Campo De Fuentes Que No Son De Confianza {#blocking-field-updates-from-untrusted-sources}

1. Vaya a la **Administrador** .

   ![](assets/blocking-field-updates-from-untrusted-sources-1.png)

1. Haga clic en **Gestión de las actividades sobre el terreno**.

   ![](assets/blocking-field-updates-from-untrusted-sources-2.png)

1. Busque el campo que desee, selecciónelo y, a continuación, debajo de **Acciones de campo**, haga clic en **Bloquear actualizaciones de campos**.

   ![](assets/blocking-field-updates-from-untrusted-sources-3.png)

1. Marque **Importación de lista fuente no confiable** y haga clic en **Aplicar**.

   ![](assets/blocking-field-updates-from-untrusted-sources-4.png)

>[!TIP]
>
>Puede mantener los campos a salvo de todas las listas, de confianza y de confianza, también comprobando **Importar lista fuente de confianza**.

Repita los pasos anteriores para cualquier otro campo que desee mantener a salvo de listas que no sean de confianza.

## Ejecución de una importación de lista que no sea de confianza {#running-an-untrusted-list-import}

1. Al ejecutar la importación de lista, asegúrese de seleccionar **No confiable** si desea que todos los campos configurados en el paso anterior sean seguros.

   ![](assets/blocking-field-updates-from-untrusted-sources-5.png)

Para obtener instrucciones detalladas sobre la importación de listas, consulte [Importar una lista de personas](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md).

¡Buen trabajo! Ahora sabe cómo mantener los campos clave a salvo de listas que no sean de confianza.
