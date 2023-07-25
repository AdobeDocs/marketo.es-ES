---
unique-page-id: 14352546
description: Prevención de la integración de direcciones secundarias de Gmail con Sales Connect - Documentos de Marketo - Documentación del producto
title: Prevención de la integración de direcciones secundarias de Gmail con Sales Connect
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Prevención de la integración de direcciones secundarias de Gmail con Sales Connect {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Integración de Gmail rota (por qué mi Gmail personal envía correos electrónicos) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

La razón más común para una conexión de Gmail rota es una integración accidental con la cuenta personal de un usuario. Esto puede ocurrir cuando un usuario hace clic en &quot;Conectar&quot; o cuando intenta enviar un correo electrónico desde su cuenta personal. Esto puede resultar muy tentador, ya que la opción existirá al acceder a su cuenta de Gmail en la misma instancia de Chrome que el correo electrónico de trabajo.

## ¿Por qué Sales Connect siquiera intenta integrarse con mi Gmail personal? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

Sales Connect se integra con Gmail a través de una extensión instalada en el navegador Chrome. Siempre que la extensión detecta una instancia de Gmail abierta, ofrece una opción para integrarse con ella. Para evitar una integración con su cuenta personal de Gmail, le recomendamos una de las tres cosas...

Iniciar sesión como otro usuario de Chrome (recomendado)

Clic [este vínculo](https://support.google.com/chrome/answer/2364824?hl=en) para leer cómo crear otro perfil de Chrome.

**Pros**: al iniciar sesión como otro usuario, se abrirá una nueva instancia de Chrome. Esta instancia es una ventana nueva de Chrome y ninguna de las extensiones antiguas existirá en esta. También mantiene cookies para que no tenga que iniciar sesión en su Gmail cada vez.

**Contras**: Debe tener dos ventanas de Chrome abiertas.

Usar otro explorador

**Ventajas:** El uso de otro navegador de Internet (IE o Firefox) que no tenga la extensión instalada evitará que esto ocurra.

**Contras**: El uso de varios exploradores puede ser molesto.

Uso De Una Ventana De Incógnito

**Ventajas:** Una ventana de incógnito es como abrir una versión desnuda de Chrome. Esto significa que no tendrá ninguna de las extensiones instaladas y que Sales Connect no estará allí para conectarse.

**Contras**: Tendrá que iniciar sesión en Gmail cada vez que inicie su día y nuevamente si cierra la ventana accidentalmente.
