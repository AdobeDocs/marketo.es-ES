---
unique-page-id: 14352475
description: Instalación de los campos de eventos de Sales Connect en el historial de actividades - Documentos de Marketo - Documentación del producto
title: Instalación de campos de eventos de conexión de ventas en el historial de actividades
exl-id: c1bdb5a6-04f0-4579-84b6-33f4a301128f
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Instalación de campos de eventos de conexión de ventas en el historial de actividades {#install-sales-connect-event-fields-on-activity-history}

Una vez que haya instalado el paquete Enterprise en Salesforce, puede instalar los campos de evento de Conexión de ventas en la sección del historial de actividades. Los campos de eventos de Conexión de ventas incluyen información como vistas, clics y campañas. Esto le permite tener información sobre los correos electrónicos importados directamente en Salesforce.

Asegúrese de formar un equipo con el administrador de Salesforce al realizar estos pasos. En este ejemplo, instalaremos los campos en la **Diseño de página de posibles clientes**. También puede instalar los campos en los diseños de página de contacto, cuenta y oportunidad. Recuerde, al registrar correos electrónicos en Cuentas y oportunidades, necesitará el contacto al que está enviando correo electrónico asociado como función de contacto.

1. Clic **Configurar**.
1. Clic **Personalizar**.
1. Clic **Posibles clientes**.
1. Clic **Diseños de página**.
1. Clic **Editar** situado junto al diseño de página que desee cambiar.

   >[!NOTE]
   >
   >Sales Connect instalará algunos diseños de página, pero si ya dispone de uno predeterminado que esté utilizando su equipo, deberá instalarlo allí. Puede eliminar los diseños de página de Conexión de ventas si no desea utilizarlos.

1. Desplácese hacia abajo hasta la sección Historial de actividades.
1. Haga clic en la llave inglesa para editarla.
1. Seleccione los campos de Conexión de ventas que desee incluir en la sección Historial de actividades. Si no ve los campos de Sales Connect aquí, es posible que haya instalado el paquete incorrecto de Salesforce.
1. Clic **Añadir** para mover los campos deseados.
1. Clic **OK**.
1. Clic **Guardar**.

   Los usuarios ahora pueden ver información valiosa y actualizaciones sobre sus correos electrónicos en Salesforce.
