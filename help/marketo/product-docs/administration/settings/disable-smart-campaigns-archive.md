---
description: Obtenga información sobre cómo habilitar la función Deshabilitar campañas inteligentes en archivo, que desactiva automáticamente las campañas cuando se archiva una carpeta o programa en Marketo.
title: Deshabilitar campañas inteligentes en archivo
feature: Administration
hide: true
source-git-commit: 526d10bb96e059d251a76ca720ff81ab42ee9516
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Deshabilitar campañas inteligentes en archivo {#disable-smart-campaigns-on-archive}

Cuando esta función está habilitada, el archivado de una carpeta o programa desactiva automáticamente sus campañas para evitar actividades inesperadas.

Cuando se archiva una carpeta o un programa, o cuando se mueve una campaña inteligente activa a una carpeta que ya está archivada, Marketo Engage detiene la ejecución de las campañas afectadas:

* Se han desactivado **campañas activadas**.
* Se han cancelado las ejecuciones pendientes de **campañas por lotes**.
* **Las campañas ejecutables** no tienen estado de ejecución, por lo que no se realiza ninguna acción.

## Cómo habilitar {#how-to-enable}

1. En la sección **Administrador**, haga clic en **Cofre del tesoro**.

   ![Menú de navegación del administrador con el cofre del tesoro resaltado](assets/disable-smart-campaigns-on-archive-1.png)

1. Desplácese a _Deshabilitar campañas inteligentes en el archivo_ y haga clic en **Editar**.

   ![Página de configuración del cofre del tesoro que muestra la fila Deshabilitar campañas inteligentes en archivo con el botón Editar](assets/disable-smart-campaigns-on-archive-2.png)

1. Seleccione la casilla **Habilitado** y haga clic en **Guardar**.

   ![Cuadro de diálogo Deshabilitar campañas inteligentes en el archivo que muestra la casilla de verificación Habilitada y el botón Guardar](assets/disable-smart-campaigns-on-archive-3.png)

<table>
  <tr>
    <td><b>Habilitado (seleccionado)</b></td>
    <td>El archivado desactiva todas las campañas, según las reglas anteriores.</td>
  </tr>
  <tr>
    <td><b>Desactivado (sin marcar)</b></td>
    <td>El archivado de una carpeta o programa sigue funcionando, pero las campañas se dejan en ejecución o se programan tal cual.</td>
  </tr>
</table>

>[!IMPORTANT]
>
>Después de cambiar esta configuración, debe actualizar el explorador para que el cambio surta efecto.

## Acciones compatibles

Las siguientes acciones desactivan las campañas cuando _Deshabilitar campañas inteligentes en el archivo_ está habilitado:

* Arrastrando y soltando una **carpeta** que contiene campañas activas en una carpeta archivada
* Arrastrando y soltando un **programa** (de cualquier tipo) que contenga campañas activas en una carpeta archivada
* Arrastrando y soltando **una sola campaña inteligente** en una carpeta archivada
* Haciendo clic con el botón derecho en **Mover** de una sola campaña inteligente a una carpeta archivada
* Haciendo clic con el botón derecho en **Mover carpeta** en una carpeta que contenga campañas activas a una carpeta archivada
* Haciendo clic con el botón derecho en **Mover** un programa que contenga campañas activas a una carpeta archivada
* Haciendo clic con el botón derecho en **Convertir en carpeta archivada** en una carpeta para archivarla sin moverla

>[!NOTE]
>
>Si se hace referencia a una campaña inteligente dentro de la carpeta o del programa que se está archivando en otra parte (por ejemplo, a través del paso de flujo &quot;Solicitar campaña&quot;), el archivado se bloquea para evitar que se interrumpa esa otra campaña.
