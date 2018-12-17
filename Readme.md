# Ejercicios del curso de confección de páginas web #

## Configuración del entorno ##

- Navegador: Chrome, firefox... (usando F12)
- Editor de código: Visual Studio Code
    https://code.visualstudio.com
- Node JS / npm
    https://nodejs.org/es
- Servidor web de desarrollo: ej http-server
    npm install -g http-server
- Git
    https://git-scm.com
- Github
    https://github.com

### Configuración de git
- Definir usuario / correo
    git config --global user.name <nombreusuario>
    git config --globa user.email <emailusuario>
- Comprobar la configuración
    git config -l --global
- Crear un repositorio: 2 formas
    1. Crearlo en local y luego sincronizar en remoto
        Inicializar el repositorio:
            git init <nombrecarpeta>
        Opcionalmente, hacer un primer commit para que no vaya vacío, por ej desde Visual Studio Code
            En Visual Studio Code se hace el commit desde el tirachinas
        Comprobar el commit:
                git log
        Crear un repositorio vacío en GitHub, preferiblemente con el mismo nombre
        Seguir las instrucciones de GitHub para sincronizar los repositorios (2 comandos)
            git remote add origin https://github.com/Amgsan/<repositorio>.git
            git push -u origin master
        Se puede publicar (subir al repositorio) o sincronizar (sube y baja)
        También se puede hacer el commit desde la linea de comandos, pero en 2 pasos:
            git status (para saber lo que hay pendiente de subir)
            git add .
            git commit -m <nombredelcommit>
    2. De remoto a local    
        Entrar en GitHub
        Clonar el repositorio: copiar el nombre del repositorio y ejecutarlo en cmd
            git clone <nombrerepositorio>.git
Para que no haga copias de algún fichero crear el fichero .gitignore
    En internet https://www.gitignore.io ayuda a crear este fichero según el tipo de desarrollo