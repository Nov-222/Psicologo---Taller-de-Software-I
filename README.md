# Psicologo---Taller-de-Software-I

Enlace de Figma: https://www.figma.com/design/yxYu4kVKuvAHhxLMz1CDve/TS?node-id=0-1&t=Ff2IOxHUwUWb7TGz-1

# Planteamineto
# Análisis del Problema de Nuestro Psicólogo de confianza (Kishou Arima)
# Descripción del problema
El señor Arima, un psicólogo que cuenta con su consultorio, está sufriendo de pérdidas de ingreso a través de su sistema de gestión de citas a través de whatsapp, debido a que ser una administración manual, el cliente por el sobreesfuerzo de administrarlo solo, llega a registrar dos de sus clientes en una misma cita, llega a olvidar registrar algunas citas y también de registrar los cambios en caso de que su cliente cancele las citas o cambie la fecha, por ello se requiere un software que mejore la administración de citas en su sistema prediseñado.
 
# Contexto
El software será utilizado por el señor Arima, manteniendo el sistema prediseñado (el señor utiliza un sistema que consiste en whatsapp, el recibe a través de mensaje directo la solicitudes de consultas) y adaptándolo para que este pueda visualizar sus citas de manera coherente y evitar errores de duplicidad de citas, se refiere a que no se puede reservar una cita en el horario de una ya programada, para evitar pérdidas.

# Usuario / Cliente
Administrador: Es el usuario utilizado por el señor Arima, este debe ser capaz de tener todo el control del software al visualizar , editar, crear y eliminar sus citas.
Cliente (personas con necesidad del servicio de el señor Arima): Estos usuarios tendrán la capacidad de registrar o cancelar su cita.

# Objetivo del sistema 
El software debe permitir que se puedan administrar citas de manera más coherente, se refiere a que el sistema debe permitir registrar, cancelar y editar una cita, a la vez que el administrador pueda visualizar todas las citas de manera intuitiva.

Para ello se implementarán las siguientes tecnologías, supabase como base de datos, el frontend será desarrollado con js vanilla, html y css.

# Alcance del sistema
Incluye:
Un sistema visual de la semana en cual se visualizan las citas de 
8 am a 12 am y de 13 pm a 17 pm
Un formulario para registrar una cita con duración de una hora.
Cancelar una cita a través del sistema visual.
Cancelar una cita a través del carnet del cliente.
Editar una cita a través del sistema visual.

No incluye:
Un chatbot para whatsapp

# Requerimientos funcionales
El software registrará una cita con los siguientes campos (nombre, apellido paterno, apellido materno, carnet, fecha, hora, número de teléfono y gmail)
El sistema permite editar los siguientes campos de una consulta registrada (fecha, hora)
El sistema permite cancelar cualquier consulta siempre y cuando no sea el mismo día.
El sistema se visualizará a través de un calendario de semana con separaciones de una hora y en caso de tener una cita registrada, se visualizará el nombre del cliente y su número de contacto.

# Requerimientos no funcionales
No se debe poder registrar una cita en la hora de otra cita registrada.
Se debe respetar el horario de reservas (8 am - 12 am) y (13 pm - 17 pm)
Todos los campos al registrar una cita deben ser obligatorios

# Supuestos y restricciones
Supuestos:
Asumimos que los clientes son capaces de llenar un formulario de manera intuitiva.
Asumimos que el administrador realiza de manera manual, el envío de mensajes de registro de citas a sus clientes.
Asumimos que el administrador siempre estará atento al software en caso de que cancelen o registren una cita.

# Restricciones:
Se debe considerar que el hardware del administrador carece de la potencia para tener una base de datos de manera local.

# Priorización
Se debe priorizar, el registro de citas, la visualización de citas y poder cancelar una cita, siguiendo el siguiente flujo: cliente quiere registrar una cita -> cita registrada exitosamente ->  cita se puede visualizar en el software -> cliente tiene inconveniente y necesita cancelar la cita -> la cita es cancelada y se visualiza como apagada en el software, una vez finalizado el flujo se procede a los complementarios (editar cita y entre otros), los requerimientos funcionales pueden cambiar a disposición del psicólogo.
