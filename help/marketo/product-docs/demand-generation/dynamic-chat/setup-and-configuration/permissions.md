---
description: Permisos - Documentos de Marketo - Documentación del producto
title: Permisos
feature: Dynamic Chat
exl-id: e05308fe-b8b7-40a3-8099-cec937e1961c
source-git-commit: feb7c04d056455c00cfe63a1ada17f7c34b509d3
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 10%

---

# Permisos {#permissions}

Hay cinco perfiles predeterminados con permisos predefinidos que puede editar en Dynamic Chat. También puede crear un perfil personalizado con un conjunto personalizado de permisos. Vamos a repasar ambas cosas.

## Editar permisos existentes {#edit-existing-permissions}

1. En el [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}, haga clic en **Dynamic Chat**.

   ![](assets/permissions-1.png)

1. En el **Perfiles de producto** , seleccione el perfil que desea editar. En este ejemplo, elegimos **Live Agent**.

   ![](assets/permissions-2.png)

1. Haga clic en **Permisos** pestaña.

   ![](assets/permissions-3.png)

1. Seleccione el área del perfil que desea editar. En este ejemplo, elegimos Chat en vivo. Haga clic en el icono de lápiz.

   ![](assets/permissions-4.png)

1. Los elementos de permiso disponibles se muestran a la izquierda. Puede elegir agregar los permisos uno a uno o todos a la vez. En este ejemplo solo hay uno disponible, por lo que vamos a añadir ese. Haga clic en **+** signo.

   ![](assets/permissions-5.png)

   >[!NOTE]
   >
   >Al habilitar la inclusión automática, se agregarán todos los elementos de permiso a la lista incluida. Cuando hay nuevos elementos de permiso disponibles, se incluyen automáticamente en ese perfil de producto.

1. Haga clic en **Guardar**.

   ![](assets/permissions-6.png)

Ahora puede repetir este proceso para cualquiera/todas las demás áreas de Dynamic Chat.

![](assets/permissions-7.png)

## Crear un perfil {#create-a-profile}

1. En el [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}, haga clic en **Dynamic Chat**.

   ![](assets/permissions-8.png)

1. En el **Perfiles de producto** pestaña, haga clic en **Nuevo perfil**.

   ![](assets/permissions-9.png)

1. **Nombre** su perfil de producto. Opcionalmente, puede darle un nombre para mostrar o una descripción y elegir que se notifique a los usuarios cuando se agreguen o eliminen. Clic **Guardar** cuando termine.

   ![](assets/permissions-10.png)

1. El nuevo perfil aparecerá en la pestaña Perfiles de producto. Selecciónelo.

   ![](assets/permissions-11.png)

1. Ahora siga los pasos 3-6 de la [sección anterior](#edit-existing-permissions) para cada área deseada.

## Lista de permisos {#list-of-permissions}

A continuación, se muestra una lista de todos los permisos disponibles para cada área.

<table>
<thead>
  <tr>
    <th style="width:30%">Área del Dynamic Chat</th>
    <th>Permisos</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Administración de conversaciones</td>
    <td><li>Ver cuadros de diálogo</li>
    <li>Administrar cuadros de diálogo (crear, eliminar)</li>
    <li>Cuadros de diálogo de publicación</li>
    <li>Ver flujos de conversación</li>
    <li>Administrar flujos de conversación (crear, eliminar)</li>
    <li>Publicar flujos de conversación</li></td>
  </tr>
  <tr>
    <td>Chat en directo</td>
    <td><li>Ver mis conversaciones</li>
    <li>Ver todas las conversaciones</li>
  </tr>
  <tr>
    <td>Reuniones</td>
    <td><li>Administrar todas las reuniones</li>
  </tr>
  <tr>
    <td>Analytics</td>
    <td><li>Ver informes de rendimiento globales</li>
    <li>Ver informes de chat en directo</li>
    <li>Ver informes de reuniones</li>
    <li>Exportar informes</li></td>
  </tr>
  <tr>
    <td>Configuración del agente</td>
    <td><li>Administrar disponibilidad de chat en vivo</li>
    <li>Conectar el calendario</li>
    <li>Administrar disponibilidad del calendario</li></td>
  </tr>
  <tr>
    <td>Configuración del administrador</td>
    <td><li>Ver operación por turnos</li>
    <li>Ver reglas personalizadas</li>
    <li>Administrar reglas personalizadas (agregar, editar, eliminar)</li>
    <li>Ver lista de cuentas <b>*</b></li>
    <li>Administrar cuentas (añadir, editar, eliminar) <b>*</b></li>
    <li>Administrar configuración del bot de chat</li>
    <li>Administrar configuración de flujos de conversación</li>
    <li>Administración de privacidad y seguridad</li>
    <li>Administrar integraciones</li>
    <li>Administrar agentes</li>
    <li>Ver equipos del agente <b>*</b></li>
    <li>Administrar equipos de agentes (añadir, editar, eliminar) <b>*</b></li></td>
  </tr>
</tbody>
</table>

**&#42;** Actualmente solo disponible para usuarios de Dynamic Prime

<p>

## Permisos de perfil predeterminados {#default-profile-permissions}

A continuación se muestran los cinco perfiles predeterminados y los permisos habilitados de forma predeterminada.

<table>
<thead>
  <tr>
    <th style="width:30%">Perfil</th>
    <th>Permisos predeterminados</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Usuario de marketing</td>
    <td><i>Administración de conversaciones</i>
    <li>Ver cuadros de diálogo</li>
    <li>Administrar cuadros de diálogo (crear, eliminar)</li>
    <li>Cuadros de diálogo de publicación</li>
    <li>Ver flujos de conversación</li>
    <li>Administrar flujos de conversación (crear, eliminar)</li>
    <li>Publicar flujos de conversación</li>
    <p>
    <i>Chat en directo</i>
    <li>n/a</li>
    <p>
    <br/><i>Reuniones</i>
    <li>n/a</li>
    <p>
    <br/><i>Analytics</i>
    <li>Ver informes de rendimiento globales</li>
    <li>Ver informes de chat en directo</li>
    <li>Ver informes de reuniones</li>
    <p>
    <br/><i>Configuración del agente</i>
    <li>n/a</li>
    <p>
    <br/><i>Configuración del administrador</i>
    <li>Ver operación por turnos</li>
    <li>Ver reglas personalizadas</li>
    <li>Ver lista de cuentas <b>*</b></li>
    <li>Ver equipos del agente <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>Live Agent</b></td>
    <td><i>Administración de conversaciones</i>
    <p>
    <li>Ver cuadros de diálogo</li>
    <li>Ver flujos de conversación</li>
    <p>
    <p><i>Chat en directo</i></p>
    <li>Ver mis conversaciones</li>
    <p>
    <p><i>Reuniones</i></p>
    <li>n/a</li>
    <p>
    <p><i>Analytics</i></p>
    <li>Ver informes de rendimiento globales</li>
    <li>Ver informes de chat en directo</li>
    <li>Ver informes de reuniones</li>
    <p>
    <p><i>Configuración del agente</i></p>
    <li>Administrar disponibilidad de chat en vivo</li>
    <li>Conectar el calendario</li>
    <li>Administrar disponibilidad del calendario</li>
    <p>
    <p><i>Configuración del administrador</i></p>
    <li>Ver operación por turnos</li>
    <li>Ver reglas personalizadas</li>
    <li>Ver lista de cuentas <b>*</b></li>
    <li>Ver equipos del agente <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>Agente de calendario</b></td>
    <td><i>Administración de conversaciones</i>
    <p>
    <li>Ver cuadros de diálogo</li>
    <li>Ver flujos de conversación</li>
    <p>
    <p><i>Chat en directo</i></p>
    <li>n/a</li>
    <p>
    <p><i>Reuniones</i></p>
    <li>n/a</li>
    <p>
    <p><i>Analytics</i></p>
    <li>Ver informes de rendimiento globales</li>
    <li>Ver informes de chat en directo</li>
    <li>Ver informes de reuniones</li>
    <p>
    <p><i>Configuración del agente</i></p>
    <li>Conectar el calendario</li>
    <li>Administrar disponibilidad del calendario</li>
    <p>
    <p><i>Configuración del administrador</i></p>
    <li>Ver operación por turnos</li>
    <li>Ver reglas personalizadas</li>
    <li>Ver lista de cuentas <b>*</b></li>
    <li>Ver equipos del agente <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>Administrador de marketing</b></td>
    <td><i>Administración de conversaciones</i>
    <p>
    <li>Ver cuadros de diálogo</li>
    <li>Administrar cuadros de diálogo (crear, eliminar)</li>
    <li>Cuadros de diálogo de publicación</li>
    <li>Ver flujos de conversación</li>
    <li>Administrar flujos de conversación (crear, eliminar)</li>
    <li>Publicar flujos de conversación</li>
    <p>
    <p><i>Chat en directo</i></p>
    <li>n/a</li>
    <p>
    <p><i>Reuniones</i></p>
    <li>n/a</li>
    <p>
    <p><i>Analytics</i></p>
    <li>Ver informes de rendimiento globales</li>
    <li>Ver informes de chat en directo</li>
    <li>Ver informes de reuniones</li>
    <li>Exportar informes</li>
    <p>
    <p><i>Configuración del agente</i></p>
    <li>n/a</li>
    <p>
    <p><i>Configuración del administrador</i></p>
    <li>Ver operación por turnos</li>
    <li>Ver reglas personalizadas</li>
    <li>Administrar reglas personalizadas (agregar, editar, eliminar)</li>
    <li>Ver lista de cuentas <b>*</b></li>
    <li>Administrar cuentas (añadir, editar, eliminar) <b>*</b></li>
    <li>Administrar configuración del bot de chat</li>
    <li>Administrar configuración de flujos de conversación</li>
    <li>Administración de privacidad y seguridad</li>
    <li>Administrar integraciones</li>
    <li>Ver equipos del agente <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>Administrador de ventas</b></td>
    <td><i>Administración de conversaciones</i>
    <p>
    <li>Ver cuadros de diálogo</li>
    <li>Ver flujos de conversación</li>
    <p>
    <p><i>Chat en directo</i></p>
    <li>Ver mis conversaciones</li>
    <li>Ver todas las conversaciones</li>
    <p>
    <p><i>Reuniones</i></p>
    <li>Administrar todas las reuniones</li>
    <p>
    <p><i>Analytics</i></p>
    <li>Ver informes de rendimiento globales</li>
    <li>Ver informes de chat en directo</li>
    <li>Ver informes de reuniones</li>
    <li>Exportar informes</li>
    <p>
    <p><i>Configuración del agente</i></p>
    <li>Administrar disponibilidad de chat en vivo</li>
    <li>Conectar el calendario</li>
    <li>Administrar disponibilidad del calendario</li>
    <p>
    <p><i>Configuración del administrador</i></p>
    <li>Ver operación por turnos</li>
    <li>Ver reglas personalizadas</li>
    <li>Administrar reglas personalizadas (agregar, editar, eliminar)</li>
    <li>Ver lista de cuentas <b>*</b></li>
    <li>Administrar cuentas (añadir, editar, eliminar) <b>*</b></li>
    <li>Administrar agentes</li>
    <li>Ver equipos del agente <b>*</b></li>
    <li>Administrar equipos de agentes <b>*</b></li>
    </td>
  </tr>
</tbody>
</table>

**&#42;** Actualmente solo disponible para usuarios de Dynamic Prime
