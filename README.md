# Practica: Despliegue Continuo con GitHub Actions y Surge.sh

Este repositorio contiene la solucion de la practica de despliegue continuo de una pagina web estatica hacia Surge.sh mediante GitHub Actions.

## Estudiante
- Nombre: Eduard Tejada
- Institucion: Instituto Tecnologico de Las Americas (ITLA)
- Materia: DevOps / Electiva

## Estructura del Proyecto
- `index.html`: Pagina web principal de la practica.
- `.github/workflows/main.yaml`: Flujo de trabajo de GitHub Actions para el despliegue automatico hacia Surge.sh.
- `.gitignore`: Archivos y carpetas ignorados por Git.

## Requisitos y Configuracion
1. Instalacion de Surge CLI:
   ```bash
   npm install --global surge
   ```

2. Secretos de GitHub configurados en el repositorio:
   - `SURGE_TOKEN`: Token de autenticacion de la cuenta en Surge.sh.
   - `SURGE_DOMAIN`: Dominio personalizado de Surge (por ejemplo: eduardtejada-practica-surge.surge.sh).
   - `SURGE_LOGIN`: Correo electronico registrado en Surge.sh.

## Despliegue
Cada vez que se realiza un commit y push a la rama `main`, GitHub Actions ejecuta automaticamente el workflow y publica los cambios en Surge.sh.
