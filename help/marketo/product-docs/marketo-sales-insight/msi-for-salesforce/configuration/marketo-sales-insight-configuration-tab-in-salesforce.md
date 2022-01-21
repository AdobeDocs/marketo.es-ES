---
unique-page-id: 42762322
description: Pestaña Configuración de la perspectiva de ventas de Marketo en Salesforce - Documentos de Marketo - Documentación del producto
title: Pestaña Configuración de Marketo Sales Insight en Salesforce
exl-id: 4e2abd48-b0a5-4b71-939b-e66c7e39bb6c
source-git-commit: 15263f9c23c958499aaa2e4e6491b4962c617358
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# Pestaña Configuración de Marketo Sales Insight en Salesforce {#marketo-sales-insight-configuration-tab-in-salesforce}

## Configuración operativa {#operational-settings}

Deberá tener esto configurado para empezar a usar Sales Insight en SFDC.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-1.png)

* MSI utiliza la API de Soap y Rest
* La página Perspectiva de ventas de su cuenta de Marketo tendrá dos paneles correspondientes con credenciales de API Soap y Rest que puede copiar y pegar aquí
* La API de Soap y Rest tiene tiempos de espera separados que puede establecer en función de las necesidades de su organización. El tiempo máximo permitido es de 120 segundos
* Desactivación del panel de perspectivas: Puede eliminar las credenciales de la API de Rest y usar solo la API de Soap. Al hacerlo, se deshabilitará la ficha Panel de perspectivas en todos los paneles de fuerza visual de MSI

## Configuración de MSI {#msi-configuration}

Las configuraciones se aplican a todos los usuarios de MSI y no son específicas de los perfiles.

**Configuración de página de Visualización**

* Habilitar lista desplegable de acción:
   * Posibilidad de ocultar Enviar correo electrónico de Marketo de la lista desplegable en Diseño de posible cliente y contacto MSI
   * Posibilidad de ocultar las opciones de Agregar a Marketo Campaign de la lista desplegable en Diseño de posible cliente y contacto MSI
* Próximos eventos: Posibilidad de mostrar eventos invitados, todos los eventos a los usuarios u ocultar completamente esta pestaña
* Próximas campañas: Capacidad para mostrar todas las campañas de correo electrónico u ocultar completamente esta pestaña
* Cargar campañas y eventos futuros: Capacidad para reducir el número de llamadas a la API Rest realizadas por los usuarios colocando eventos y campañas detrás de un botón &quot;Cargar elementos próximos&quot; bajo demanda
* Configuración de pestañas: Las cinco pestañas estarán disponibles de forma predeterminada. Puede elegir el orden de las pestañas en el panel Perspectiva de ventas . El mismo orden se aplicará a todos los diseños (posible cliente, contacto, cuenta, oportunidad)

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-2.png)

**Ficha Global de Marketo**

* Fuente RSS habilitada: Cuando está habilitado, los usuarios de MSI pueden ver su Fuente de posibles clientes en una fuente RSS (además de la Fuente de posibles clientes en Salesforce). La fuente RSS solo puede funcionar si la función &quot;Caducidad del token&quot; está desactivada. Esta configuración se controla en la página Administración de perspectivas de ventas de Marketo.
* Mejor modo de depuración
* Ocultar predeterminado: La opción que elija aquí será el número de días que la mejor apuesta se ocultará en la ficha Mejores apuestas de Marketo cuando haga clic en el icono &quot;Ocultar&quot;
* Campo Estado de contacto: La opción que elija aquí es el valor que se rellena en la columna Encabezado de estado de la ficha Mejores apuestas de Marketo
* Configuración de la fuente en directo: La opción para mostrar solo la fuente en directo (en los paneles Posible cliente, Contacto, Cuenta y Oportunidad y la página de Marketo global), solo la fuente de posibles clientes (en la página global de Marketo) o ambas, en directo y la fuente de posibles clientes
* Configuración de pestañas: Las cinco pestañas estarán disponibles de forma predeterminada. Puede elegir el orden de las pestañas en la página global de Marketo

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-3.png)

**Límites**

* Actividad (Momento interesante, Actividad web, Correo electrónico) está configurada en 1000 de forma predeterminada. Las campañas de correo electrónico y los eventos están establecidos en 200 de forma predeterminada
* Si nota problemas de tiempo de espera en su organización, puede reducir el límite

**Configuración de la acción**

* Enviar correo electrónico de Marketo: Al habilitar esto, todos los usuarios de Sales Insight tendrán acceso para enviar correos electrónicos desde los paneles Posible cliente, Contacto, Cuenta, Oportunidad y Mejor apuesta (acciones masivas y participación en línea)
* Añadir a Marketo Campaign: Al habilitar esto, todos los usuarios de Perspectiva de ventas tendrán acceso para agregar campañas desde los paneles Posible cliente, Contacto, Cuenta, Oportunidad y Mejor apuesta (acciones masivas y participación en línea)

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-4.png)

## Restablecer la perspectiva de ventas de Marketo {#reset-marketo-sales-insight}

Si elige hacerlo, se borrarán todas las configuraciones en SFDC y no se podrán restaurar. Tendrá que volver a configurar todo de nuevo.

![](assets/marketo-sales-insight-configuration-tab-in-salesforce-5.png)

>[!MORELIKETHIS]
>
>[Configuración de la perspectiva de ventas para su equipo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md)
