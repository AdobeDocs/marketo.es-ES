---
unique-page-id: 2950578
description: Administrar datos de Perfiles sociales - Documentos de marketing - Documentación de productos
title: Administrar datos de Perfiles sociales
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---


# Administrar datos de Perfil social {#manage-social-profile-data}

Cuando alguien interactúa con una aplicación social de Marketing [](../../../../product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md) o autoriza a su red social a rellenar previamente un formulario de Marketo con [relleno de formulario social](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md), Marketo captura todos los datos disponibles en su perfil social. Puede vista esta información en la [página Detalles de la persona](http://docs.marketo.com/display/DOCS/Using+the+Person+Detail+Page) o agregarla como columna en una [vista personalizada de una lista inteligente](http://docs.marketo.com/display/DOCS/Create+and+Change+Views+for+Lists+and+Smart+List).

El relleno de formularios sociales y las aplicaciones sociales capturan conjuntos de campos ligeramente diferentes; consulte la sección de cada uno de ellos a continuación.

>[!NOTE]
>
>**Disponibilidad**
>
>No todos los clientes han adquirido esta funcionalidad. Póngase en contacto con su representante de ventas para obtener más detalles.

## Capturado mediante la aplicación de Social {#captured-via-social-app}

Según la configuración de privacidad de la red y del usuario, se recuperan uno o varios de estos campos:

>[!NOTE]
>
>La información adicional de las redes sociales aparece en la página Detalles de la persona unos cinco minutos después de que la persona autorice.

## Desde Twitter: {#from-twitter}

* Nombre (analizado desde Nombre para mostrar)
* Apellido (analizado desde Nombre para mostrar)
* URL de la foto de perfil
* URL de la página de perfil
* Alcance social (número de seguidores)

>[!NOTE]
>
>Las aplicaciones sociales no recuperan la dirección de correo electrónico de la persona.

## Desde Facebook: {#from-facebook}

* Nombre
* Apellido
* URL de perfil
* URL de la foto de perfil
* Género
* Alcance social (número de amigos)

### Capturado mediante el relleno de formulario social {#captured-via-social-form-fill}

Según la configuración de privacidad de la red y del usuario, se recuperan uno o varios de estos campos:

>[!CAUTION]
>
>Los datos capturados por el relleno de formularios sociales sobrescriben los campos coincidentes a menos que [bloquee las actualizaciones de esos campos en el nivel de formulario](../../../../product-docs/administration/field-management/block-updates-to-a-field.md).

## Desde Twitter: {#from-twitter-1}

* Nombre (analizado desde Nombre para mostrar)
* Apellido (analizado desde Nombre para mostrar)
* Correo electrónico

## Desde Facebook: {#from-facebook-1}

* Nombre
* Apellido
* Correo electrónico
* Fecha de nacimiento
* Puesto de trabajo
* Compañía

>[!NOTE]
>
>El relleno del formulario social captura la dirección de correo electrónico *sólo* si la persona la introduce en el formulario. Si necesita la dirección de correo electrónico, debe [convertirla en un campo requerido en el formulario](../../../../product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Para capturar esta información de los formularios, habilite [relleno de formulario social](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md).

>[!NOTE]
>
>**Buceo profundo**
>
>Obtenga más información sobre cómo trabajar con formularios en la [división profunda de Forms](http://docs.marketo.com/display/docs/forms).

