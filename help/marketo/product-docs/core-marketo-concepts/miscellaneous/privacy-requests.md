---
description: Solicitudes de privacidad - Documentos de Marketo - Documentación del producto
title: Solicitudes de privacidad
exl-id: ae61eabc-ad8f-4c7b-8097-838e89c1a3ec
source-git-commit: 5aa75cc35ef8d39983563ab34b075ae580f9a97b
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Solicitudes de privacidad {#privacy-requests}

Este documento proporciona información general sobre la administración de solicitudes de privacidad de datos individuales que puede enviar al Marketo Engage a través de la interfaz de usuario del Privacy Service y la API del Privacy Service.

>[!NOTE]
>
>Las solicitudes de privacidad enviadas a través de la interfaz de usuario del Privacy Service o la API para el Marketo Engage solo se aplican a lo siguiente:
>
>* usuarios Marketo Engage que se han incorporado al sistema Identity Management de Adobe
>
>**-o-**
>
>* usuarios Marketo Engage que utilizan otro producto Experience Cloud que ya se encuentra en el sistema Identity Management de Adobe (por ejemplo, RT-CDP, B2B y B2P Editions, Audience Manager).


Puede enviar solicitudes individuales para acceder a los datos de consumo y eliminarlos del Marketo Engage de dos maneras:

* A través de [IU de Privacy Service](https://privacyui.cloud.adobe.io/). Consulte la documentación [here](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html){target=&quot;_blank&quot;}.
* A través de la API de Privacy Service. Consulte la documentación [here](https://developer.adobe.com/experience-platform-apis/references/privacy-service/){target=&quot;_blank&quot;} e información de API [here](https://developer.adobe.com/experience-platform-apis/){target=&quot;_blank&quot;}.

La variable [Privacy Service](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html){target=&quot;_blank&quot;} admite dos tipos de solicitudes: acceso a los datos y eliminación de datos.

Veamos cómo se pueden crear solicitudes de acceso y eliminación.

## Configuración necesaria para enviar solicitudes de Marketo Engage {#required-setup-to-send-requests-for-marketo-engage}

Para realizar solicitudes de acceso y eliminación de datos para el Marketo Engage, debe:

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

* &quot;acción&quot;: o **access** o **delete**
* &quot;userIDs&quot;:
   * &quot;namespace&quot;: **email**
   * &quot;type&quot;: **standard**
   * “Valor”: `<Data Subject’s Email Address>`

&quot;incluir&quot;:

* **marketing** (que es el producto de Adobe que se aplica a la solicitud)

&quot;regulación&quot;:

* **gdpr**, **ccpa**, **pdpa**, **lgpd_bra** o **nzpa_nzl**  (que es la norma de privacidad que se aplica a la solicitud)

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
