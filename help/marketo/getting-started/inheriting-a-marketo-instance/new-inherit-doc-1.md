---
description: Heredar documento 1 - Documentos de Marketo - Documentación del producto
title: Heredar documento 1
hide: true
hidefromtoc: true
source-git-commit: b6628cee17799801815f5b84c424399538eaf5ee
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 8%

---

# Heredar documento 1 {#inherit-doc-1}

La auditoría de una instancia heredada puede parecer una

¿Heredó una instancia de Marketo Engage existente de otro administrador? Si es así, este artículo es para usted.

>[!TIP]
>
>Si es un usuario Marketo Engage nuevo y no está familiarizado con muchos de los términos, consulte la [Glosario de Marketo](/help/marketo/getting-started/marketo-glossary.md){target="_blank"}.

## Usuarios y funciones {#users-and-roles}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>Usuarios</td> 
   <td><li>¿Cuántos usuarios hay?</li>
<li>¿Hay algún usuario que debería haber caducado?</li>
<li>¿Su compañía tiene directivas para eliminar usuarios?</li> 
<li>¿Cuántos usuarios tienen permisos de administrador?</li>
<li>¿Alguno de estos usuarios debe cambiarse a otras funciones?</li> 
<li>¿Quiénes son los usuarios de API en esta instancia?</li></td>
   <td>3.1</td>
  </tr>
  <tr> 
   <td>Funciones</td> 
   <td><li>¿Cuántos roles hay?</li>  
<li>¿Qué permisos/acceso tiene cada función? ¿Se debe realizar algún ajuste?</li>
<li>¿Cuántos usuarios hay por función?</li>
<li>¿Con qué frecuencia inician sesión los usuarios?</li>
<li>¿Cada usuario de API tiene su propia función de usuario? Si no es así, considere implementar esto para facilitar la resolución de problemas.</li> 
<li>¿Sus funciones de usuario y permisos se alinean con las políticas de privacidad de datos corporativas?</li></td>
   <td>3.2</td>
  </tr>
  <tr> 
   <td>Documentación interna</td> 
   <td><li>¿Los usuarios y las funciones están claramente definidos en su organización?</li>
<li>¿Cuál es su proceso para agregar un nuevo usuario/administrador?</li></td>
   <td>3.3</td>
  </tr>
  <tr> 
   <td>Zona protegida (si corresponde)</td> 
   <td><li>¿Tiene una instancia de zona protegida? Si es así, revise las categorías anteriores para su zona protegida.</li>
<li>¿La importación de programas está vinculada a su zona protegida?</li></td>
   <td>3.4</td>
  </tr>
 </tbody> 
</table>

## Pista de auditoría {#audit-trail}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>Pista de auditoría</td> 
   <td><li>¿Quién está trabajando en la instancia?</li></td>
   <td>3.1</td>
  </tr>
 </tbody> 
</table>

## Espacios de trabajo y particiones {#workspaces-and-partitions}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>Espacios de trabajo y particiones</td> 
   <td><li>¿Cuántos espacios de trabajo y/o particiones tiene?</li>
<li>¿Cuál es el propósito principal de cada espacio de trabajo y partición?</li>
<li>¿Es necesario auditarlas o cambiarlas?</li>
<li>¿Cuál es la relación entre sus espacios de trabajo y las particiones?</li>
<li>¿Cuántos usuarios tienen acceso a cada espacio de trabajo?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Documentación interna</td> 
   <td><li>¿Cómo se definen los espacios de trabajo y las particiones?</li>
<li>¿Cuál es el proceso para añadir espacios de trabajo a la instancia o añadir usuarios a un espacio de trabajo?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Campañas inteligentes {#smart-campaigns}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>Configuración de campañas inteligentes</td> 
   <td><li>¿Tiene restricciones en el tamaño de la campaña inteligente?</li>
<li>Si no es así, considere la posibilidad de agregar uno. Se recomienda limitar los límites de las campañas inteligentes al 25 % de la base de datos para evitar una comunicación excesiva o procesar toda la base de datos en flujos de trabajo, esto no solo protege la marca, sino que ayuda a proteger el rendimiento de la instancia.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Límites de comunicación {#communication-limits}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>Límites de comunicación</td> 
   <td><li>¿Existen límites? ¿Su empresa tiene políticas en las que podrían ser necesarios límites de comunicación?</li>
<li>El Adobe recomienda limitar la comunicación a 1 por día y a 3 por 7 días, con correos electrónicos no operativos bloqueados.</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Etiquetas {#tags}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>Etiquetas</td> 
   <td><li>¿Cuántas etiquetas hay? ¿Cuántas etiquetas se están utilizando? ¿Es necesario añadir alguna?</li>
<li>¿Se requieren etiquetas dentro de los programas?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Canales</td> 
   <td><li>¿Cuántos canales hay? ¿Cuántos están en uso?</li>
<li>¿Son apropiados todos los estados de programas de canal? ¿Muestran progresión dentro del programa?</li>
<li>¿Sus canales están relacionados con tipos de programas específicos?</li>
<li>¿Qué estados se consideran un éxito para cada canal? ¿Se alinean con sus objetivos de marketing?</li>
<li>¿Se está utilizando correctamente el canal operativo?</li>
<li>En el caso del Report Builder avanzado (Explorador del ciclo de ingresos\RCE), ¿está configurado el comportamiento de análisis de canal para que se ajuste a las prácticas del programa que incorporan el coste del período?</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Calendario de marketing (si corresponde)</td> 
   <td><li>¿Cuántos tipos de entradas de calendario hay? ¿Siguen siendo relevantes?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Administración de bases de datos {#database-management}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>Administración de campos</td> 
   <td><li>¿Cuántos campos hay? Haga clic en "Exportar nombres de campo" para revisar una lista de sus campos, campos personalizados y sus nombres de API.</li>
<li>¿Cuántos campos personalizados hay?</li>
<li>¿Cuántos campos se están utilizando? Seleccione "Exportar usados por" en la lista desplegable Acciones de campo para revisar los recursos relacionados de un campo.</li>
<li>¿Cuántos se sincronizan entre Marketo Engage y su CRM?</li>
<li>¿Los campos de CRM están sincronizados con los objetos adecuados?</li>
<li>¿Hay alguna vista personalizada configurada para los detalles de la persona? ¿Debería haber?</li>
<li>¿Tiene una convención de nombres para los campos basada en el origen? Si no es así, considere implementar esto.</li>
<li>¿Hay algún campo bloqueado? Asegúrese de comprender por qué lo son.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Actividades personalizadas</td> 
   <td><li>¿Hay alguna actividad personalizada?</li>
<li>Si es así, haga clic en ellas para comprender qué actividades no están relacionadas con un formulario, un correo electrónico o una página de aterrizaje de Marketo.</li></td>
   <td>3</td>
  </tr>
  <tr> 
   <td> objetos personalizados de </td> 
   <td><li>¿Cuántos objetos personalizados hay? ¿Cómo se sincronizan con su CRM?</li>
<li>¿Cómo utilizan sus programas y consultas de lista estos objetos personalizados?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Integraciones {#integrations}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>Perspectiva de ventas de Marketo (si corresponde)</td> 
   <td><li>¿Se ha instalado el paquete MSI?</li>
<li>¿Ha actualizado a la versión más reciente de Sales Insight?</li>
<li>¿Ha completado la configuración de Sales Insight?</li>
<li>¿Ha dado acceso a sus usuarios en función del número de puestos que ha adquirido?</li></td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Cofre del tesoro {#treasure-chest}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
 </tbody> 
</table>

## Varios {#miscellaneous}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Área</th> 
   <th>Revisar enfoque</th>
   <th>Columna 3</th>
  </tr> 
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
  <tr> 
   <td>1</td> 
   <td>2</td>
   <td>3</td>
  </tr>
 </tbody> 
</table>
