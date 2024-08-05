---
unique-page-id: 2950578
description: 'Administración de datos de perfil social: documentos de Marketo, documentación del producto'
title: Administrar datos de perfil social
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
feature: Social
source-git-commit: 97324d932b65020d041f728928d3792140bea71c
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 5%

---

# Administrar datos de perfil social {#manage-social-profile-data}

Cuando alguien interactúa con una [aplicación social](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md) de Marketo o autoriza a su red social a rellenar previamente un formulario de Marketo con [relleno de formulario social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), Marketo captura todos los datos disponibles en su perfil social. Puede ver esta información en la [página Detalles de persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) o agregarla como una columna en una [vista personalizada de una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

>[!IMPORTANT]
>
>El 31 de julio de 2024, empezamos el proceso de dejar de utilizar esta función. No va a poder crear nuevos recursos. Los recursos existentes seguirán funcionando hasta el 31 de enero de 2025. [Más información](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

Las aplicaciones sociales y de relleno de formularios capturan conjuntos de campos ligeramente diferentes; consulte la sección correspondiente a cada uno de los campos siguientes.

>[!AVAILABILITY]
>
>No todos los usuarios de Marketo Engage han adquirido esta funcionalidad. Póngase en contacto con el equipo de cuenta de Adobe (su administrador de cuentas) para obtener más información.

## Capturado mediante aplicación social {#captured-via-social-app}

Según la configuración de privacidad de la red y del usuario, se recuperan uno o más de estos campos:

>[!NOTE]
>
>La información adicional de las redes sociales aparece en la página Detalles de la persona unos cinco minutos después de que la persona lo autorice.

## Desde el Twitter: {#from-twitter}

* Nombre (analizado desde Nombre para mostrar)
* Apellidos (analizado desde Nombre para mostrar)
* URL de fotografía de perfil
* URL de página de perfil
* Alcance social (número de seguidores)

>[!NOTE]
>
>Las aplicaciones sociales no recuperan la dirección de correo electrónico de la persona.

## Desde Facebook: {#from-facebook}

* Nombre
* Apellido
* URL de perfil
* URL de fotografía de perfil
* Sexo
* Alcance social (número de amigos)

### Capturado mediante rellenado de formulario social {#captured-via-social-form-fill}

Según la configuración de privacidad de la red y del usuario, se recuperan uno o más de estos campos:

>[!CAUTION]
>
>Los datos capturados por el relleno de formulario social sobrescriben los campos coincidentes a menos que [bloquee las actualizaciones de esos campos en el nivel de formulario](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## Desde el Twitter: {#from-twitter-1}

* Nombre (analizado desde Nombre para mostrar)
* Apellidos (analizado desde Nombre para mostrar)
* Correo electrónico

## Desde Facebook: {#from-facebook-1}

* Nombre
* Apellido
* Correo electrónico
* Fecha de nacimiento
* Cargo
* Compañía

>[!NOTE]
>
>El relleno de formulario social captura la dirección de correo electrónico _solamente_ si la persona lo escribe en el formulario. Si necesita la dirección de correo electrónico, [debe convertirla en un campo obligatorio en el formulario](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Para capturar esta información de los formularios, habilite [rellenado de formulario social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
