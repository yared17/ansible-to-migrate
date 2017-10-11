Building a simple LAMP stack and deploying Application using Ansible Playbooks.
-------------------------------------------

These playbooks require Ansible 1.2.

These playbooks are meant to be a reference and starter's guide to building
Ansible Playbooks. These playbooks were tested on CentOS 6.x so we recommend
that you use CentOS or RHEL to test these modules.

This LAMP stack can be on a single node or multiple nodes. The inventory file
'hosts' defines the nodes in which the stacks should be configured.

        [webservers]
        localhost

        [dbservers]
        bensible

Here the webserver would be configured on the local host and the dbserver on a
server called "bensible". The stack can be deployed using the following
command:

        ansible-playbook -i hosts site.yml

Once done, you can check the results by browsing to http://localhost/index.php.
You should see a simple test page and a list of databases retrieved from the
database server.
-------------------------------------------

Creación de una pila LAMP sencilla e implementación de la aplicación mediante Ansible Playbooks.
-------------------------------------------
Estos cuadernos requieren Ansible 1.2.

Estos libros de ejercicios están destinados a ser una guía de referencia y de inicio para la creación de libros de ejercicios Ansible. Estos manuales se probaron en CentOS 6.x por lo que recomendamos que utilice CentOS o RHEL para probar estos módulos.

Esta pila LAMP puede estar en un solo nodo o en varios nodos. El archivo de inventario 'hosts' define los nodos en los que se deben configurar las pilas.

     [servidores web]
     localhost

     [dbservers]
     bienesible
Aquí el servidor web sería configurado en el host local y el dbserver en un servidor llamado "bensible". La pila se puede implementar mediante el siguiente comando:

     ansible-playbook -i hosts site.yml
Una vez hecho esto, puede comprobar los resultados consultando http: //localhost/index.php. Debería ver una página de prueba simple y una lista de bases de datos recuperadas del servidor de bases de datos.
