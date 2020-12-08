---
unique-page-id: 7514126
description: Ejemplo de atribución 1 - Documentos de marketing - Documentación del producto
title: Ejemplo de atribución 1
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# Ejemplo de atribución 1 {#attribution-example}

Lea el siguiente escenario e intente determinar los números que deben estar en la cuadrícula.

* 11 de abril | Fred es adquirido por (feria comercial)
* 15 de abril | Asistentes a Margo (seminario web): éxito
* 22 de abril | Fred está asociado (rol) a la oportunidad
* 22 de abril | Se crea una oportunidad por 3.000 dólares

| Nombre del programa | (Exposición comercial) | (Seminario web) |
|---|---|---|
| (FT) Opción creada | `<pre>1</pre>` | `<pre>0</pre>` |
| Canalización creada (FT) | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT) Opty Won | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT) Ingresos obtenidos | `<pre>0</pre>` | `<pre>0</pre>` |

**Mostrar respuestas**

>[!NOTE]
>
>**Explicación**
>
>Primero es entender que algunos tipos son RECUENTOS y otros son MONEDAS. La opción Creada es un recuento, un entero. La canalización es una moneda. En Marketing Cloud, la moneda se ajustará a la configuración regional de administración.
>
>La razón por la que la feria recibió todo el crédito es porque Margo no estaba asociado con un rol en la oportunidad. Sin papel, sin crédito.

>[!NOTE]
>
>**Reglas de atribución**
>
>1. El crédito se divide equitativamente
>1. No puedes dar más crédito del que ganaste
>1. No puedes dar crédito por algo que pasó en el pasado


Pruebe todos los ejemplos y usted será un profesional de atribución!

>[!NOTE]
>
>**Artículos relacionados**
>
>* [Ejemplo de atribución 2](attribution-example-2.md)
>* [Ejemplo de atribución 3](attribution-example-3.md)
>* [Ejemplo de atribución 4](attribution-example-4.md)

