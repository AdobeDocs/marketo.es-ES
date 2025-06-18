---
solution: Marketo Engage
product: marketo
title: Spam Assassin
description: EL TEXTO VA AQUÍ
level: Beginner, Intermediate
feature: Email Editor
hide: true
hidefromtoc: true
source-git-commit: 0157bc64444151a43bf464158d508e84d75b3427
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 3%

---

# Spam Assassin {#spam-assassin}

Con SpamAssassin en Marketo Engage, puede probar el contenido del correo electrónico y ver la probabilidad de que los ISP/proveedores de buzones de correo lo marquen como correo no deseado.

SpamAssassin analiza el contenido y asigna una puntuación basada en distintos criterios. Cuanto más baja sea la puntuación, mejor. Es importante mantener una puntuación baja, ya que el envío de correos electrónicos con una puntuación alta puede afectar negativamente a la capacidad de envío general.

## Acceso al informe de spam {#access-the-spam-report}

1. En la pantalla Simular, haga clic en el botón **Informe de spam**.

CAPTURA DE PANTALLA

1. Se genera un informe de spam.

CAPTURA DE PANTALLA

1. Compruebe las puntuaciones y descripciones de cada elemento.

>[!IMPORTANT]
>
>Si la puntuación general es mayor de 5, el correo electrónico puede bloquearse o marcarse como correo no deseado durante la entrega.

1. Si considera que la puntuación es demasiado alta, edite el contenido en el Designer de correo electrónico y, a continuación, vuelva a ejecutar el informe de correo no deseado hasta que la puntuación esté donde desea que esté.

CAPTURA DE PANTALLA

>[!NOTE]
>
>La puntuación de spam se deriva mediante SpamAssassin y las reglas no son propiedad de Adobe. Encontrará más detalles sobre estas reglas en la [documentación de SpamAssassin](https://spamassassin.apache.org/#_blank). Se puede ver una lista completa de errores [aquí](https://spamassassin.apache.org/old/tests_3_0_x.html?utm_source=chatgpt.com).
