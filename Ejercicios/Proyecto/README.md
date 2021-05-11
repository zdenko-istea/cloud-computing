# Proyecto IaaS

## Problemática/Idea

En nuestra empresa se migraron los servidores de computo a kubernetes, a distintos tipos de cluster con distintas caracteristicas, estos clusters son multinodo. Si bien el equipo de computo recomienda levantar localmente un cluster de minikube para las pruebas que queremos realizar no nos sirve ya que especificamente necesitamos un cluster multinodo para que el entorno local sea lo mas parecido a un entorno real de produccion.

## Solución/Proyecto

La solucion a nuestra problematica es levantar un cluster multinodo con vagrant. La ventaja de utilizar solamente vagrant para toda la configuracion es que no dependemos de otras herramientas como tal vez Ansible (que no corre en windows el control plane) pudiendo asi utilizar nuestra solucion en distintos entornos no solamente en unix. Ademas vamos a subir nuestra solucion a un repositorio de github donde otros compañeros van a poder usar nuestra solucion y colaborar con mejoras o cambios a problemas que encuentren en el mismo.

## Implementación y guía paso a paso

Vamos a empezar con los requisitos para esto:

* Primero y principal vamos a instalar virtualbox, lo vamos a necesitar para que vagrant cree nuestras maquinas virtuales, esto lo podemos hacer directamente desde este [enlace][vbox]

* Segundo vamos a descargar vagrant desde el siguiente [enlace][vagrant]

* Una vez descargados, recomiendo instalar un editor de texto como por ejemplo visual studio code de microsoft o el editor de preferencia que tengamos para trabajar con los vagrantfile que vamos a crear.

* Usando la siguiente [guia][k8s] como base crearemos un vagrantfile el cual se encargara de crear nuestro master junto a 2 nodos, es importante saber que podemos customizarlo a nuestro gusto ya sea agregando mas nodos, cambiandoles los hostname, IPs, red, addon para que se encargue de la parte de networking (en nuestro caso calico nos estaba dando errores a la hora de correr el vagrant up por lo que utilizamos weave net)

* Una vez teniendo listo nuestro vagrant file, con el comando "vagrant up" levantaremos toda nuestra infraestructura 

* Si todo sale bien, deberiamos ser capaces de correr el comando "vagrant ssh k8s-master (el nombre de la vm que sea el master del cluster)" y nos conectariamos al master del cluster, donde podremos verificar que todos los nodos se hayan conectado correctamente con el comando "kubectl get nodes" dandonos una salida como la siguiente: 

    ```bash
    vagrant@k8s-master:~$ kubectl get nodes
    NAME         STATUS   ROLES                  AGE   VERSION
    k8s-master   Ready    control-plane,master   23m   v1.21.0
    k8s-node-1   Ready    <none>                 19m   v1.21.0
    k8s-node-2   Ready    <none>                 16m   v1.21.0
    ```

    Links:

    [vbox]: <https://www.virtualbox.org/wiki/Downloads>
    [vagrant]: <https://www.vagrantup.com/downloads>
    [k8s]:<https://medium.com/@raj10x/multi-node-kubernetes-cluster-with-vagrant-virtualbox-and-kubeadm-9d3eaac28b98>