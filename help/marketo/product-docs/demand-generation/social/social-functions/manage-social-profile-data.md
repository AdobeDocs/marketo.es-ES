---
unique-page-id: 2950578
description: Administrar datos de Perfiles sociales - Documentos de marketing - Documentación de productos
title: Administrar datos de Perfiles sociales
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---


# Administrar datos de Perfiles sociales {#manage-social-profile-data}

Cuando alguien interactúa con una aplicación [](../../../../product-docs/demand-generation/social/configuring-social-actions/customize-social-app-button.md)social de marketing o autoriza a su red social a rellenar previamente un formulario de marketing con relleno [de formulario](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)social, Marketing captura todos los datos disponibles en su perfil social. Puede vista esta información en la página [Detalles de la](http://docs.marketo.com/display/DOCS/Using+the+Person+Detail+Page)persona o agregarla como columna en una vista [personalizada de una lista](http://docs.marketo.com/display/DOCS/Create+and+Change+Views+for+Lists+and+Smart+List)inteligente.

>[!NOTE]
>
>**FYI**
>
>Marketo ahora está estandarizando el idioma en todas las suscripciones, por lo que puede ver posibles clientes/posibles clientes en su suscripción y persona/personas en docs.marketo.com. Estos términos significan lo mismo; no afecta a las instrucciones del artículo. También hay otros cambios. [Más información](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

El relleno de formularios sociales y las aplicaciones sociales capturan conjuntos de campos ligeramente diferentes; consulte la sección de cada uno de ellos a continuación.

>[!NOTE]
>
>**Disponibilidad**
>
>No todos los clientes han adquirido esta funcionalidad. Póngase en contacto con su representante de ventas para obtener más detalles.

## Capturado mediante la aplicación social {#captured-via-social-app}

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

### Capturado mediante Relleno de formulario social {#captured-via-social-form-fill}

Según la configuración de privacidad de la red y del usuario, se recuperan uno o varios de estos campos:

>[!CAUTION]
>
>Los datos capturados por el relleno de formularios sociales sobrescriben los campos coincidentes a menos que [bloquee las actualizaciones de esos campos en el nivel](../../../../product-docs/administration/field-management/block-updates-to-a-field.md)del formulario.

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
>El relleno de formulario social captura la dirección de correo electrónico *únicamente* si la persona la introduce en el formulario. Si necesita la dirección de correo electrónico, debe [convertirla en un campo obligatorio en el formulario](../../../../product-docs/demand-generation/forms/creating-a-form/make-a-form-field-required.md).

>[!MORELIKETHIS]
>
>Para capturar esta información de los formularios, habilite el rellenado [de formularios](../../../../product-docs/demand-generation/forms/form-actions/enable-social-form-fill-on-a-form.md)sociales.

>[!NOTE]
>
>**Buceo profundo**
>
>Obtenga más información sobre cómo trabajar con formularios en el buceo profundo de [Forms](http://docs.marketo.com/display/docs/forms) .

