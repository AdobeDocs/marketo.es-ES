---
unique-page-id: 11382815
description: Instalación del complemento de Marketo Outlook por TI - Documentos de Marketo - Documentación del producto
title: Instalación del complemento de Marketo Outlook por TI
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
source-git-commit: a24b0de6493d4849723099d6164fafb73ef7c926
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 1%

---

# Instalación del complemento de Marketo Outlook por TI {#marketo-outlook-plugin-installation-by-it}

A veces, las políticas corporativas requieren que su equipo de TI instale todo el software en los equipos de sus empleados. En estos casos, TI suele hacerlo de forma remota utilizando su propio software de implementación. Este documento proporciona las líneas de comandos que utilizaría como entradas durante el proceso de implementación para instalar de forma remota el complemento de outlook.

>[!PREREQUISITES]
>
>[Configuración](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) la clave de empresa.

Ejecute la siguiente línea de comandos como &quot;System&quot; o una cuenta de usuario administrativo con el modificador /i para instalar.

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Ejemplo**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

Para solucionar el problema, puede habilitar el registro para crear un archivo de registro de salida.

`<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Ejemplo**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

Para especificar una ubicación de los archivos de registro, puede especificar la ruta del archivo en la línea de comandos.

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Ejemplo**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>La ubicación de almacenamiento del archivo de registro debe existir o se anulará la instalación.

Consulte [Lista completa de conmutadores de Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) si desea probar distintos niveles de registro o niveles de interfaz de usuario.

>[!MORELIKETHIS]
>
>[Desinstalación del complemento de Marketo Outlook por TI](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
