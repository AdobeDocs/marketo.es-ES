---
unique-page-id: 11382829
description: Descubra cómo el departamento de TI puede desinstalar el complemento de Marketo Outlook. Quite el complemento de los equipos de usuario cuando sea necesario.
title: Desinstalación del complemento Marketo [!DNL Outlook] por TI
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
feature: Marketo Sales Insights
TQID: https://experienceleague.adobe.com/p2CjKHycrJRHLpphyn2qsUEKP-dWh2OlTezwrOn9Ljw
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 138
ht-degree: 2%

---

# Desinstalación del complemento Marketo [!DNL Outlook] por TI {#marketo-outlook-plugin-uninstall-by-it}

Así es como el departamento de TI puede desinstalar el complemento de Marketo [!DNL Outlook] de forma remota.

Ejecute la siguiente línea de comandos como, por ejemplo, &quot;System&quot; o una cuenta de usuario administrativo con el modificador /x para desinstalar.

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**Ejemplo**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

Para solucionar problemas, puede habilitar el registro para crear un archivo de registro de salida.

`<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Ejemplo**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

Para especificar una ubicación de los archivos de registro, puede especificar la ruta de acceso del archivo en la línea de comandos.

`<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Ejemplo**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>Si se desinstala el complemento de forma remota, se cerrará [!DNL Outlook] a la fuerza en el equipo del usuario.

Consulte la lista completa de modificadores de [Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) si desea probar diferentes niveles de registro o niveles de interfaz de usuario.
