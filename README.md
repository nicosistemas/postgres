### REPO UTILIZADO PARA PROBAR CODESPACES Y ISSUES


* PRUEBAS DE ISSUES:

https://github.com/nicosistemas/postgres/issues/1


* CODESPACES:

[algunas maquinas que se pueden usar para codespaces](https://containers.dev/features)

agregas un json en .devcontainer/maquina.json con datos de la máquina Ó podes agregar más maquinas para poder elegir según las features que tengan esos codespaces:

```
.devcontainer/EQUIPO-1/devcontainer.json
.devcontainer/EQUIPO-2/devcontainer.json
```

fuente: https://github.com/devcontainers-contrib/features
---
 ejemplo kubectl

``` console
{
    "id": "kubectl-asdf",
    "version": "2.0.14",
    "name": "Kubectl (via asdf)",
    "documentationURL": "http://github.com/devcontainers-contrib/features/tree/main/src/kubectl-asdf",
    "description": "Installs Kubectl",
    "options": {
        "version": {
            "default": "latest",
            "description": "Select the version to install.",
            "proposals": [
                "latest"
            ],
            "type": "string"
        }
    },
    "installsAfter": [
        "ghcr.io/devcontainers-contrib/features/asdf-package"
    ]
}
```

 ejemplo psql cli

``` console
{
    "id": "postgres-asdf",
    "version": "1.0.2",
    "name": "PostgreSQL (via asdf)",
    "documentationURL": "http://github.com/devcontainers-contrib/features/tree/main/src/postgres-asdf",
    "description": "PostgreSQL is a powerful, open source object-relational database system with over 35 years of active development that has earned it a strong reputation for reliability, feature robustness, and performance.",
    "options": {
        "version": {
            "default": "latest",
            "description": "Select the version to install.",
            "proposals": [
                "latest"
            ],
            "type": "string"
        }
    },
    "installsAfter": [
        "ghcr.io/devcontainers-contrib/features/asdf-package"
    ]
}
```

 ejemplo curl

``` console
{
    "id": "curl-apt-get",
    "version": "1.0.16",
    "name": "cURL (via apt-get)",
    "documentationURL": "http://github.com/devcontainers-contrib/features/tree/main/src/curl-apt-get",
    "description": "cURL is a computer software project providing a library and command-line tool for transferring data using various network protocols.",
    "options": {},
    "installsAfter": [
        "ghcr.io/devcontainers-contrib/features/apt-get-packages"
    ]
}
```


### se puede activar con https://codespaces.new eligiendo el repo correspondiente

* DRAFT PULL REQUEST

https://github.com/nicosistemas/postgres-codespaces/pull/12
