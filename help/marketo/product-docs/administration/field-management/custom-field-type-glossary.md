---
unique-page-id: 2951259
description: Glosario de tipo de campo personalizado - Documentos de Marketo - Documentación del producto
title: Glosario de tipo de campo personalizado
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# Glosario de tipo de campo personalizado {#custom-field-type-glossary}

Al crear un campo personalizado en Marketo, tiene una lista de tipos para elegir.

>[!PREREQUISITES]
>
>[Crear un campo personalizado en Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>Según el tipo de campo, los operadores [filter/déclencheur](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) serán diferentes.

>[!NOTE]
>
>La mayoría de los campos no superan el límite en el número de caracteres, sino en la cantidad de bytes. Debido a esto, no podemos proporcionar un límite de caracteres definitivo para cada campo. La excepción es **String**, que tiene un máximo de 255 caracteres.

## Booleano {#boolean}

**Nombre de ejemplo:** Es cliente: Etiquete a sus personas como clientes

**Valores de ejemplo:** True (marcado) / False (sin marcar)

**Operadores**: Ninguna

## Moneda {#currency}

**Nombre de ejemplo:** Presupuesto: Almacenar un valor numérico para el presupuesto de una empresa

**Valores de ejemplo:** 100

**Operadores**: es, no es, entre, bueno que, menor que, al menos, que está vacío, no está vacío

## Fecha {#date}

**Nombre de ejemplo:** Fecha de renovación: Almacene las fechas de renovación de los clientes

**Valores de ejemplo:** 19/8/14

**Operadores**: es, no es, entre, en el pasado antes, en el futuro, en el futuro después, en el lapso de tiempo, después, antes, en o después, en o antes de está vacío, no está vacío

## Datetime {#datetime}

**Nombre de ejemplo:** Fecha de creación: Almacene la fecha y la hora en que se crea una persona

**Valores de ejemplo:** 19/8/14 2:00

**Operadores**: es, no es, entre, en el pasado antes, en el futuro, en el futuro después, en el lapso de tiempo, después, antes, en o después, en o antes de está vacío, no está vacío

## Correo electrónico {#email}

**Nombre de ejemplo:** Correo electrónico alternativo: mantenga una dirección de correo electrónico alternativa para sus personas (en realidad no puede enviar correos electrónicos a este campo como el campo de dirección de correo electrónico predeterminado, que es especial)

**Valores de ejemplo:** name@company.com

**Operadores**: es, no es, empieza por, no comienza por, contiene, no contiene, está vacío, no está vacío

## Flotante {#float}

**Nombre de ejemplo:** Promedio de punto de graduación: mantenga el promedio de punto de graduación de una persona o cualquier otro valor numérico que tenga decimales

**Valores de ejemplo:** 2.47

**Operadores**: entre, bueno que, al menos que, como máximo, esté vacío, no esté vacío

## Fórmula {#formula}

**Nombre de ejemplo:** Saludos. Utilice este campo especial en una  [solución para obtener la ](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) fórmula correcta según el sexo

**Valores de ejemplo:** comprobar la solución vinculada

## Número entero {#integer}

**Nombre de ejemplo:** Número de empleados: almacene un valor numérico que no requiera decimales

**Valores de ejemplo:** 600

**Operadores**: es, no es, entre, bueno que, menor que, al menos, que está vacío, no está vacío

## Porcentaje {#percent}

**Nombre de ejemplo:** Es probable que lo compre: almacene un valor de porcentaje (tal vez calculado en el lado de CRM)

**Valores de ejemplo:** 85%

**Operadores**: es, no es, entre, bueno que, menor que, al menos, que está vacío, no está vacío

## Teléfono {#phone}

**Nombre de ejemplo:** Teléfono alternativo: almacene un número de teléfono adicional para sus usuarios

**Valor de ejemplo:** 650-555-5555

**Operadores**: es, no es, empieza por, no comienza por, contiene, no contiene, está vacío, no está vacío

## Puntuación {#score}

**Nombre de ejemplo:** Puntuación de comportamiento / Puntuación demográfica: cree varios campos de puntuación para realizar un seguimiento de los distintos atributos.

**Valor de ejemplo:** 14

**Operadores**: es, no es, entre, bueno que, menor que, al menos, que está vacío, no está vacío

## Cadena {#string}

**Nombre de ejemplo:** Nombre central: almacene un atributo de texto adicional

**Valor de ejemplo:** Rose

**Operadores**: es, no es, empieza por, no comienza por, contiene, no contiene, está vacío, no está vacío

## Área de texto {#text-area}

**Nombre de ejemplo:** Comentarios: agregue un campo de comentarios a los formularios para permitir la entrada de texto multilínea

**Valor de ejemplo:** este artículo es fantástico.

**Operadores**: es, no es, empieza por, no comienza por, contiene, no contiene, está vacío, no está vacío

## URL {#url}

**Nombre de ejemplo:** Blog: cree un campo para almacenar direcciones url de blog de personas

**Valor de ejemplo:** www.myblog.com

**Operadores**: es, no es, empieza por, no comienza por, contiene, no contiene, está vacío, no está vacío
