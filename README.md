# Pugstagram

Proyecto realizado en Svelte

Link demo: https://cyara-pugstagram.netlify.app

# Svelte



# Sapper
```
 npm install sapper --save-dev

 npm install polka compression sirv
```
### polka 

Versión mínima de express, nos va servir para crear el servidor

### compression

Nos ayuda a comprimir nuestros archivos

### sirv

Nos ayuda a publicar nuestro sitio de mejor forma con los archivos estáticos

### Archivo .env

Se añaden las variables de entorno.

### Archivo server.js

Ahí se construye el proyecto (se hacen las importaciones de poka, sirv, compression y se hace el llamado de las variables de entorno.

### Archivo client.js

Se hace la configuración del proyecto para trabajar con Svelte y Sapper.

# Sapper Environment

```
npm install sapper-environment
```
https://www.npmjs.com/package/sapper-environment
https://github.com/JpCapdevila/sapper-environment/blob/master/README.md


# Netlify:

### Svelte:
[build]
    command = "npm run build"
    publish = "dist/"

### Sapper:
[build]
    command = "npm run export"
    publish = "__sapper__/export"


# Heroku

### Sapper




| Nombre  |  Email |
| ------------ | ------------ |
|  Cristhian Yara |  cmyarap@gmail.com |