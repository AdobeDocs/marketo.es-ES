---
unique-page-id: 2951259
description: Glosario de tipos de campos personalizados - Documentos de Marketo - Documentación del producto
title: Glosario de tipo de campo personalizado
exl-id: 495d4deb-28f1-4044-98d3-27c20756fe73
source-git-commit: 20c41143d1e7839352dddbfea0951c2633987692
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 2%

---

# Glosario de tipo de campo personalizado {#custom-field-type-glossary}

Al crear un campo personalizado en Marketo, tiene una lista de tipos para elegir.

>[!PREREQUISITES]
>
>[Creación de un campo personalizado en Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

>[!TIP]
>
>Según el tipo de campo, filtro/déclencheur [operadores](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/smart-list-filter-operators-glossary.md) será diferente.

>[!NOTE]
>
>La mayoría de los campos no alcanzan el máximo en el número de caracteres, sino en la cantidad de bytes. Por ello, no podemos proporcionar un límite de caracteres definitivo para cada campo. La excepción es **Cadena**, que alcanza un máximo de 255 caracteres.

## Booleano {#boolean}

**Nombre de ejemplo:** Es cliente: Etiquete a sus empleados como clientes

**Valores de ejemplo:** Verdadero (activado) / Falso (desactivado)

**Operadores**: Ninguno

## Moneda {#currency}

**Nombre de ejemplo:** Presupuesto: almacene un valor numérico para el presupuesto de una empresa

**Valores de ejemplo:** 100

**Operadores**: es, no es, entre, bueno que, menos que, al menos, como máximo, está vacío, no está vacío

## Fecha {#date}

**Nombre de ejemplo:** Fecha de renovación: guarde las fechas de renovación de los clientes

**Valores de ejemplo:** 19/8/14

**Operadores**: es, no es, entre, en el pasado, en el pasado antes, en el futuro, en el futuro después, en el lapso de tiempo, después, antes, en o después, en o antes, está vacío, no está vacío

## Fecha y hora {#datetime}

**Nombre de ejemplo:** Fecha de creación: almacena la fecha y la hora de creación de una persona.

**Valores de ejemplo:** 19/8/14 2:00

**Operadores**: es, no es, entre, en el pasado, en el pasado antes, en el futuro, en el futuro después, en el lapso de tiempo, después, antes, en o después, en o antes, está vacío, no está vacío

## Correo electrónico {#email}

**Nombre de ejemplo:** Correo electrónico alternativo: mantenga una dirección de correo electrónico alternativa para sus recursos (no puede enviar correos electrónicos a este campo, como el campo de dirección de correo electrónico predeterminado, ya que es especial)

**Valores de ejemplo:** name@company.com

**Operadores**: es, no es, comienza con, no empieza con, contiene, no contiene, está vacío, no está vacío

## Flotante {#float}

**Nombre de ejemplo:** Promedio de punto de grado: mantenga el promedio de punto de grado de una persona o cualquier otro valor numérico que tenga decimales

**Valores de ejemplo:** 2,47

**Operadores**: entre, bueno que, menor que, como mínimo, está vacío, no está vacío

## Fórmula {#formula}

**Nombre de ejemplo:** Saludos: utilice este campo especial en una [solución para obtener el saludo adecuado](/help/marketo/product-docs/administration/field-management/create-and-use-a-concatenated-string-formula-field.md) en función del sexo

**Valores de ejemplo:** comprobar la solución vinculada

## Entero {#integer}

**Nombre de ejemplo:** Número de empleados: almacene un valor numérico que no requiera decimales

**Valores de ejemplo:** 600

**Operadores**: es, no es, entre, bueno que, menos que, al menos, como máximo, está vacío, no está vacío

## Porcentaje {#percent}

**Nombre de ejemplo:** Probabilidad de comprar: almacene un valor porcentual (tal vez calculado en el lado del CRM)

**Valores de ejemplo:** 85 %

**Operadores**: es, no es, entre, bueno que, menos que, al menos, como máximo, está vacío, no está vacío

## Teléfono {#phone}

**Nombre de ejemplo:** Teléfono alternativo: almacena un número de teléfono adicional para tu gente

**Valor de ejemplo:** 650-555-5555

**Operadores**: es, no es, comienza con, no empieza con, contiene, no contiene, está vacío, no está vacío

## Puntuación {#score}

**Nombre de ejemplo:** Puntuación de comportamiento/puntuación demográfica: cree varios campos de puntuación para realizar un seguimiento de diferentes atributos

**Valor de ejemplo:** 14

**Operadores**: es, no es, entre, bueno que, menos que, al menos, como máximo, está vacío, no está vacío

## Cadena {#string}

**Nombre de ejemplo:** Segundo nombre: almacene un atributo de texto adicional

**Valor de ejemplo:** Rose

**Operadores**: es, no es, comienza con, no empieza con, contiene, no contiene, está vacío, no está vacío

## Área de texto {#text-area}

**Nombre de ejemplo:** Comentarios: agregue un campo de comentarios a los formularios para permitir la entrada de texto multilínea

**Valor de ejemplo:** Este artículo es fantástico!

**Operadores**: es, no es, comienza con, no empieza con, contiene, no contiene, está vacío, no está vacío

## URL {#url}

**Nombre de ejemplo:** Blog: Cree un campo para almacenar las direcciones URL del blog de la persona

**Valor de ejemplo:** www.myblog.com

**Operadores**: es, no es, comienza con, no empieza con, contiene, no contiene, está vacío, no está vacío
