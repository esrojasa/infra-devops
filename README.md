# infra-devops


## jenkins

Revisar plugins instalados, en la consola de script de jenkins:

    Jenkins.instance.pluginManager.plugins.each{ plugin -> 
        println ("${plugin.getDisplayName()} (${plugin.getShortName()}): ${plugin.getVersion()
    }")
}

## Sonarqube
Contraseña por defecto tras primera instalacion:

    admin/admin

## Nexus

para obtener la contraseña inicial, debes revisar el contenido del fichero _/nexus-data/admin.password del contenedor de nexus. Aca un atajo

    docker exec -it devops-infra-nexus-1 cat /nexus-data/admin.passwo

# urls de acceso:


[Jenkins](http://localhost:8080)

[Nexus Artifactory](http://localhost:8081)

[Sonarqube](http://localhost:8084)