---
description: Explicación de la sincronización de Veva - Marketo Docs - Documentación del producto
title: Explicación de la sincronización de Veva
hide: true
hidefromtoc: true
source-git-commit: c36b9206494c14a52937fa787a37601eaf6f4bd4
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Explicación de la sincronización de Veva {#understanding-the-veeva-sync}

En pocos pasos, es fácil ejecutar una sincronización entre Adobe Marketo Engage y Veeva CRM.

## Cómo funciona la sincronización {#how-the-sync-works}

El Marketo Engage se sincroniza con Veeva CRM todo el día, todos los días. Cada sincronización tarda un tiempo, se detiene durante 5 minutos y, a continuación, se inicia de nuevo.

>[!NOTE]
>
>La primera sincronización podría tardar horas o incluso días porque el Marketo Engage está copiando toda la base de datos de Veva. Después, cada sincronización suele tardar minutos (a veces segundos) y solo sincroniza los datos que han cambiado.

![](assets/understanding-the-veeva-sync-1.png)

La sincronización entre Veeva y el Marketo Engage solo es bidireccional para los campos Contacto en el objeto Cuenta de persona . En estos casos, cada vez que realice cambios en Veva o en el Marketo Engage, las actualizaciones se reflejarán en ambos sistemas. Todas las demás sincronizaciones son de Veva a Marketo Engage solamente. Haga clic en los vínculos siguientes para obtener detalles sobre cada uno.

## ¿Qué se sincroniza entre Marketo y Veva? {#what-is-synced-between-marketo-and-veeva}

Cuentas de persona Los usuarios llaman y llaman a objetos clave Objetos personalizados

## Aspectos importantes {#things-to-know}

* Las credenciales introducidas en el Marketo Engage de Veva se utilizan para sincronizar datos. Solo se incluirán los datos a los que tengan acceso esas credenciales.

* Veeva CRM se basa en force.com y el Marketo Engage de experiencias enriquecidas con la plataforma se hereda en esta sincronización.

* El CRM de Veva muestra: Posible cliente, Contacto, Cuentas (Cuentas comerciales, Oportunidad, Campaña y Actividad). Sin embargo, no son compatibles con la sincronización con el Marketo Engage.
