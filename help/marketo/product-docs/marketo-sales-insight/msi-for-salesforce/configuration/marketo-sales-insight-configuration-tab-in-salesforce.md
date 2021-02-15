---
unique-page-id: 42762322
description: Ficha Configuración de perspectiva de ventas de marketing en Salesforce - Documentos de marketing - Documentación del producto
title: Ficha Configuración de perspectiva de ventas de marketing en Salesforce
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---


# Ficha Configuración de perspectiva de ventas de marketing en Salesforce {#marketo-sales-insight-configuration-tab-in-salesforce}

## Configuración operativa {#operational-settings}

Deberá tener esta configuración para poder realizar inicios mediante Sales Insight en SFDC.

![](assets/one.png)

* MSI utiliza la API Soap y Rest
* La página de perspectiva de ventas de su cuenta de Marketing tendrá dos paneles correspondientes con credenciales de API de Soap y Rest que puede copiar y pegar aquí
* La API de Soap y Rest tiene tiempos de espera separados que puede establecer en función de las necesidades de su organización. El tiempo máximo permitido es de 120 segundos
* Desactivación del Panel de perspectivas: Puede eliminar las credenciales de la API de descanso y utilizar únicamente la API de Soap. Al hacerlo, se desactivará la ficha Panel de perspectivas en todos los paneles de fuerza visual MSI

## Configuración de MSI {#msi-configuration}

Las configuraciones se aplican a todos los usuarios de MSI y no son específicas de los perfiles.

**Configuración de la ficha Marcado**

* Mejor modo de depuración de apuestas
* Ocultar predeterminado: La opción que elija aquí será el número de días que se ocultará una mejor apuesta en la ficha Mejores apuestas de Marketing cuando haga clic en el icono &quot;Ocultar&quot;
* Campo de estado de contacto: la opción que elija aquí será el valor que se rellene en la columna Encabezado de estado de la ficha Mejores apuestas de Marketing
* Configuración de tabulación: las 5 fichas estarán disponibles de forma predeterminada. Puede elegir el orden de las fichas en la página global de Marketing to

**Configuración de página de VisualForce**

* Habilitar la lista desplegable Acción:

   * Posibilidad de ocultar el mensaje de correo electrónico de Enviar marketing de la lista desplegable en Diseño de posibles clientes y contactos MSI
   * Posibilidad de ocultar las opciones de Añadir a la Campaña de marketing desde la lista desplegable en Diseño de posibles clientes y contactos MSI

* Próximos eventos: Capacidad para mostrar eventos invitados, todos los eventos a los usuarios u ocultar completamente esta ficha
* Próximas campañas: Posibilidad de mostrar todas las campañas de correo electrónico u ocultar completamente esta ficha
* Configuración de tabulación: las 5 fichas estarán disponibles de forma predeterminada. Las 5 fichas estarán disponibles de forma predeterminada. Puede elegir el orden de las fichas en el panel de perspectiva de ventas. El mismo pedido se aplicará a todo el diseño (posible cliente, contacto, cuenta, oportunidad)

![](assets/two.png)

**Límites**

* La actividad (Momento interesante, Actividad Web, Correo electrónico) se establece en 1000 de forma predeterminada. Las campañas y Eventos de correo electrónico están configuradas en 200 de forma predeterminada
* Si nota problemas de tiempo de espera en su organización, puede reducir el límite

## Restablecer perspectiva de ventas de marketing {#reset-marketo-sales-insight}

Si elige hacerlo, borrará todas las configuraciones de SFDC y no se podrán restaurar. Tendrá que volver a configurar todo de nuevo.

![](assets/three.png)
