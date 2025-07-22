---
unique-page-id: 14352546
description: Prevención de la integración de direcciones secundarias de Gmail con Sales Connect - Documentos de Marketo - Documentación del producto
title: Prevención de la integración de direcciones secundarias de Gmail con Sales Connect
exl-id: a84fe53b-0ec8-400c-8747-be496c68a8e3
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Impedir que la dirección secundaria de Gmail se integre con [!DNL Sales Connect] {#preventing-secondary-gmail-address-from-integrating-with-sales-connect}

## Integración de Gmail rota (por qué mi Gmail personal envía correos electrónicos) {#broken-gmail-integration-why-is-my-personal-gmail-sending-emails}

La razón más común para una conexión de Gmail rota es una integración accidental con la cuenta personal de un usuario. Esto puede ocurrir cuando un usuario hace clic en &quot;Conectar&quot; o cuando intenta enviar un correo electrónico desde su cuenta personal. Esto puede ser muy tentador porque la opción existirá al acceder a su cuenta de Gmail en la misma instancia de [!DNL Chrome] que su correo electrónico de trabajo.

## ¿Por qué [!DNL Sales Connect] siquiera intenta integrarse con mi Gmail personal? {#why-does-sales-connect-even-try-to-integrate-with-my-personal-gmail}

[!DNL Sales Connect] se integra con Gmail a través de una extensión instalada en el explorador [!DNL Chrome]. Siempre que la extensión detecta una instancia de Gmail abierta, ofrece una opción para integrarse con ella. Para evitar una integración con su cuenta personal de Gmail, le recomendamos una de las tres cosas...

Iniciar Sesión Como Otro [!DNL Chrome]Usuario (Recomendado)

Haga clic en [este vínculo](https://support.google.com/chrome/answer/2364824?hl=en) para leer cómo crear otro [!DNL Chrome]perfil.

**Profesionales**: Iniciar sesión como otro usuario abrirá una nueva instancia de [!DNL Chrome]. Esta instancia es una ventana completamente nueva de [!DNL Chrome] y ninguna de las extensiones antiguas existirá en esta. También mantiene cookies para que no tenga que iniciar sesión en su Gmail cada vez.

**Desventajas**: Debe tener dos ventanas de [!DNL Chrome]abiertas.

Usar otro explorador

**Ventajas:** Usar otro navegador de Internet (IE o Firefox) que no tenga instalada la extensión evitará que esto ocurra.

**Desventajas**: Usar varios exploradores puede ser molesto.

Uso De Una Ventana De Incógnito

**Ventajas:** Una ventana de incógnito es como abrir una versión desnuda de [!DNL Chrome]. Esto significa que no tendrá ninguna de las extensiones instaladas y [!DNL Sales Connect] no estará allí para conectarse.

**Desventajas**: Tendrás que iniciar sesión en Gmail cada vez que empieces el día y de nuevo si cierras la ventana accidentalmente.
