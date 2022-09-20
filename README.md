# Challenge population mysql :writing_hand:

Desafio: superar los tests haciendo uso de consultas en sql.

## Entorno

Asegurarse de tener instalado `git` . Esto se puede revisar muy facilmente a trevez del comando `git --version` . En caso de no estar instalado, se puede hacer a travez de los siguientes paso

- En linux, a travez del comando `sudo apt install git`.
- En Windows, a travez de la pagina oficial https://git-scm.com/

Procurar tener actualizado `node.js` a la versión lts. Para saber si Node.js esta instalado en su sistema, abra una terminal y ejecute el siguiente comando `npm doctor`. El resultado debe ser la versión de `node ` y `npm`instalada. Si el comando no se encuentra o no se encuentran actualizados, se puede instalar `Node.js` mediante alguno de los siguientes pasos

- En windows, desde la [pagina oficial](https://nodejs.org/en/), descargando y ejecutando la versión `lts`.
- En Linux, a través de `nvm`.
    - Abrir una terminal y ejecutar alguno de los siguientes comando
      
        ```bash
        curl -o- [https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh](https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh) | bash
        ```
        
        ```bash
        wget -qO- [https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh](https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh) | bash
        ```
        
    - Cerrar la terminal y abrir otra para ejecutar el siguiente comando para verificar la correcta instalación`nvm --version` . Una vez observada la versión, ejecutar el siguiente comando para instalar Node.js
      
        ```bash
        nvm install --lts
        ```


## Instalación y ejecución

- 🛠Para instalar las dependencias ejecutar el comando `npm install`

- ⚒Para ejecutar el modo playground o repl, ejecutar el comando `npm run dev`

- 🔧Para traducir el código en `/src` a `JavaScript` , usar el comando `npm run build`

- 🔑Para ejecutar el código con `Node.js`, usar el comando `npm run start`

- 🧪Para ejecutar los test con jest, usar el comando `npm run test`

- 🧪Para ejecutar los test de cobertura, usar el comando `npm run test:coverage`

## Variables de entorno

- `BDD_HOST`: host de la base de datos, por defecto es `localhost`
- `BDD_USER`: usuario para acceder a la base de datos, por defecto es `root`
- `BDD_PASS`: contraseña para acceder a la base de datos, por defecto es `newpass`

Se puede usar el archivo `.env` para configurar estas variables de entorno en testing y desarrollo. Solo se debe ejecutar el comando `cp .env.example .env`.

## Características

- [TypeScript](https://www.typescriptlang.org/)
- [Jest](https://jestjs.io/)
- [mysql2](https://www.npmjs.com/package/mysql2)
