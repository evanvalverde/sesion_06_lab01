# sesion_06_lab01
Laboratorio 1 de la sesión 6 del curso Ansible/AWX 2021: Handlers

## Enunciado

Crearemos un repositorio Github con el nombre sesion_06_lab01
En el añadiremos el inventario y el ansible.cfg que creamos oportuno
Crearemos un playbook.yml con las siguientes tareas:
	- Atacara al nodo_01
	- Instalaremos la paquetería de bind y bind-utils llamara a un handler para arrancar el servicio named y 	habilitarlo permanentemente
	- Forzaremos el handler anterior
	- Añadiremos el servicio de dns al firewall de la maquina
	- Comentaremos las siguientes lineas del archivo /etc/named.conf
	- Creamos un handler para reiniciar le named
	- Forzaremos el handler anterior
	- Modificaremos el archivo /etc/sysconfig/named y cambiaremos el parámetro OPTIONS="-4"
	- Forzaremos el handler del reinicio del servicio named
	- Editaremos el fichero /etc/resolv.conf para borrar todas las líneas con nameserver y añadir un nameserver 	IP-nodo_01 (usar asible facts)
	- Las dos siguientes tareas se han completar cuando se terminen todas las anteriores:
		- reiniciar el servidor
		- comprobar el servicio named esta levantado.
		- mostrar un mensaje por pantalla con la resolución de la tarea anterior