# Documentación Básica de React y Backend con Node.js

## Introducción
Node.js permite ejecutar JavaScript en el servidor, facilitando la creación de aplicaciones backend escalables.

### Node.js
1. **Conceptos básicos**
   - Instalación y configuración
   - Módulos y paquetes (require, `npm` y `yarn`)
2. **Creación de un servidor básico**
   - Uso del módulo `http`
   - Uso de frameworks como Express.js
3. **Rutas**
   - Definición de rutas GET, POST, PUT, DELETE
4. **Middleware**
   - Funciones como `next()` en Express.js
   - Uso de middleware como `body-parser`
5. **Gestión de bases de datos**
   - Conexión con bases de datos como MongoDB o MySQL
6. **Autenticación y seguridad**
   - Uso de `jsonwebtoken` para autenticación
   - CORS y protección de rutas

---

## Ejercicios Propuestos

1. **Servidor básico**
   - Crea un servidor que responda con "Hola Mundo" al acceder a la ruta principal.

```javascript
const http = require('http');

const server = http.createServer((req, res) => {
    res.statusCode = 200;
    res.setHeader('Content-Type', 'text/plain');
    res.end('Hola Mundo');
});

server.listen(3000, () => {
    console.log('Servidor corriendo en http://localhost:3000');
});
```

2. **API con Express**
   - Crea un servidor con Express y define rutas básicas para obtener y agregar datos.

```javascript
const express = require('express');
const app = express();

app.use(express.json());

const datos = [];

app.get('/datos', (req, res) => {
    res.json(datos);
});

app.post('/datos', (req, res) => {
    datos.push(req.body);
    res.status(201).send('Dato agregado');
});

app.listen(3000, () => {
    console.log('Servidor escuchando en http://localhost:3000');
});
```

3. **Conexión con MongoDB**
   - Usa `mongoose` para guardar y recuperar datos en una base de datos MongoDB.

```javascript
const mongoose = require('mongoose');

mongoose.connect('mongodb://localhost/miapp', { useNewUrlParser: true, useUnifiedTopology: true });

const esquema = new mongoose.Schema({ nombre: String });
const Modelo = mongoose.model('Elemento', esquema);

const elemento = new Modelo({ nombre: 'Ejemplo' });

elemento.save().then(() => console.log('Elemento guardado'));
```

---

## Proyecto Final
- Implementa la API para manejar los datos (crear, leer, actualizar, eliminar).

## Recursos Adicionales
- [Express.js Documentation](https://expressjs.com/)
- [MongoDB Documentation](https://www.mongodb.com/docs/)