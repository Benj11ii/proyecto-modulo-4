# Gestor Inteligente de Clientes (GIC)

## Descripción General

El Gestor Inteligente de Clientes (GIC) es una aplicación desarrollada en Python que implementa el paradigma de Programación Orientada a Objetos (POO) para la gestión de clientes. El sistema permite administrar distintos tipos de clientes, aplicar validaciones, registrar actividades y persistir información mediante archivos.

Este proyecto corresponde al Módulo 4 del programa Python Trainee – SENCE.

Repositorio del proyecto:  
https://github.com/Benj11ii/proyecto-modulo-4/tree/main

---

## Contexto del Problema

La empresa SolutionTech ha identificado la necesidad de modernizar su sistema de gestión de clientes, actualmente realizado de forma manual, lo que ha provocado duplicación de datos, falta de validaciones y dificultades para escalar el sistema.

La solución propuesta consiste en desarrollar una plataforma en Python, modular y escalable, capaz de integrarse con servicios externos.

---

## Objetivo del Proyecto

Desarrollar una plataforma basada en Programación Orientada a Objetos que permita:

- Gestionar clientes de distintos tipos
- Aplicar validaciones de datos
- Registrar actividades del sistema
- Persistir información en archivos
- Simular integración con APIs externas

---

## Estructura del Proyecto

El proyecto se organiza en los siguientes archivos:

- **main.py**  
  Archivo principal que inicia la ejecución del sistema.

- **menu_inicial.py**  
  Contiene el menú principal y la lógica de navegación.

- **modelos.py**  
  Define la clase base Cliente, sus subclases, validadores, getters/setters y el registro de actividad.

- **gestor_archivos.py**  
  Maneja la carga y guardado de datos, incluyendo clientes de prueba.

- **conexion_api_externa.py**  
  Implementa la simulación de validaciones externas y el envío de correos electrónicos.

---

## Programación Orientada a Objetos

El sistema aplica los principios de la POO para asegurar escalabilidad y mantenibilidad:

- Encapsulamiento mediante atributos privados y setters/getters
- Herencia entre la clase Cliente y sus subclases
- Polimorfismo en métodos como `mostrar_perfil()`

La clase Cliente define los atributos y comportamientos comunes, mientras que las clases ClienteRegular, ClientePremium y ClienteCorporativo agregan funcionalidades específicas.

---

## Registro de Actividad

El sistema incorpora la clase RegistroActividad, encargada de almacenar los eventos asociados a cada cliente, permitiendo la trazabilidad y auditoría básica del sistema.

Cada cliente puede contener cero o múltiples registros de actividad.

---

## Diagrama UML

El proyecto incluye un diagrama de clases UML desarrollado con PlantUML, donde se representan:

- Relaciones de herencia entre clases
- Composición entre Cliente y RegistroActividad
- Atributos públicos y privados
- Métodos principales del sistema

---

## Funcionalidades Principales

- Crear, editar y eliminar clientes (CRUD)
- Validar correo electrónico, teléfono y dirección
- Registrar acciones internas del sistema
- Guardar y cargar datos en archivos JSON
- Simular validación y notificación mediante API externa

Se incluye además validación de correo electrónico mediante la API:

https://rapid-email-verifier.fly.dev/api/validate

---

## Conclusiones

El sistema desarrollado cumple con los requerimientos del módulo, aplicando correctamente los principios de la Programación Orientada a Objetos. La solución es funcional, escalable y mantiene la integridad de los datos mediante validaciones y manejo de excepciones.

El proyecto refleja la correcta aplicación de herencia, encapsulamiento y polimorfismo, así como una estructura modular adecuada para su mantenimiento y futura ampliación.
