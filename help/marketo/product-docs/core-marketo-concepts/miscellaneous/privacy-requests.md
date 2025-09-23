---
description: 'Solicitudes de privacidad: documentos de Marketo, documentación del producto'
title: Solicitudes de privacidad
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 16%

---

# Solicitudes de privacidad {#privacy-requests}

Este documento proporciona información general sobre la administración de solicitudes de privacidad de datos individuales que puede enviar a Marketo Engage a través de la interfaz de usuario de Privacy Service y la API de Privacy Service.

>[!NOTE]
>
>Las solicitudes de privacidad enviadas a través de la interfaz de usuario de Privacy Service o la API para Marketo Engage solo se aplican a lo siguiente:
>
>* Usuarios de Marketo Engage que han incorporado el sistema Identity Management de Adobe
>
>**-o-**
>
>* Usuarios de Marketo Engage que utilizan otro producto de Experience Cloud que ya se encuentra en el sistema Identity Management de Adobe (por ejemplo, RT-CDP, ediciones B2B y B2P, Audience Manager).

Puede enviar solicitudes individuales para acceder a los datos de consumo y eliminarlos de Marketo Engage de dos formas:

* A través de la IU de Privacy Service: `https://experience.adobe.com/#/@YOURCOMPANYNAME/privacy`. Consulte la documentación [aquí](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html?lang=es){target="_blank"}.
* Mediante la API de Privacy Service. Consulte la documentación [aquí](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target="_blank"} y la información de la API [aquí](https://developer.adobe.com/experience-platform-apis/){target="_blank"}.

[Privacy Service](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html?lang=es){target="_blank"} admite dos tipos de solicitudes: acceso a datos y eliminación de datos.

Veamos cómo se pueden crear solicitudes de acceso y eliminación.

## Configuración necesaria para enviar solicitudes de Marketo Engage {#required-setup-to-send-requests-for-marketo-engage}

Para realizar solicitudes de acceso y eliminación de datos para Marketo Engage, debe:

1. Identificar lo siguiente:

   a. ID de organización de IMS <br/>
b. Dirección de correo electrónico de la persona sobre la que desea actuar

   Un ID de organización de IMS es una cadena alfanumérica de 24 caracteres anexada a @AdobeOrg. Si el equipo de marketing o el administrador interno del sistema de Adobe no conocen la ID de organización de IMS de su organización, póngase en contacto con el Servicio de atención al cliente de Adobe en `gdprsupport@adobe.com`. Necesita el ID de organización de IMS para enviar solicitudes a la API de privacidad.

1. En Privacy Service, puede enviar solicitudes de acceso y eliminación a Marketo Engage y comprobar el estado de las solicitudes existentes.

## Valores de campo requeridos en solicitudes JSON de Marketo Engage {#required-field-values-in-marketo-engage-json-requests}

&quot;companyContext&quot;:

* &quot;área de nombres&quot;: **imsOrgID**
* &quot;valor&quot;: `<Your IMS Org ID Value>`

&quot;usuarios&quot;:

* &quot;acción&quot;: ya sea **acceso** (access) o **eliminación** (delete)
* &quot;userID&quot;:
   * &quot;área de nombres&quot;: **correo electrónico**
   * &quot;tipo&quot;: **estándar**
   * &quot;valor&quot;: `<Data Subject's Email Address>`

&quot;incluir&quot;:

* **marketo** (que es el producto de Adobe que se aplica a la solicitud)

&quot;regulación&quot;:

* **gdpr**, **ccpa**, **pdpa**, **lgpd_bra** o **nzpa_nzl** (que es la norma de privacidad que se aplica a la solicitud)

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
          "action": [
            "delete"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": "john.doe@adobe.com",
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

## Ejemplo 2: Solicitud de acceso a CCPA {#ccpa-access-request}

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
      "jobId": "3115e42d-011b-47ab-a2b0-ed4356af4d3e",
      "customer": {
        "user": {
          "action": [
            "access"
          ],
          "userIDs": [
            {
              "namespace": "email",
              "value": "john.doe@adobe.com",
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

>[!MORELIKETHIS]
>
>[Administración de privacidad](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md)
