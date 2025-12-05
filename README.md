# 👨‍💻 **Arley Gustavo Rozo Rodríguez**  

### **🚀 Futuro Desarrollador de Software | Campuslands 2025**

[![GitHub Followers](https://img.shields.io/github/followers/Arleyrozo27?style=social)](https://github.com/Arleyrozo27)
[![GitHub Stars](https://img.shields.io/github/stars/Arleyrozo27?style=social)](https://github.com/Arleyrozo27)
[![Visitors](https://visitor-badge.laobi.icu/badge?page_id=Arleyrozo27.Arleyrozo27)](https://github.com/Arleyrozo27)

---

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)

---

## 📌 **Portada del Repositorio**

> "Este repositorio representa mi evolución como desarrollador de software. Cada proyecto aquí documentado aplica las mejores prácticas de la industria, arquitecturas escalables y metodologías ágiles aprendidas en Campuslands."

**✨ Este repositorio cumple con todos los estándares profesionales:**
- ✅ **Arquitectura limpia** con tecnologías enseñadas en Campuslands
- ✅ **Documentación exhaustiva** para fácil mantenimiento
- ✅ **Commits profesionales** siguiendo Conventional Commits
- ✅ **Despliegue en GitHub Pages** para frontend
- ✅ **Metodologías ágiles** (Scrum) completamente documentadas
- ✅ **APIs RESTful** con Spring Boot y Python

---

## 🏆 **Proyectos Campuslands**

### **🎯 Proyecto 1: Sistema de Gestión con Spring Boot**
*Estado: En desarrollo | Tecnologías: Java, Spring Boot, MySQL*

```java
// Ejemplo de código - UserController.java

@RestController
@RequestMapping("/api/users")
public class UserController {
    
    @Autowired
    private UserService userService;
    
    @GetMapping
    public ResponseEntity<List<UserDTO>> getAllUsers() {
        return ResponseEntity.ok(userService.findAll());
    }
    
    @PostMapping
    public ResponseEntity<UserDTO> createUser(@Valid @RequestBody UserRequest request) {
        return ResponseEntity.status(HttpStatus.CREATED)
               .body(userService.createUser(request));
    }
}

```
-----

Características:

✅ API REST con Spring Boot

✅ Conexión a MySQL con Spring Data JPA

✅ Validación de datos con Bean Validation

✅ Manejo de excepciones global

Estructura del proyecto:

````
src/
├── main/
│   ├── java/
│   │   └── com/
│   │       └── arley/
│   │           └── sistema/
│   │               ├── controller/
│   │               ├── service/
│   │               ├── repository/
│   │               ├── model/
│   │               └── dto/
│   └── resources/
│       ├── application.properties
│       └── data.sql
└── test/
    └── java/
        └── com/
            └── arley/
                └── sistema/
                    └── controller/

````

### **📊 Proyecto 2: API con Python y PostgreSQL**
*Estado: Completado | Tecnologías: Python, PostgreSQL, FastAPI*

### **python**

````
# Ejemplo de código - main.py

from fastapi import FastAPI, HTTPException
from pydantic import BaseModel
import psycopg2

app = FastAPI()

class Item(BaseModel):
    name: str
    price: float

@app.get("/items/")
async def read_items():
    conn = psycopg2.connect(
        host="localhost",
        database="mydatabase",
        user="myuser",
        password="mypassword"
    )
    cur = conn.cursor()
    cur.execute("SELECT * FROM items")
    items = cur.fetchall()
    cur.close()
    conn.close()
    return {"items": items}

@app.post("/items/")
async def create_item(item: Item):

    # Lógica para crear item en PostgreSQL
    return {"message": "Item creado", "item": item}

````

### **🌐 Proyecto 3: Portafolio Web Responsive**
*Estado: Completado | Tecnologías: HTML, CSS, JavaScript*

#### **html**

```
<!-- Ejemplo de código - index.html -->
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portafolio Arley Rozo</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>👨‍💻 Arley Rozo</h1>
        <p>Desarrollador Full Stack en formación</p>
    </header>
    
    <section id="proyectos">
        <h2>Mis Proyectos</h2>
        <div class="proyecto">
            <h3>Sistema de Gestión</h3>
            <p>Spring Boot + MySQL</p>
        </div>
    </section>
</body>
</html>
```

#### **CSS**

```
/* Ejemplo de código - styles.css */

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #333;
    color: white;
    padding: 2rem;
    text-align: center;
}

.proyecto {
    border: 1px solid #ddd;
    padding: 1rem;
    margin: 1rem;
    border-radius: 5px;
}

```
---

## **🛠️ Stack Tecnológico (Campuslands)**

### **💻 Backend:**

*Java - Programación orientada a objetos*

*Spring Boot - Framework para aplicaciones Java*

*Python - Desarrollo rápido de aplicaciones*

---
### **🌐 Frontend:**

*HTML5 - Estructura web*

*CSS3 - Estilos y diseño responsive*

*JavaScript - Interactividad en el navegador*

---
### **🗄️ Bases de Datos:**

*MySQL - Sistema de gestión de bases de datos relacional*

*PostgreSQL - Base de datos relacional avanzada*

---
### **🔧 Herramientas:**

*Git - Control de versiones*

*GitHub - Repositorio y colaboración*

*Postman - Pruebas de APIs*

---

### **🏗️ Arquitectura de Proyectos**

*Estructura para proyecto Spring Boot:*

````

proyecto-spring-boot/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── arley/
│   │   │           └── proyecto/
│   │   │               ├── ProyectoApplication.java
│   │   │               ├── controller/
│   │   │               │   └── UserController.java
│   │   │               ├── service/
│   │   │               │   └── UserService.java
│   │   │               ├── repository/
│   │   │               │   └── UserRepository.java
│   │   │               ├── model/
│   │   │               │   └── User.java
│   │   │               └── dto/
│   │   │                   └── UserDTO.java
│   │   └── resources/
│   │       ├── application.properties
│   │       ├── static/
│   │       └── templates/
│   └── test/
│       └── java/
│           └── com/
│               └── arley/
│                   └── proyecto/
│                       └── ProyectoApplicationTests.java
├── pom.xml
└── README.md

````

*Estructura para proyecto web (HTML/CSS/JS):*

````

proyecto-web/
├── index.html
├── styles.css
├── script.js
├── images/
│   └── logo.png
├── pages/
│   ├── about.html
│   └── contact.html
└── README.md

````

`*Estructura para proyecto Python:*

````
proyecto-python/
├── main.py
├── requirements.txt
├── modules/
│   ├── __init__.py
│   ├── database.py
│   └── utils.py
├── tests/
│   └── test_main.py
└── README.md

````

---

## 🤝 **Trabajo Colaborativo**

### **Flujo de trabajo con Git:**

Crear rama para nueva característica:
   
```
git checkout -b feature/nueva-funcionalidad
Hacer commits descriptivos:


git add .
git commit -m "feat: ✨ agregar funcionalidad X"
Subir cambios:


git push origin feature/nueva-funcionalidad
Crear Pull Request en GitHub

```

---

Buenas prácticas que aplico:

✅ Commits pequeños y frecuentes

✅ Mensajes de commit descriptivos

✅ Pull Requests con descripción clara

✅ Code review entre compañeros

✅ Mantener main branch estable

---

## **🎓 Formación en Campuslands**

### *Tecnologías aprendidas:*

#### Java: Fundamentos, POO, Spring Boot

#### Python: Sintaxis, estructuras de datos, APIs

#### Frontend: HTML5, CSS3, JavaScript básico

#### Bases de datos: MySQL, PostgreSQL, consultas SQL

#### Git y GitHub: Control de versiones y colaboración

---

### *Proyectos desarrollados:*

#### Sistema de gestión con Spring Boot y MySQL

#### API REST con Python y PostgreSQL

#### Portafolio web responsive con HTML/CSS/JS

#### Aplicaciones web con Java EE

---

### *Metodologías aplicadas:*

Desarrollo ágil con Scrum

Control de versiones con Git

Code review entre compañeros

Documentación de proyectos

---

## **📫 Contacto**
### Información de contacto:


### 📧 Email: arleyrodriguez280@gmail.com

### 💼 LinkedIn: https://www.linkedin.com/in/estudiante-backen-arley-rozo

### 🌐 Portafolio: https://portafolio-arley-rozo.onrender.com

### 🐙 GitHub: https://github.com/Arleyrozo27

---

## **Disponibilidad:**

### 🔍 Buscando: Práctica profesional o puesto junior

### 📍 Modalidad: Presencial o remoto

### ⏰ Tiempo: Tiempo completo

### 🎯 Objetivos 2025

---

## **Metas profesionales:**

### 👨‍💻 Conseguir primera experiencia como desarrollador

### 📚 Dominar Spring Boot y desarrollo backend

### 🌐 Aprender más sobre frontend moderno

### 🤝 Contribuir a proyectos open source

---

<div align="center">
    
## **⭐ ¡Gracias por visitar mi perfil!**

### **"El mejor momento para plantar un árbol fue hace veinte años. El segundo mejor momento es ahora."**

### **Siempre aprendiendo, siempre mejorando 🚀**

</div> 

