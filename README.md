### REPO UTILIZADO PARA PROBAR CODESPACES Y ISSUES


* PRUEBAS DE ISSUES:

https://github.com/nicosistemas/postgres/issues/1


* CODESPACES:

[algunas maquinas que se pueden usar para codespaces](https://containers.dev/features)

agregas un json en .devcontainer/maquina.json con datos de la máquina, algo asi:

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
