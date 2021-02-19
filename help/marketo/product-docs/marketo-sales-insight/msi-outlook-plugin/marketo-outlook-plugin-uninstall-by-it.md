---
unique-page-id: 11382829
description: Desinstalación del complemento de Marketing to Outlook por TI - Documentos de marketing - Documentación del producto
title: Desinstalación del complemento de Marketing to Outlook por TI
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# Desinstalación del complemento de Marketingto Outlook por parte de TI {#marketo-outlook-plugin-uninstall-by-it}

Así es como TI puede desinstalar el complemento de Marketing to Outlook de forma remota.

Ejecute la siguiente línea de comandos como &quot;System&quot; o una cuenta de usuario administrativo con el modificador /x para desinstalar.

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

Para especificar una ubicación de los archivos de registro, puede especificar la ruta del archivo en la línea de comandos.

`<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**Ejemplo**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>Al desinstalar el complemento de forma remota, se cerrará Outlook de forma forzada en el equipo del usuario.

Consulte la [lista completa de switches](https://support.microsoft.com/en-us/kb/227091) de Microsoft si desea probar diferentes niveles de registro o niveles de interfaz de usuario.
