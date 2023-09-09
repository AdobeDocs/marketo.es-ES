---
unique-page-id: 42762322
description: 'Pestaña Configuración de Marketo Sales Insight en Salesforce: Documentos de Marketo: documentación del producto'
title: Pestaña Configuración de Marketo Sales Insight en Salesforce
exl-id: 4e2abd48-b0a5-4b71-939b-e66c7e39bb6c
feature: Marketo Sales Insights
source-git-commit: 4848676d423ff96c2e880819bc760b2f8dbbd094
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---

# Pestaña Configuración de Marketo Sales Insight en Salesforce {#marketo-sales-insight-configuration-tab-in-salesforce}

## Configuración operativa {#operational-settings}

Deberá tener esto configurado para empezar a utilizar el conocimiento de ventas en SFDC.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-1.png)

* MSI utiliza la API de SOAP y la de REST
* La página Información de ventas de su cuenta de Marketo tendrá dos paneles correspondientes con credenciales de API de SOAP y REST que puede copiar y pegar aquí
* La API de SOAP y REST tiene tiempos de espera independientes que puede establecer según las necesidades de su organización. El tiempo máximo permitido es de 120 segundos
* Desactivación del panel de perspectivas: puede eliminar las credenciales de la API de REST y solo utilizar la API de SOAP. Al hacerlo, se deshabilita la pestaña Tablero de perspectivas en todos los paneles de fuerza visual de MSI

## Configuración de MSI {#msi-configuration}

Las configuraciones son aplicables a todos los usuarios de MSI y no son específicas de los perfiles.

**Configuración de página de Visualforce**

* Activar lista desplegable de Acción:
   * Capacidad para ocultar el menú desplegable Enviar correo electrónico de Marketo desde en el diseño de MSI de contacto y posible cliente
   * Capacidad para ocultar las opciones de Agregar a Marketo Campaign de la lista desplegable en el diseño de MSI de posible cliente y contacto
* Próximos eventos: permite mostrar eventos invitados, todos los eventos a los usuarios u ocultar esta pestaña por completo
* Próximas campañas: capacidad de mostrar todas las campañas de correo electrónico u ocultar completamente esta pestaña
* Cargar próximas campañas y eventos: capacidad para reducir el número de llamadas a la API de REST realizadas por los usuarios colocando la pestaña eventos y campañas detrás de un botón &quot;Cargar próximos elementos&quot; bajo demanda
* Configuración de ficha: las cinco fichas estarán disponibles de forma predeterminada. Puede elegir el orden de las pestañas en el panel Información de ventas. El mismo orden se aplicará a todos los diseños (posible cliente, contacto, cuenta, oportunidad)

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-2.png)

**Pestaña Global de Marketo**

* Fuente RSS habilitada: cuando está habilitada, los usuarios de MSI pueden ver su fuente de posibles clientes en una fuente RSS (además de la fuente de posibles clientes en Salesforce). La fuente RSS solo puede funcionar si la función &quot;Caducidad del token&quot; está desactivada. Esta configuración se controla en la página de administración de Sales Insight de Marketo.
* Mejor modo de depuración
* Ocultar predeterminado: la opción que elija aquí será el número de días que se ocultará la mejor opción en la pestaña Mejor opción de Marketo al hacer clic en el icono &quot;Ocultar&quot;
* Campo de estado de contacto: la opción que elija aquí será el valor que se rellene en la columna Encabezado de estado de la pestaña Lo mejor para Marketo
* Configuración de fuente en directo: la opción para mostrar solo la fuente en directo (en los paneles Posible cliente, Contacto, Cuenta y Oportunidad y en la página Global Marketo), solo la fuente de posible cliente (en la página global de Marketo) o ambas
* Configuración de ficha: las cinco fichas estarán disponibles de forma predeterminada. Puede elegir el orden de las pestañas en la página global de Marketo

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-3.png)

**Límites**

* La actividad (momento interesante, actividad web, correo electrónico) se establece en 1000 de forma predeterminada. Las campañas de correo electrónico y los eventos están configurados en 200 de forma predeterminada
* Si observa problemas de tiempo de espera en su organización, puede reducir el límite

**Configuración de acción**

* Enviar correo electrónico a Marketo: si se activa, todos los usuarios de Perspectiva de ventas tendrán acceso para enviar correos electrónicos desde los paneles Posible cliente, Contacto, Cuenta, Oportunidad y la pestaña Resultados más probables (acciones masivas y participación en línea)
* Añadir a Marketo Campaign: si se activa, todos los usuarios de Perspectiva de ventas tendrán acceso para añadir a las campañas desde los paneles Posible cliente, Contacto, Cuenta, Oportunidad y Mejor opción (acciones masivas y participación en línea)

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-4.png)

## Configuración de soporte {#support-settings}

Si selecciona esta casilla, se habilitará el registro de depuración en la instancia de Salesforce. Puede ayudarle a solucionar problemas.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-5.png)

## Restablecer perspectiva de ventas de Marketo {#reset-marketo-sales-insight}

Si elige hacerlo, se borrarán todas las configuraciones en SFDC y no se podrán restaurar. Tendrá que volver a configurar todo.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-6.png)

>[!IMPORTANT]
>
>No active la casilla &quot;Activar acciones MSI&quot; a menos que esté utilizando las funciones de acciones de Sales Insights.

>[!MORELIKETHIS]
>
>[Añadir el acceso de Sales Insight a los perfiles](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-access-to-profiles.md){target="_blank"}
