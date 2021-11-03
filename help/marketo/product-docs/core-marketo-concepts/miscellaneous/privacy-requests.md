---
description: Solicitudes de privacidad - Documentos de Marketo - Documentación del producto
title: Solicitudes de privacidad
source-git-commit: 17e68ea00647dbfd98fde94827eb300804944511
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Solicitudes de privacidad {#privacy-requests}

Este documento proporciona información general sobre la administración de solicitudes de privacidad de datos individuales que puede enviar al Marketo Engage a través de la interfaz de usuario del Privacy Service y la **API de Privacy Service**.

Puede enviar solicitudes individuales para acceder a los datos de consumo y eliminarlos del Marketo Engage de dos maneras:

* A través de [IU de Privacy Service](https://privacyui.cloud.adobe.io/). Consulte la documentación [here](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html#!api-specification/markdown/narrative/tutorials/privacy_service_tutorial/privacy_service_ui_tutorial.md).
* A través de **API de Privacy Service**. Consulte la documentación [here](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html#!api-specification/markdown/narrative/tutorials/privacy_service_tutorial/privacy_service_api_tutorial.md) y la referencia de la API [here](https://www.adobe.io/apis/experiencecloud/gdpr/api-reference.html#!acpdr/swagger-specs/privacy-service.yaml).

La variable [Privacy Service](https://www.adobe.io/apis/experienceplatform/home/services/privacy-service.html) admite dos tipos de solicitudes: acceso a los datos y eliminación de datos.

Nota: Las solicitudes de privacidad enviadas a través de la interfaz de usuario del Privacy Service o la API para el Marketo Engage solo se aplican a los clientes que tienen las ediciones Marketo Engage + RT-CDP, B2B y B2P.

Veamos cómo se pueden crear solicitudes de acceso y eliminación.

## Configuración necesaria para enviar solicitudes de Marketo Engage {#required-setup-to-send-requests-for-marketo-engage}

Para realizar solicitudes de acceso y eliminación de datos para Marketo Engage, debe:

1. Identifique lo siguiente:

   a. ID de organización IMS<br/>
b. Dirección de correo electrónico de la persona en la que desea actuar

   Un ID de organización de IMS es una cadena alfanumérica de 24 caracteres anexada a @AdobeOrg. Si el equipo de marketing o el administrador interno del sistema de Adobe no conocen el ID de organización de IMS de su organización, póngase en contacto con el servicio de atención al cliente de Adobe en gdprsupport@adobe.com. Necesita el ID de organización de IMS para enviar solicitudes a la API de privacidad.

1. En Privacy Service, puede enviar solicitudes de acceso y eliminación al Marketo Engage y comprobar el estado de las solicitudes existentes.

## Valores de campo requeridos en solicitudes JSON de Marketo Engage {#required-field-values-in-marketo-engage-json-requests}

&quot;companyContexts&quot;:

* &quot;namespace&quot;: **imsOrgID**
* “Valor”: `<Your IMS Org ID Value>`

&quot;usuarios&quot;:

* &quot;key&quot;: `<Your Request Tracking Key>`   (opcional)
* &quot;acción&quot;: o **access** o **delete**
* &quot;userIDs&quot;:
   * &quot;namespace&quot;: **email**
   * &quot;type&quot;: **standard**
   * “Valor”: `<Data Subject’s Email Address>`

&quot;incluir&quot;:

* **marketing** (que es el producto de Adobe que se aplica a la solicitud)

&quot;regulación&quot;:

* **gdpr**, **ccpa**, **pdpa**, **lgpd** o **nzpa**  (que es la norma de privacidad que se aplica a la solicitud)

## Ejemplo 1: Solicitud de eliminación de RGPD {#gdpr-delete-request}

Solicitud JSON

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "key": "AAGDPRO1", 
      "action": [
        "delete"
      ],
      "userIDs": [
        {
          "namespace": "email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "gdpr",
}
```

Respuesta JSON

```text
{
  "requestId": "16331241037112570RX-245",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": "997b01e3-9568-402c-904b-b4e60a437875",
      "customer": {
        "user": {
          "key": "AAGDPRO1",
          "action": [
            "delete"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": " john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```

## Ejemplo 2: Solicitud de acceso a la CCPA {#ccpa-access-request}

Solicitud JSON

```text
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "1231659F56A68A8B7F000101@AdobeOrg"
    }
  ],
  "users": [
    {
      "key": "AAGDPRO1",
      "action": [
        "access"
      ],
      "userIDs": [
        {
          "namespace": "email",
          "type": "standard",
          "value": "john.doe@adobe.com"
        }
      ]
    }
  ],
  "include": [
    "marketo"
  ],
  "regulation": "ccpa",
}
```

Respuesta JSON

```text
{
  "requestId": "16329573462631890RX-207",
  "totalRecords": 1,
  "jobs": [
    {
      "jobId": " 3115e42d-011b-47ab-a2b0-ed4356af4d3e",
      "customer": {
        "user": {
          "key": "AAGDPRO1",
          "action": [
            "access"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": " john.doe@adobe.com",
              "type": "standard",
              "namespaceId": 6,
              "isDeletedClientSide": false
            }
          ]
        }
      }
    }
  ]
}
```
