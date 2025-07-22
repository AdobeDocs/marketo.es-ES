---
unique-page-id: 11382815
description: Marketo [!DNL Outlook] Instalación de complementos por TI - Documentos de Marketo - Documentación del producto
title: Instalación de complementos de Marketo [!DNL Outlook] por TI
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 1%

---

# Instalación del complemento Marketo [!DNL Outlook] por TI {#marketo-outlook-plugin-installation-by-it}

A veces, las políticas corporativas requieren que su equipo de TI instale todo el software en los equipos de sus empleados. En estos casos, el departamento de TI suele hacerlo de forma remota utilizando su propio software de implementación. Este documento proporciona las líneas de comandos que utilizaría como entradas durante el proceso de implementación para instalar de forma remota el complemento de Outlook.

>[!PREREQUISITES]
>
>[Configurar](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) la clave de empresa.

Ejecute la siguiente línea de comandos como &quot;System&quot; o una cuenta de usuario administrativo con el modificador /i para instalar.

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Ejemplo**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

Para solucionar problemas, puede habilitar el registro para crear un archivo de registro de salida.

`<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Ejemplo**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

Para especificar una ubicación de los archivos de registro, puede especificar la ruta de acceso del archivo en la línea de comandos.

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**Ejemplo**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>Debe existir la ubicación de almacenamiento del archivo de registro o se anulará la instalación.

Consulte la [lista completa de conmutadores de Microsoft](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) si desea probar diferentes niveles de registro o niveles de interfaz de usuario.

>[!MORELIKETHIS]
>
>[Desinstalación del complemento de Marketo [!DNL Outlook] por parte del equipo de TI](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
