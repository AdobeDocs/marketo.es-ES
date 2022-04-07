---
unique-page-id: 11382829
description: Desinstalación del complemento de Marketo Outlook por parte de TI - Documentos de Marketo - Documentación del producto
title: Desinstalación del complemento de Marketo Outlook por TI
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
source-git-commit: a24b0de6493d4849723099d6164fafb73ef7c926
workflow-type: tm+mt
source-wordcount: '128'
ht-degree: 2%

---

# Desinstalación del complemento de Marketo Outlook por TI {#marketo-outlook-plugin-uninstall-by-it}

Así es como TI puede desinstalar el complemento de Marketo Outlook de forma remota.

Ejecute la siguiente línea de comandos como como como &quot;Sistema&quot; o una cuenta de usuario administrativo con el modificador /x para desinstalar.

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**Ejemplo**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

Para solucionar el problema, puede habilitar el registro para crear un archivo de registro de salida.

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
>La desinstalación remota del complemento forzosamente cerrará Outlook en el equipo del usuario.

Consulte [Lista completa de conmutadores de Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) si desea probar distintos niveles de registro o niveles de interfaz de usuario.
