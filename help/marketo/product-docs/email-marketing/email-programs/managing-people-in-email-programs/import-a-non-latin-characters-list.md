---
unique-page-id: 5472678
description: 'Importación de una Lista de caracteres no latinos: Documentos de marketing: documentación del producto'
title: Importación de una Lista de caracteres no latinos
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Importación de una Lista de caracteres no latinos {#import-a-non-latin-characters-list}

¿Está intentando importar un archivo que no está en inglés? La lista se ve perfecta cuando se abre con Excel.

![](assets/image2015-2-10-9-3a34-3a57.png)

Pero al importarlo a Marketing, es posible que vea que los caracteres que no son ingleses no se recogen correctamente.

![](assets/image2015-2-10-9-3a35-3a49.png)

Esto se debe a que el archivo no se guarda correctamente para que Marketing reconozca todos los caracteres no latinos. La buena noticia es que hay algunos pasos sencillos que puedes seguir para arreglarlo.

1. Seleccione **Guardar como...** en el menú **Archivo** de Excel.

   ![](assets/image2015-2-10-9-3a46-3a44.png)

1. Elija Texto Unicode **UTF-16 (.txt)** como opción **Formato** . Esto codificará el archivo de la forma en que Marketing puede mostrarlos.

   ![](assets/image2015-2-10-9-3a48-3a7.png)

   >[!NOTE]
   >
   >Marketo también es compatible con UTF-8, Shift-JIS o EUC-JP.

1. Excel guardará el nuevo archivo como archivo de texto con la extensión .txt. Pero también convierte todas las comas del archivo en fichas. Tenemos que volver a cambiarlo.

   >[!TIP]
   >
   >Puede abrir el archivo de texto con el **Bloc de notas** si utiliza Windows o **TextEdit** si utiliza un Mac.

   ![](assets/image2015-2-10-9-3a51-3a41.png)

1. Seleccione una ficha del documento y cópiela.

   ![](assets/image2015-2-10-9-3a55-3a53.png)

1. Seleccione **Buscar y reemplazar...** en el menú **Editar** .

   ![](assets/image2015-2-10-9-3a59-3a8.png)

   >[!TIP]
   >
   >La acción equivalente para los usuarios de Windows es: **Editar > Reemplazar...**

1. Pegue la ficha copiada en el paso 4 en el primer cuadro (que se va a reemplazar) y escriba una coma en el segundo cuadro (reemplazar por). Y haga clic en **Todo**.

   ![](assets/image2015-2-10-10-3a8-3a53.png)

1. Y voila, todas las comas están de vuelta y estamos listos para rodar.

   ![](assets/image2015-2-10-10-3a14-3a45.png)

1. Importe el nuevo archivo en Marketing y la información debería mostrarse correctamente esta vez.

   ![](assets/image2015-2-10-10-3a16-3a9.png)

   >[!NOTE]
   >
   >Los campos de fecha y hora que se importan se tratan como Hora central. Si tiene campos de fecha y hora en un huso horario diferente, puede utilizar una fórmula de Excel para transformarla en hora central (América/Chicago).

Sabemos que esto es raro, pero funciona. ¡Feliz importación!