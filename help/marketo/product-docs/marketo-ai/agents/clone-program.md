---
description: Clone program duplica un programa de Marketo existente en una nueva carpeta con un nuevo nombre, conservando su estructura y permitiendo personalizar la nueva campaña.
title: Clonar programa
beta: true
hide: true
source-git-commit: f552c0b0219aede39e0742466ab2473e8e924e55
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# Clonar programa {#clone-program}

El agente de programa de clonación copia un programa de trabajo, incluidas sus campañas inteligentes, pasos de flujo, recursos de correo electrónico y configuración, en una nueva ubicación del entorno de Marketo.

>[!PREREQUISITES]
>
>* Para usar esta característica, primero debe aceptar los términos de [Core Gen-AI y los términos suplementarios](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.
>
>* Debe tener permiso para crear programas en la carpeta de destino.
>
>* El programa de origen que desea clonar ya debe existir en su entorno de Marketo.

## Cómo usar {#how-to-use}

1. En Mi Marketo, haga clic en el mosaico **Generar con IA**.

1. En la ventana de solicitud, escriba las instrucciones. Por ejemplo, &quot;Clone mi programa Seminario web del segundo trimestre en la carpeta Campañas del tercer trimestre y denomínelo Seminario web de demostración de producto del tercer trimestre&quot;.

1. Marketo AI confirma el programa de origen, la carpeta de destino y el nuevo nombre. Revise y confirme.

1. Se crea el clon. Marketo AI confirma cuándo se ha realizado y le indica dónde encontrarlo.

1. Abra el nuevo programa en Marketo y actualice lo que sea diferente: contenido de correo electrónico, fechas, filtros de audiencia, tokens, etc.

1. Ejecute el agente [Program QA](/help/marketo/product-docs/marketo-ai/agents/program-qa.md) antes de activarlo.

## Casos de uso {#use-cases}

**Reutilización de campañas trimestrales**: un administrador de campañas ejecuta la misma serie de seminarios web cada trimestre. Piden a Marketo AI que clone el programa de seminarios web del trimestre pasado en la carpeta del trimestre nuevo con un nombre actualizado. A continuación, actualizan la copia de correo electrónico, los tokens de fecha del seminario web y el vínculo de registro, lo que ahorra horas de tiempo de configuración.

**Creación de una plantilla a partir de un programa probado**: un especialista en operaciones de marketing clona un programa de lanzamiento de producto de alto rendimiento en una carpeta &quot;Plantillas&quot; para que sirva como punto de partida para lanzamientos futuros. El clon se deja desactivado y se utiliza como copia de referencia.

**Prueba A/B con un nuevo enfoque**: Un administrador de campaña quiere probar una cadencia de correo electrónico diferente sin cambiar un programa en ejecución. Clonan el programa activo, modifican los pasos de espera en el clon y activan ambos, ejecutándolos en diferentes segmentos de audiencia para comparar los resultados.

## Cosas que debe tener en cuenta {#things-to-note}

* Los programas clonados se crean en un estado desactivado. Nada se activa hasta que se activan las campañas inteligentes.
* Los recursos de correo electrónico del clon son copias, no se comparten con el original. Los cambios en los correos electrónicos del clon no afectarán al programa de origen.
* Los tokens utilizados en el programa de origen se copian en el clon. Sin embargo, deben actualizarse con nuevos valores (fechas, direcciones URL, nombres de eventos).
* Los filtros de campaña inteligente del clon hacen referencia a las mismas listas y campos que el original. Revise y actualice la segmentación de audiencia antes de activarla.
* Los recursos locales que hacen referencia a otros programas o listas compartidas se copian en el clon. Estas referencias deben revisarse antes de activarlas.
