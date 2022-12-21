---
unique-page-id: 2950578
description: 'Administrar datos de perfil social: documentos de Marketo: documentación de producto'
title: Administrar datos de perfil social
exl-id: 9b20c6fc-5c80-4665-9c93-1bb6e53a29ae
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 6%

---

# Administrar datos de perfil social {#manage-social-profile-data}

Cuando alguien interactúa con un Marketo [aplicación social](/help/marketo/product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)o autoriza a su red social a rellenar previamente un formulario de Marketo con [relleno de formulario social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), Marketo captura todos los datos disponibles en su perfil social. Puede ver esta información en el [Página Detalles de persona](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md)o agréguelo como una columna en un [vista personalizada de una lista inteligente](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/create-and-change-views-for-lists-and-smart-list.md).

El relleno de formularios sociales y las aplicaciones sociales capturan conjuntos de campos ligeramente diferentes; consulte la sección de cada a continuación.

>[!AVAILABILITY]
>
>No todos los clientes han adquirido esta funcionalidad. Póngase en contacto con su representante de ventas para obtener más información.

## Capturado a través de la aplicación social {#captured-via-social-app}

Según la configuración de privacidad de la red y del usuario, se recuperan uno o más de estos campos:

>[!NOTE]
>
>La información adicional de las redes sociales aparece en la página Detalles de la persona unos cinco minutos después de que la persona lo autorice.

## Desde Twitter: {#from-twitter}

* Nombre (analizado desde Nombre para mostrar)
* Apellidos (analizado desde Nombre para mostrar)
* URL de foto de perfil
* URL de la página del perfil
* Alcance social (número de seguidores)

>[!NOTE]
>
>Las aplicaciones sociales no recuperan la dirección de correo electrónico de la persona.

## Desde Facebook: {#from-facebook}

* Nombre
* Apellido
* URL del perfil
* URL de foto de perfil
* Sexo
* Alcance social (número de amigos)

### Capturado mediante Relleno de formulario social {#captured-via-social-form-fill}

Según la configuración de privacidad de la red y del usuario, se recuperan uno o más de estos campos:

>[!CAUTION]
>
>Los datos capturados por el rellenado de formularios sociales sobrescriben los campos coincidentes a menos que [bloquear actualizaciones de esos campos en el nivel de formulario](/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md).

## Desde Twitter: {#from-twitter-1}

* Nombre (analizado desde Nombre para mostrar)
* Apellidos (analizado desde Nombre para mostrar)
* Email

## Desde Facebook: {#from-facebook-1}

* Nombre
* Apellido
* Email
* Fecha de nacimiento
* Cargo
* Compañía

>[!NOTE]
>
>El relleno de formulario social captura la dirección de correo electrónico _only_ si la persona lo introduce en el formulario. Si necesita la dirección de correo electrónico, debe [haga que sea un campo obligatorio en el formulario](/help/marketo/product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Para capturar esta información de los formularios, active [relleno de formulario social](/help/marketo/product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).
