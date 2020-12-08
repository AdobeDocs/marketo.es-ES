---
unique-page-id: 11382815
description: Instalación del complemento de Marketo para Outlook por TI - Documentos de marketing - Documentación del producto
title: Instalación del complemento de Marketo Outlook por TI
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---


# Instalación del complemento de Marketo Outlook por TI {#marketo-outlook-plugin-installation-by-it}

A veces, las políticas corporativas requieren que su equipo de TI instale todo el software en los equipos de sus empleados. En estos casos, TI lo hace a menudo de forma remota utilizando su propio software de implementación. Este documento proporciona las líneas de comandos que utilizaría como entradas durante el proceso de implementación para instalar de forma remota el complemento de Outlook.

>[!NOTE]
>
>**Requisitos previos**
>
>[Configure](http://docs.marketo.com/display/DOCS/Install+the+Marketo+Add-in+for+Outlook+with+an+Enterprise+Key) la clave de empresa.

Ejecute la siguiente línea de comandos como &quot;System&quot; o una cuenta de usuario administrativo con el modificador /i para instalar.  `<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Ejemplo**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

Para solucionar problemas, puede habilitar el registro para crear un archivo de registro de salida.  `<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Ejemplo**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

Para especificar una ubicación de los archivos de registro, puede especificar la ruta del archivo en la línea de comandos.  `<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Ejemplo**
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>La ubicación de almacenamiento del archivo de registro debe existir o se anulará la instalación.

Consulte la lista completa de switches [de](https://support.microsoft.com/en-us/kb/227091) Microsoft si desea probar diferentes niveles de registro o niveles de interfaz de usuario.

>[!NOTE]
>
>**Artículos relacionados**
>
>[Desinstalación del complemento de Marketing to Outlook por TI](marketo-outlook-plugin-uninstall-by-it.md)

