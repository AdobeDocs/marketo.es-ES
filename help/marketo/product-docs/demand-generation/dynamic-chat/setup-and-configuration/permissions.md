---
description: Permisos - Documentos de Marketo - Documentación del producto
title: Permisos
feature: Dynamic Chat
exl-id: 06798ac4-636b-476e-bbb1-498062844406
source-git-commit: 38e1e2d8c2fef7163f77d7774837571008075b5f
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 5%

---

# Permisos {#permissions}

Hay cinco perfiles predeterminados con permisos predefinidos que puede editar en Dynamic Chat. También puede crear un perfil personalizado con un conjunto personalizado de permisos. Vamos a repasar ambas cosas.

## Editar permisos existentes {#edit-existing-permissions}

1. En [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}, haga clic en **Dynamic Chat**.

   ![](assets/permissions-1.png)

1. En la ficha **Perfiles de producto**, seleccione el perfil que desee editar. En este ejemplo, elegimos **Agente activo**.

   ![](assets/permissions-2.png)

1. Haga clic en la ficha **Permisos**.

   ![](assets/permissions-3.png)

1. Seleccione el área del perfil que desea editar. En este ejemplo, elegimos Chat en vivo. Haga clic en el icono de lápiz.

   ![](assets/permissions-4.png)

1. Los elementos de permiso disponibles se muestran a la izquierda. Puede elegir agregar los permisos uno a uno o todos a la vez. Haga clic en el signo **+**.

   ![](assets/permissions-5.png)

   >[!NOTE]
   >
   >Al habilitar la inclusión automática, se agregarán todos los elementos de permiso a la lista incluida. Cuando hay nuevos elementos de permiso disponibles, se incluyen automáticamente en ese perfil de producto.

1. Haga clic en **Guardar**.

   ![](assets/permissions-6.png)

Ahora puede repetir este proceso para cualquiera/todas las demás áreas de Dynamic Chat.

![](assets/permissions-7.png)

## Crear un perfil {#create-a-profile}

1. En [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}, haga clic en **Dynamic Chat**.

   ![](assets/permissions-8.png)

1. En la ficha **Perfiles de producto**, haga clic en **Nuevo perfil**.

   ![](assets/permissions-9.png)

1. **Nombre** su perfil de producto. Opcionalmente, puede darle un nombre para mostrar o una descripción y elegir que se notifique a los usuarios cuando se agreguen o eliminen. Haga clic en **Guardar** cuando termine.

   ![](assets/permissions-10.png)

1. El nuevo perfil aparecerá en la pestaña Perfiles de producto. Selecciónelo.

   ![](assets/permissions-11.png)

1. Ahora siga los pasos 3-6 de la sección [arriba](#edit-existing-permissions) para cada área deseada.

## Lista de permisos {#list-of-permissions}

A continuación, se muestra una lista de todos los permisos disponibles para cada área.

<table>
<thead>
  <tr>
    <th style="width:25%">Área del Dynamic Chat</th>
    <th>Permisos</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Administración de conversaciones</td>
    <td><li>Ver cuadros de diálogo</li>
    <li>Administrar cuadros de diálogo (crear, eliminar)</li>
    <li>Diálogos de Publish</li>
    <li>Ver flujos de conversación</li>
    <li>Administrar flujos de conversación (crear, eliminar)</li>
    <li>Flujos de conversación Publish</li></td>
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
    <li>Administrar cuentas (agregar, editar, eliminar) <b>*</b></li>
    <li>Administrar configuración del bot de chat</li>
    <li>Administrar configuración de flujos de conversación</li>
    <li>Administración de privacidad y seguridad</li>
    <li>Administrar integraciones</li>
    <li>Administrar agentes</li>
    <li>Ver equipos del agente <b>*</b></li>
    <li>Administrar equipos del agente (agregar, editar, eliminar) <b>*</b></li></td>
  </tr>
</tbody>
</table>

**&#42;** Actualmente solo está disponible para usuarios de Dynamic Prime

<p>

## Permisos de perfil predeterminados {#default-profile-permissions}

A continuación se muestran los cinco perfiles predeterminados y los permisos habilitados de forma predeterminada.

<table>
<thead>
  <tr>
    <th style="width:25%">Perfil</th>
    <th>Permisos predeterminados</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Usuario de marketing</td>
    <td><i>Administración de conversaciones</i>
    <li>Ver cuadros de diálogo</li>
    <li>Administrar cuadros de diálogo (crear, eliminar)</li>
    <li>Diálogos de Publish</li>
    <li>Ver flujos de conversación</li>
    <li>Administrar flujos de conversación (crear, eliminar)</li>
    <li>Flujos de conversación Publish</li>
    <br>
    <i>Chat en vivo</i>
    <li>n/a</li>
    <br>
    <i>Reuniones</i>
    <li>n/a</li>
    <br>
    <i>Análisis</i>
    <li>Ver informes de rendimiento globales</li>
    <li>Ver informes de chat en directo</li>
    <li>Ver informes de reuniones</li>
    <br>
    <i>Configuración del agente</i>
    <li>n/a</li>
    <br>
    <i>Configuración de administración</i>
    <li>Ver operación por turnos</li>
    <li>Ver reglas personalizadas</li>
    <li>Ver lista de cuentas <b>*</b></li>
    <li>Ver equipos del agente <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>Live Agent</b></td>
    <td><i>Administración de conversaciones</i>
    <li>Ver cuadros de diálogo</li>
    <li>Ver flujos de conversación</li>
    <br>
    <i>Chat en vivo</i>
    <li>Ver mis conversaciones</li>
    <br>
    <i>Reuniones</i>
    <li>n/a</li>
    <br>
    <i>Análisis</i>
    <li>Ver informes de rendimiento globales</li>
    <li>Ver informes de chat en directo</li>
    <li>Ver informes de reuniones</li>
    <br>
    <i>Configuración del agente</i>
    <li>Administrar disponibilidad de chat en vivo</li>
    <li>Conectar el calendario</li>
    <li>Administrar disponibilidad del calendario</li>
    <br>
    <i>Configuración de administración</i>
    <li>Ver operación por turnos</li>
    <li>Ver reglas personalizadas</li>
    <li>Ver lista de cuentas <b>*</b></li>
    <li>Ver equipos del agente <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>Agente de calendario</b></td>
    <td><i>Administración de conversaciones</i>
    <li>Ver cuadros de diálogo</li>
    <li>Ver flujos de conversación</li>
    <br>
    <i>Chat en vivo</i>
    <li>n/a</li>
    <br>
    <i>Reuniones</i>
    <li>n/a</li>
    <br>
    <i>Análisis</i>
    <li>Ver informes de rendimiento globales</li>
    <li>Ver informes de chat en directo</li>
    <li>Ver informes de reuniones</li>
    <br>
    <i>Configuración del agente</i>
    <li>Conectar el calendario</li>
    <li>Administrar disponibilidad del calendario</li>
    <br>
    <i>Configuración de administración</i>
    <li>Ver operación por turnos</li>
    <li>Ver reglas personalizadas</li>
    <li>Ver lista de cuentas <b>*</b></li>
    <li>Ver equipos del agente <b>*</b></li>
    </td>
  </tr>
  <tr>
    <td><b>Administrador de marketing</b></td>
    <td><i>Administración de conversaciones</i>
    <li>Ver cuadros de diálogo</li>
    <li>Administrar cuadros de diálogo (crear, eliminar)</li>
    <li>Diálogos de Publish</li>
    <li>Ver flujos de conversación</li>
    <li>Administrar flujos de conversación (crear, eliminar)</li>
    <li>Flujos de conversación Publish</li>
    <br>
    <i>Chat en vivo</i>
    <li>n/a</li>
    <br>
    <i>Reuniones</i>
    <li>n/a</li>
    <br>
    <i>Análisis</i>
    <li>Ver informes de rendimiento globales</li>
    <li>Ver informes de chat en directo</li>
    <li>Ver informes de reuniones</li>
    <li>Exportar informes</li>
    <br>
    <i>Configuración del agente</i>
    <li>n/a</li>
    <br>
    <i>Configuración de administración</i>
    <li>Ver operación por turnos</li>
    <li>Ver reglas personalizadas</li>
    <li>Administrar reglas personalizadas (agregar, editar, eliminar)</li>
    <li>Ver lista de cuentas <b>*</b></li>
    <li>Administrar cuentas (agregar, editar, eliminar) <b>*</b></li>
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
    <li>Ver cuadros de diálogo</li>
    <li>Ver flujos de conversación</li>
    <br>
    <i>Chat en vivo</i>
    <li>Ver mis conversaciones</li>
    <li>Ver todas las conversaciones</li>
    <br>
    <i>Reuniones</i>
    <li>Administrar todas las reuniones</li>
    <br>
    <i>Análisis</i>
    <li>Ver informes de rendimiento globales</li>
    <li>Ver informes de chat en directo</li>
    <li>Ver informes de reuniones</li>
    <li>Exportar informes</li>
    <br>
    <i>Configuración del agente</i>
    <li>Administrar disponibilidad de chat en vivo</li>
    <li>Conectar el calendario</li>
    <li>Administrar disponibilidad del calendario</li>
    <br>
    <i>Configuración de administración</i>
    <li>Ver operación por turnos</li>
    <li>Ver reglas personalizadas</li>
    <li>Administrar reglas personalizadas (agregar, editar, eliminar)</li>
    <li>Ver lista de cuentas <b>*</b></li>
    <li>Administrar cuentas (agregar, editar, eliminar) <b>*</b></li>
    <li>Administrar agentes</li>
    <li>Ver equipos del agente <b>*</b></li>
    <li>Administrar equipos del agente <b>*</b></li>
    </td>
  </tr>
</tbody>
</table>

**&#42;** Actualmente solo está disponible para usuarios de Dynamic Prime
