### Características

- Navegación entre páginas mediante un menú interactivo.
- Funcionalidades básicas de lógica implementadas con JavaScript(comparación de números, selección de meses, listas dinámicas).
- Registro de usuarios con validación y almacenamiento en localStorage.
- Visualización de usuarios registrados en una tabla interactiva.
- Diseño responsivo con estilos personalizados en CSS.
- Código implementado exclusivamente con arrow functions.

![Descripción de la imagen](https://raw.githubusercontent.com/JCPB2000/Actividad-de-aprendizaje-2/d691886e17a11eb95908cb5f497e0601ee8ddf15/1.png)

**Estructura del proyecto**

###### actividad-aprendizaje-2
```
│
├── index.html             # Página principal con datos del estudiante
├── funciones.html         # Funciones lógicas (comparar números, meses, listas)
├── registro.html          # Formulario para registrar usuarios
├── resultados.html        # Tabla con usuarios registrados
│
├── css/
│   └── estilo.css         # Estilos compartidos para todas las páginas
│
├── scripts/
│   ├── acciones.js        # Funciones generales
│   ├── funciones.js       # Comparación y gestión lógica
│   ├── registro.js        # Registro de usuarios
│   └── resultados.js      # Visualización de datos
│
└── README.md              # Documentación del proyecto
```

##Implementación

###### Funcionalidades
1- Inicio
-Muestra los datos del estudiante en un diseño organizado.
2- Funciones lógicas
-Comparación de números con condicionales if.
-Identificación de meses con switch.
-Gestión de una lista dinámica de nombres usando arrays.
3- 	Registro de usuarios
-Formulario validado para capturar datos del usuario.
-Campos: ID, Cédula, Nombres, Fecha de nacimiento, Ciudad.
4- Resultados
-Muestra los usuarios registrados en formato tabular.



###Código Destacado

JavaScript: Comparación de Números
 document.getElementById('btn-comparar').addEventListener('click', () => {
    const num1 = parseFloat(document.getElementById('input1').value);
    const num2 = parseFloat(document.getElementById('input2').value);
    const resultado = num1 > num2 ? `${num1} es mayor` : num1 < num2 ? `${num2} es mayor` : "Son iguales";
    document.getElementById('resultado').textContent = resultado;
});



####Javascript　
##### Comparación de Números

```javascript
document.getElementById('btn-comparar').addEventListener('click', () => {
    const num1 = parseFloat(document.getElementById('input1').value);
    const num2 = parseFloat(document.getElementById('input2').value);
    const resultado = num1 > num2 ? `${num1} es mayor` : num1 < num2 ? `${num2} es mayor` : "Son iguales";
    document.getElementById('resultado').textContent = resultado;
});
```

####HTML
##### Registro de usuarios
```html
<form id="formulario">
    <input type="text" id="id-usuario" placeholder="ID" required>
    <input type="text" id="cedula-usuario" placeholder="Cédula" required>
    <input type="text" id="nombres-usuario" placeholder="Nombres" required>
    <input type="date" id="fecha-usuario" required>
    <select id="ciudad-usuario" required>
        <option value="Quito">Quito</option>
        <option value="Guayaquil">Guayaquil</option>
    </select>
    <button type="button" id="registrar-btn">Registrar</button>
</form>

```
####CSS
##### Registro de usuarios
```css
/* Estilo general del cuerpo de la página */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

/* Cabecera del formulario */
header {
    background-color: #0e6b0b;
    color: white;
    padding: 15px 0;
    text-align: center;
}

/* Barra de navegación */
nav ul {
    list-style: none;
    background-color: #333;
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    text-decoration: none;
    color: white;
    padding: 10px 20px;
}

/* Contenedor principal del formulario */
main {
    padding: 20px;
    background: white;
    margin: 20px auto;
    border-radius: 5px;
    max-width: 400px;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
}

/* Formulario en disposición vertical */
form {
    display: flex;
    flex-direction: column;
    gap: 15px;
}

/* Estilo de las etiquetas */
form label {
    font-weight: bold;
    margin-bottom: 5px;
}

/* Estilo de los campos de entrada */
form input, form select, form button {
    padding: 10px;
    font-size: 16px;
    border: 1px solid #ddd;
    border-radius: 5px;
    width: 100%;
    box-sizing: border-box;
}

/* Efecto al enfocar los campos */
form input:focus, form select:focus {
    outline: none;
    border-color: #007bff;
    box-shadow: 0px 0px 5px rgba(0, 123, 255, 0.5);
}

/* Botón del formulario */
form button {
    background-color: #007bff;
    color: white;
    border: none;
    cursor: pointer;
    transition: background-color 0.3s;
}

/* Efecto al pasar el mouse sobre el botón */
form button:hover {
    background-color: #0056b3;
}

/* Estilo del título principal */
h1 {
    text-align: center;
    color: #fff7f7;
}
```


###FIN
