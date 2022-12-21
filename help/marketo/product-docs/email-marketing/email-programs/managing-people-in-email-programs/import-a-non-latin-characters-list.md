---
unique-page-id: 5472678
description: 'Importar una lista de caracteres no latinos: documentos de Marketo: documentación del producto'
title: Importar una lista de caracteres no latinos
exl-id: 11519e2c-ab01-4164-8ce3-0717e4c13ae6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Importar una lista de caracteres no latinos {#import-a-non-latin-characters-list}

¿Intenta importar un archivo que no esté en inglés? La lista parece perfecta cuando se abre con Excel.

![](assets/image2015-2-10-9-3a34-3a57.png)

Sin embargo, al importarlo en Marketo, es posible que vea que los caracteres que no están en inglés no se recogen correctamente.

![](assets/image2015-2-10-9-3a35-3a49.png)

Esto se debe a que el archivo no se guarda correctamente para que Marketo reconozca todos los caracteres que no sean latinos. La buena noticia es que hay algunos pasos simples que puedes seguir para arreglarlo.

1. Select **Guardar como...** de la variable **Archivo** en Excel.

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. Choose **Texto Unicode UTF-16 (.txt)** como el **Formato** . Esto codificará el archivo de la forma en que Marketo puede mostrarlos.

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo también es compatible con UTF-8, Shift-JIS o EUC-JP.

1. Excel guardará el nuevo archivo como archivo de texto con la extensión .txt . Pero también convierte todas las comas del archivo en pestañas. Tenemos que volver a cambiarlo.

   >[!TIP]
   >
   >Puede abrir el archivo de texto utilizando **Bloc de notas** si utiliza Windows o **TextEdit** si utiliza un Mac.

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. Seleccione una pestaña del documento y cópiela.

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. Select **Buscar y reemplazar...** de la variable **Editar** para abrir el Navegador.

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >La acción equivalente para los usuarios de Windows es: **Editar > Reemplazar...**

1. Pegue la ficha que ha copiado en el paso 4 en el primer cuadro (que desea reemplazar) y escriba una coma en el segundo cuadro (reemplazar por). Y haga clic en **Todo**.

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. Y voila, todas las comas están de vuelta y estamos listos para rodar.

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. Importe el nuevo archivo en Marketo y la información debería mostrarse correctamente esta vez.

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >Cualquier campo de fecha y hora que se importe se tratará como Hora central. Si tiene campos de fecha y hora en un huso horario diferente, puede utilizar una fórmula de Excel para transformarla a la hora central (América/Chicago).

Sabemos que esto es raro, pero funciona. ¡Feliz importación!
