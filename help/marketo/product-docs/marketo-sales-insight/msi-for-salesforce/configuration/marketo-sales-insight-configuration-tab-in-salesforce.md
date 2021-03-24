---
unique-page-id: 42762322
description: Pestaña Configuración de Marketo Sales Insight en Salesforce - Marketo Docs - Documentación del producto
title: Pestaña Configuración de Marketo Sales Insight en Salesforce
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---


# Pestaña Configuración de Marketo Sales Insight en Salesforce {#marketo-sales-insight-configuration-tab-in-salesforce}

## Configuración operativa {#operational-settings}

Deberá tener esto configurado para empezar a usar Sales Insight en SFDC.

![](assets/one.png)

* MSI utiliza la API de Soap y Rest
* La página Perspectiva de ventas de su cuenta de Marketo tendrá dos paneles correspondientes con credenciales de API Soap y Rest que puede copiar y pegar aquí
* La API de Soap y Rest tiene tiempos de espera separados que puede establecer en función de las necesidades de su organización. El tiempo máximo permitido es de 120 segundos
* Desactivación del panel de perspectivas: Puede eliminar las credenciales de la API de Rest y usar solo la API de Soap. Al hacerlo, se deshabilitará la ficha Panel de perspectivas en todos los paneles de fuerza visual de MSI

## Configuración de MSI {#msi-configuration}

Las configuraciones se aplican a todos los usuarios de MSI y no son específicas de los perfiles.

**Configuración de la ficha Marketo**

* Mejor modo de depuración
* Ocultar predeterminado : la opción que elija aquí será el número de días que la mejor apuesta estará oculta en la ficha Mejores apuestas de Marketo cuando haga clic en el icono &quot;Ocultar&quot;
* Campo Estado de Contacto : la opción que elija aquí es el valor que se rellena en la columna Encabezado de Estado de la ficha Mejores apuestas de Marketo.
* Configuración de pestañas : las 5 pestañas estarán disponibles de forma predeterminada. Puede elegir el orden de las pestañas en la página global de Marketo

**Configuración de página de Visualización**

* Habilitar lista desplegable de acción:

   * Posibilidad de ocultar Enviar correo electrónico de Marketo de la lista desplegable en Diseño de posible cliente y contacto MSI
   * Posibilidad de ocultar las opciones de Agregar a campaña de Marketo de la lista desplegable Diseño de posible cliente y contacto MSI

* Próximos eventos: Posibilidad de mostrar eventos invitados, todos los eventos a los usuarios u ocultar completamente esta pestaña
* Próximas campañas: Capacidad para mostrar todas las campañas de correo electrónico u ocultar completamente esta pestaña
* Cargar campañas y eventos futuros: Capacidad para reducir el número de llamadas a la API Rest realizadas por los usuarios colocando eventos y campañas detrás de un botón &quot;Cargar elementos próximos&quot; bajo demanda
* Configuración de pestañas : las 5 pestañas estarán disponibles de forma predeterminada. Las 5 pestañas estarán disponibles de forma predeterminada. Puede elegir el orden de las pestañas en el panel Perspectiva de ventas . El mismo orden se aplicará a todo el diseño (posible cliente, contacto, cuenta, oportunidad)

![](assets/two.png)

**Límites**

* Actividad (Momento interesante, Actividad web, Correo electrónico) está configurada en 1000 de forma predeterminada. Las campañas de correo electrónico y los eventos están establecidos en 200 de forma predeterminada
* Si nota problemas de tiempo de espera en su organización, puede reducir el límite

## Restablecer la perspectiva de ventas de Marketo {#reset-marketo-sales-insight}

Si elige hacerlo, se borrarán todas las configuraciones en SFDC y no se podrán restaurar. Tendrá que volver a configurar todo de nuevo.

![](assets/three.png)

>[!MORELIKETHIS]
>
>[Configuración de la perspectiva de ventas para su equipo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/setting-up-sales-insight-for-your-team.md)
