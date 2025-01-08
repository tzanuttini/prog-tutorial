# Documentación Básica de React y Backend con Node.js

## Introducción
React es una biblioteca de JavaScript para construir interfaces de usuario dinámicas y reutilizables.

---

## Temas a Tratar

### React
1. **Conceptos básicos**
   - Componentes (funcionales y de clase)
   - JSX
   - Props y State
2. **Ciclo de vida del componente**
   - Métodos importantes en componentes de clase
   - Uso de hooks como `useEffect`
3. **Gestión de eventos**
   - Eventos como `onClick`, `onChange`
   - Pasar funciones como props
4. **Renderizado condicional**
   - Uso de operadores ternarios y `if`
5. **Listas y keys**
   - Renderizar listas con `map`
   - Uso de keys únicas
6. **Context API**
   - Compartir datos entre componentes sin prop drilling
7. **React Router**
   - Navegación entre páginas
8. **Integración con APIs**
   - Fetching de datos usando `fetch` o `axios`

---

## Ejercicios Propuestos

1. **Crear un componente simple**
   - Haz un componente que reciba un nombre como prop y lo muestre en pantalla.

```jsx
function Saludo({ nombre }) {
    return <h1>Hola, {nombre}!</h1>;
}

export default Saludo;
```

2. **Contador con estado**
   - Crea un componente con botones para incrementar y decrementar un contador.

```jsx
import { useState } from "react";

function Contador() {
    const [contador, setContador] = useState(0);

    return (
        <div>
            <h2>Contador: {contador}</h2>
            <button onClick={() => setContador(contador + 1)}>Incrementar</button>
            <button onClick={() => setContador(contador - 1)}>Decrementar</button>
        </div>
    );
}

export default Contador;
```

3. **Lista dinámica**
   - Crea una lista de tareas donde puedas agregar y eliminar elementos.

---

## Proyecto Final
- Crea una aplicación que permita agregar y mostrar elementos desde una API.

---

## Recursos Adicionales
- [React Documentation](https://reactjs.org/)
- [MDN Web Docs - Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)

