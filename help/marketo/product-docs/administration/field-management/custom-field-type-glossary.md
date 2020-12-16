---
unique-page-id: 2951259
description: Glosario de tipo de campo personalizado - Documentos de marketing - Documentación del producto
title: Glosario de tipo de campo personalizado
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '606'
ht-degree: 0%

---


# Glosario de tipo de campo personalizado {#custom-field-type-glossary}

Al crear un campo personalizado en Marketing, tiene una lista de tipos para elegir.

>[!PREREQUISITES]
>
>* [Creación de un campo personalizado en Marketing](create-a-custom-field-in-marketo.md)

>



>[!TIP]
>
>En función del tipo de campo, [los operadores](https://docs.marketo.com/display/public/DOCS/Smart+List+Filter+Operators+Glossary) de filtro/activador serán diferentes.

>[!NOTE]
>
>La mayoría de los campos no llegan al máximo en el número de caracteres, sino en la cantidad de bytes. Debido a esto, no podemos proporcionar un límite de caracteres definitivo para cada campo. La excepción es **String**, que tiene un máximo de 255 caracteres.

## Booleano {#boolean}

**Nombre de ejemplo:** Es cliente: etiquete a sus personas como clientes

**Valores de ejemplo:** Verdadero (marcado) / Falso (sin marcar)

**Operadores**: Ninguno

## Moneda {#currency}

**Nombre de ejemplo:** Presupuesto: Almacene un valor numérico para el presupuesto de una compañía

**Valores de ejemplo:** 100

**Operadores**: es, no es, entre, bueno que, por lo menos que, como máximo, está vacío, no está vacío

## Fecha {#date}

**Nombre de ejemplo:** Fecha de renovación: almacene las fechas de renovación de los clientes

**Valores de ejemplo:** 19/8/14

**Operadores**: es, no está, entre, en el pasado, antes, en el futuro, después, en el marco de tiempo, después, antes, en o después, en o antes de que esté vacío, no está vacío

## Datetime {#datetime}

**Nombre de ejemplo:** Fecha de creación: almacene la fecha y la hora en que se crea una persona

**Valores de ejemplo:** 19/8/14 2:00

**Operadores**: es, no está, entre, en el pasado, antes, en el futuro, después, en el marco de tiempo, después, antes, en o después, en o antes de que esté vacío, no está vacío

## Correo electrónico {#email}

**Nombre de ejemplo:** Correo electrónico alternativo: mantenga una dirección de correo electrónico alternativa para sus usuarios (en realidad no puede enviar correos electrónicos a este campo como el campo de dirección de correo electrónico predeterminada, que es especial)

**Valores de ejemplo:** [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#335d525e5673505c5e43525d4a1d505c5e)

**Operadores**: es, no es, inicios con, no inicios con, contiene, no contiene, está vacío, no está vacío

## Flotante {#float}

**Nombre de ejemplo:** Promedio de punto de grado: mantenga la media del punto de grado de una persona o cualquier otro valor numérico que tenga decimales

**Valores de ejemplo:** 2,47

**Operadores**: entre, bueno que, por lo menos, menos de, como máximo, está vacío, no está vacío

## Fórmula {#formula}

**Nombre de ejemplo:** Saludos - utilice este campo especial en una [solución para obtener el saludo](create-and-use-a-concatenated-string-formula-field.md) correcto en función del género

**Valores de ejemplo:** comprobar la solución vinculada

## Entero {#integer}

**Nombre de ejemplo:** Número de empleados: almacene un valor numérico que no requiera decimales

**Valores de ejemplo:** 600

**Operadores**: es, no es, entre, bueno que, por lo menos que, como máximo, está vacío, no está vacío

## Porcentaje {#percent}

**Nombre de ejemplo:** Posibilidad de compra: almacene un valor de porcentaje (tal vez calculado en el lado de CRM)

**Valores de ejemplo:** 85 %

**Operadores**: es, no es, entre, bueno que, por lo menos que, como máximo, está vacío, no está vacío

## Teléfono {#phone}

**Nombre de ejemplo:** Teléfono alternativo: almacene un número de teléfono adicional para sus usuarios

**Valor de ejemplo:** 650-555-555

**Operadores**: es, no es, inicios con, no inicios con, contiene, no contiene, está vacío, no está vacío

## Puntuación {#score}

**Nombre de ejemplo:** Puntuación demográfica/puntuación de comportamiento: cree varios campos de puntuación para realizar un seguimiento de los distintos atributos.

**Valor de ejemplo:** 14

**Operadores**: es, no es, entre, bueno que, por lo menos que, como máximo, está vacío, no está vacío

## Cadena {#string}

**Nombre de ejemplo:** Nombre central: almacenar un atributo de texto adicional

**Valor de ejemplo:** Rosa

**Operadores**: es, no es, inicios con, no inicios con, contiene, no contiene, está vacío, no está vacío

## Área de texto {#text-area}

**Nombre de ejemplo:** Comentarios: agregue un campo de comentarios a los formularios para permitir la entrada de texto multilínea

**Valor de ejemplo:** ¡Este artículo es fantástico!

**Operadores**: es, no es, inicios con, no inicios con, contiene, no contiene, está vacío, no está vacío

## URL {#url}

**Nombre de ejemplo:** Blog: cree un campo para almacenar direcciones URL del blog de personas

**Valor de ejemplo:** www.myblog.com

**Operadores**: es, no es, inicios con, no inicios con, contiene, no contiene, está vacío, no está vacío
