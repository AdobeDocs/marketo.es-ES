---
unique-page-id: 11378814
description: 'Listas inteligentes de cuenta: Documentos de Marketo, documentación del producto'
title: Listas inteligentes de cuentas
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
feature: Target Account Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# Listas inteligentes de cuentas {#account-smart-lists}

A continuación se indica cómo identificar de forma rápida y precisa sus cuentas de alto valor.

>[!NOTE]
>
>Esta función solo está disponible para los que tengan el complemento Administración de cuentas de Target y una licencia de TAM emitida.

## Crear una lista inteligente de cuentas {#create-an-account-smart-list}

1. En Marketo, vaya a **Actividades de marketing**.

   ![](assets/account-smart-lists-1.png)

1. Busque y seleccione el programa que desee.

   ![](assets/account-smart-lists-2.png)

1. Haga clic en el menú desplegable **Nuevo** y seleccione **Nuevo recurso local**.

   ![](assets/account-smart-lists-3.png)

1. Haga clic en **Lista inteligente de cuentas**.

   ![](assets/account-smart-lists-4.png)

1. Escriba un nombre y haga clic en **Crear** (la descripción y las etiquetas son opcionales).

   ![](assets/account-smart-lists-5.png)

Se ha creado su lista inteligente de cuentas. Consulte a continuación los pasos para definir sus reglas.

## Reglas de lista inteligente de cuentas {#account-smart-list-rules}

Las listas inteligentes de cuentas funcionan de manera similar a las listas inteligentes estándar, con una excepción notable: los contenedores.

1. Para definir la lista inteligente de cuentas, haga clic en la ficha **Reglas de la lista inteligente de cuentas**.

   ![](assets/account-smart-lists-6.png)

1. Elija los filtros de cuenta que desee. En este ejemplo elegimos _Sector es atención sanitaria_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

   >[!NOTE]
   >
   >Los datos del indicador ICP que se usaron en su [clasificación y ajuste de generación de perfiles de cuenta](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md) aparecerán como Atributos de cuenta personalizados para usarlos en su Lista inteligente de cuentas. Estos datos de atributos personalizados se basan en el momento en el que se creó o actualizó el modelo de perfil de cuenta.

1. Elija su filtro de persona coincidente. En este ejemplo elegimos _El estado es California_.

   ![](assets/account-smart-lists-9.png)

**PASO OPCIONAL**: Aquí es donde entran los contenedores. Si elige un filtro de persona coincidente adicional, puede soltarlo debajo del primero o _en_, creando un contenedor. En este ejemplo creamos un contenedor al agregar _El puesto es CFO_.

![](assets/account-smart-lists-10.png)

Este es el aspecto que tendrá el contenedor.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>Al crear un contenedor de filtros, se crea una regla &quot;y&quot;, lo que significa que solo devolverá todos los resultados combinados. En este ejemplo, las cuentas con una industria de la salud, junto con estar ubicado en California _y_ con alguien listado como CFO. Si no desea utilizar contenedores, simplemente suelte el filtro por debajo o por encima del existente.

¡Y eso es todo! Consulte la sección siguiente para ver cómo puede aprovechar su lista inteligente de cuentas.

>[!TIP]
>
>Al igual que con las listas inteligentes estándar, puede utilizar la lógica avanzada para restringir aún más los resultados. Necesita al menos tres filtros para hacerlo y, en las listas inteligentes de cuentas, un contenedor (independientemente de cuántos filtros contenga él mismo) es igual a un filtro.

## Acciones de la lista inteligente de cuentas {#account-smart-list-actions}

En la pestaña Información general de la lista inteligente de cuentas, verá algunas opciones de acción.

**Exportar**: Esto exporta los resultados de su Lista inteligente de cuentas como CSV.

**Clonar**: crea una copia de la lista inteligente de cuentas.

**Enviar a la red de anuncios**: envía la lista a LinkedIn como una nueva audiencia coincidente.

También puede hacer referencia a su lista inteligente de cuentas en una campaña o lista inteligente estándar usando el filtro _Personas, miembros de la lista inteligente de cuentas_.

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>Los resultados de la lista inteligente Personas miembro de cuenta mostrarán todas las personas de las cuentas identificadas, no solo las personas que se encuentren a través de filtros de Personas coincidentes en la lista inteligente de cuentas.

>[!NOTE]
>
>**Definición**
>
>**Lista inteligente de miembros de la cuenta Personas**: En este caso, la palabra &quot;miembro&quot; hace referencia a la propia cuenta, por lo que &quot;miembro de personas&quot; hace referencia a las personas reales (registros de Marketo) en esas cuentas.
