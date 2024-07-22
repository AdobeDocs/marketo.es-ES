---
unique-page-id: 2951259
description: Glosario de tipos de campos personalizados - Documentos de Marketo - Documentación del producto
title: Glosario de tipo de campo personalizado
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 2%

---

# Glosario de tipo de campo personalizado {#custom-field-type-glossary}

Al crear un campo personalizado en Marketo, tiene una lista de tipos para elegir.

>[!PREREQUISITES]
>
>[Crear un campo personalizado en Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>Según el tipo de campo, el filtro o el déclencheur [operadores](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) serán diferentes.

>[!NOTE]
>
>La mayoría de los campos no alcanzan el máximo en el número de caracteres, sino en la cantidad de bytes. Por ello, no podemos proporcionar un límite de caracteres definitivo para cada campo. La excepción es **String**, que alcanza un máximo de 255 caracteres.

## Booleano {#boolean}

**Nombre de ejemplo:** es cliente: Etiquete a sus empleados como clientes

**Valores de ejemplo:** Verdadero (comprobado) / Falso (desmarcado)

**Operadores**: Ninguno

## Moneda {#currency}

**Nombre de ejemplo:** Presupuesto: almacena un valor numérico para el presupuesto de una compañía

**Valores de ejemplo:** 100

**Operadores**: es, no es, entre, mayor que, menor que, al menos, como máximo, está vacío, no está vacío

## Fecha {#date}

**Nombre de ejemplo:** Fecha de renovación - Almacena las fechas de renovación de tus clientes

**Valores de ejemplo:** 19/8/14

**Operadores**: es, no es, entre, en el pasado, en el pasado antes, en el futuro después, en el lapso de tiempo, después, antes, en o después, en o antes, está vacío, no está vacío

## Fecha y hora {#datetime}

**Nombre de ejemplo:** Fecha de creación: almacena la fecha y la hora en que se creó una persona

**Valores de ejemplo:** 19/8/14 2:00

**Operadores**: es, no es, entre, en el pasado, en el pasado antes, en el futuro después, en el lapso de tiempo, después, antes, en o después, en o antes, está vacío, no está vacío

## Correo electrónico {#email}

**Nombre de ejemplo:** Correo electrónico alternativo: mantenga una dirección de correo electrónico alternativa para sus recursos (en realidad no puede enviar correos electrónicos a este campo como el campo de dirección de correo electrónico predeterminado, ese campo es especial)

**Valores de ejemplo:** name@company.com

**Operadores**: es, no es, empieza por, no empieza por, contiene, no contiene, está vacío, no está vacío

## Flotante {#float}

**Nombre de ejemplo:** Promedio de punto de calificación: mantenga el promedio de punto de calificación de una persona o cualquier otro valor numérico que tenga decimales

**Valores de ejemplo:** 2.47

**Operadores**: entre, mayor que, menor que, como mínimo, está vacío, no está vacío

## Fórmula {#formula}

**Nombre de ejemplo:** Saludos - use este campo especial en una [solución para obtener el saludo correcto](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) basado en el género

**Valores de ejemplo:** compruebe la solución vinculada

## Entero {#integer}

**Nombre de ejemplo:** Número de empleados: almacene un valor numérico que no requiera decimales

**Valores de ejemplo:** 600

**Operadores**: es, no es, entre, mayor que, menor que, al menos, como máximo, está vacío, no está vacío

## Porcentaje {#percent}

**Nombre de ejemplo:** con probabilidad de comprar: almacene un valor porcentual (tal vez calculado en el lado del CRM).

**Valores de ejemplo:** 85%

**Operadores**: es, no es, entre, mayor que, menor que, al menos, como máximo, está vacío, no está vacío

## Teléfono {#phone}

**Nombre de ejemplo:** Teléfono alternativo: almacena un número de teléfono adicional para tus empleados

**Valor de ejemplo:** 650-555-5555

**Operadores**: es, no es, empieza por, no empieza por, contiene, no contiene, está vacío, no está vacío

## Puntaje {#score}

**Nombre de ejemplo:** Puntuación de comportamiento/Puntuación demográfica: cree varios campos de puntuación para realizar un seguimiento de atributos diferentes

**Valor de ejemplo:** 14

**Operadores**: es, no es, entre, mayor que, menor que, al menos, como máximo, está vacío, no está vacío

## Cadena {#string}

**Nombre de ejemplo:** Segundo nombre: almacene un atributo de texto adicional

**Valor de ejemplo:** Rose

**Operadores**: es, no es, empieza por, no empieza por, contiene, no contiene, está vacío, no está vacío

## Área de texto {#text-area}

**Nombre de ejemplo:** Comentarios: agregue un campo de comentarios a los formularios para permitir la entrada de texto multilínea

**Valor de ejemplo:** Este artículo es fantástico.

**Operadores**: es, no es, empieza por, no empieza por, contiene, no contiene, está vacío, no está vacío

## URL {#url}

**Nombre de ejemplo:** blog: cree un campo para almacenar las direcciones URL del blog de la persona

**Valor de ejemplo:** www.myblog.com

**Operadores**: es, no es, empieza por, no empieza por, contiene, no contiene, está vacío, no está vacío
