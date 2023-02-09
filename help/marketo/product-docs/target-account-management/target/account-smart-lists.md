---
unique-page-id: 11378814
description: Listas inteligentes de cuentas - Documentos de Marketo - Documentación del producto
title: Listas inteligentes de cuenta
exl-id: fbdfb2b8-0061-467d-be89-527744a659a9
source-git-commit: adff42d54d7953c9ec72e4d736ce0153502be960
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# Listas inteligentes de cuenta {#account-smart-lists}

A continuación se muestra cómo identificar de forma rápida y precisa sus cuentas de alto valor.

>[!NOTE]
>
>Esta función solo está disponible para aquellos que tengan el complemento Administración de cuentas de Target y una licencia de TAM emitida.

## Crear una lista inteligente de cuentas {#create-an-account-smart-list}

1. En Marketo, vaya a **Actividades de marketing**.

   ![](assets/account-smart-lists-1.png)

1. Busque y seleccione el programa que desee.

   ![](assets/account-smart-lists-2.png)

1. Haga clic en el **Nuevo** y seleccione **Nuevo recurso local**.

   ![](assets/account-smart-lists-3.png)

1. Haga clic en **Lista inteligente de cuentas**.

   ![](assets/account-smart-lists-4.png)

1. Introduzca un nombre y haga clic en **Crear** (La descripción y las etiquetas son opcionales).

   ![](assets/account-smart-lists-5.png)

Se ha creado la lista inteligente de cuentas. Consulte a continuación los pasos para definir sus reglas.

## Reglas de lista inteligente de cuentas {#account-smart-list-rules}

Las listas inteligentes de cuentas funcionan de manera similar a las listas inteligentes estándar, con una excepción notable: contenedores.

1. Para definir la lista inteligente de cuentas, haga clic en el botón **Reglas de lista inteligente de cuentas** pestaña .

   ![](assets/account-smart-lists-6.png)

1. Elija los filtros de cuenta que desee. En este ejemplo elegimos _El sector es el sector sanitario_.

   ![](assets/account-smart-lists-7.png)

   ![](assets/account-smart-lists-8.png)

   >[!NOTE]
   >
   >Los datos del indicador ICP que se han utilizado en su [Clasificación y ajuste de perfiles de cuenta](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md) aparecerá como Atributos de cuenta personalizados para su uso en la lista inteligente de cuentas. Estos datos de atributo personalizados se basan en cuándo se creó o actualizó el modelo de perfil de cuenta.

1. Elija los filtros de persona coincidentes. En este ejemplo elegimos _El estado es California_.

   ![](assets/account-smart-lists-9.png)

**Paso opcional**: Aquí es donde entran los contenedores. Si elige un filtro adicional de persona coincidente, puede soltarlo debajo del primero o _en_ , creando un contenedor. En este ejemplo estamos creando un contenedor añadiendo _El puesto de trabajo es CFO_.

![](assets/account-smart-lists-10.png)

Así se verá el contenedor.

![](assets/account-smart-lists-11.png)

>[!NOTE]
>
>Al crear un contenedor de filtros, se crea una regla &quot;y&quot;, lo que significa que solo devolverá todos los resultados combinados. En este ejemplo, cuentas con una industria de la salud, junto con estar ubicados en California _y_ con alguien incluido como CFO. Si no desea utilizar contenedores, simplemente suelte el filtro debajo o encima del existente.

¡Y eso es todo! Consulte la siguiente sección para ver cómo puede aprovechar su Lista inteligente de cuentas.

>[!TIP]
>
>Al igual que con las listas inteligentes estándar, puede utilizar la lógica avanzada para restringir aún más los resultados. Necesita al menos tres filtros para hacerlo y, en Listas inteligentes de cuenta, un contenedor (independientemente de cuántos filtros contenga) es igual a un filtro.

## Acciones de la lista inteligente de cuentas {#account-smart-list-actions}

En la ficha Información general de la lista inteligente de cuentas, verá algunas opciones de acción.

**Exportar**: Esto exporta los resultados de la lista inteligente de cuentas como CSV.

**Clonar**: Realiza una copia de la lista inteligente de cuentas.

**Enviar a red de publicidad**: Envía la lista a LinkedIn como una nueva audiencia coincidente.

También puede hacer referencia a su lista inteligente de cuentas en una campaña o lista inteligente estándar utilizando la variable _Miembros de la lista inteligente de cuentas_ filtro.

![](assets/account-smart-lists-12.png)

>[!NOTE]
>
>Los resultados de la Lista inteligente Personas de cuenta mostrarán a todas las personas de las cuentas identificadas, no solo a las personas que se encuentran a través de filtros Personas coincidentes en la lista inteligente de cuentas.

>[!NOTE]
>
>**Definición**
>
>**Miembros de la lista inteligente de cuentas**: En este caso, la palabra &quot;miembro&quot; se refiere a la cuenta en sí, por lo que &quot;miembro del pueblo&quot; se refiere a las personas reales (registros de Marketo) de esas cuentas.
