---
unique-page-id: 10096409
description: 'Evitar el envío de contenido duplicado: Documentos de Marketo: Documentación del producto'
title: Evitar enviar contenido duplicado
exl-id: fd7118e8-6e34-4973-8aa5-effb774447fd
source-git-commit: daaf3dc9b4da95db743409c6e2a6c426ed00e9c7
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 3%

---

# Evitar enviar contenido duplicado {#avoid-sending-duplicate-content}

¿Alguna vez has recibido el mismo correo electrónico dos veces? Molesto, ¿no?

A continuación se presentan siete escenarios y resultados posibles que deben tenerse en cuenta para evitar enviar a alguien el mismo mensaje dos veces con programas de participación.

## Situaciones {#scenarios}

| El correo electrónico se envía desde | La persona es | La persona recibe el correo electrónico |
|---|---|---|
| Una campaña en un programa separado, independiente y predeterminado | No es miembro del programa predeterminado | Sí |
| Una campaña en un programa separado, independiente y predeterminado | Un miembro del programa predeterminado | No |
| Campaña dentro de un programa predeterminado que se activa desde una emisión dentro de la función **same** Programa CEE | Un miembro del programa predeterminado | No |
| Campaña dentro de un programa predeterminado que se activa desde una emisión dentro de la función **same** Programa CEE | No es miembro del programa predeterminado | Sí |
| Campaña dentro de un programa predeterminado que se activa desde una emisión dentro de una **different** Programa CEE | Un miembro del programa predeterminado | No |
| Campaña dentro de un programa predeterminado que se activa desde una emisión dentro de una **different** Programa CEE | No es miembro del programa predeterminado | Sí |
| A **different** Programa CEE que utiliza un flujo inteligente | Miembro de ambos programas de Europa central y oriental | No |
