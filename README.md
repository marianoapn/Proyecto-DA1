# 📦 NearDupFinder

Sistema de gestión de catálogo con detección automática de ítems duplicados, desarrollado en **.NET 8 con Blazor Server** y arquitectura en capas.

## 🧠 Descripción

NearDupFinder permite gestionar catálogos de productos evitando duplicados mediante algoritmos de similitud textual.

Cada vez que se crea o modifica un ítem, el sistema analiza posibles duplicados utilizando:

- Similitud de texto (**Jaccard**)
- Distancia de strings (**Levenshtein**)
- Coincidencias de atributos (marca, modelo)

Esto permite mantener la consistencia de datos, evitando errores en stock, precios y reportes.

## 🏗️ Arquitectura

El sistema está dividido en 5 capas principales:

- Interfaz (Blazor)
- Lógica de negocio
- Dominio
- Abstracciones (interfaces)
- Persistencia (Entity Framework)

### Características

- ✔ Bajo acoplamiento
- ✔ Alta cohesión
- ✔ Aplicación de principios SOLID y GRASP

## ⚙️ Tecnologías

- .NET 8
- Blazor Server
- Entity Framework Core
- SQL Server (Azure SQL Edge)
- Docker
- MSTest (TDD)
- Lucene.Net (procesamiento de texto)

## 🧪 Testing

- ✔ +400 tests
- ✔ ~98% cobertura de código
- ✔ Enfoque TDD (Test-Driven Development)

## 🚀 Funcionalidades principales

- Gestión de usuarios y autenticación
- CRUD de catálogos e ítems
- Detección automática de duplicados
- Clustering de productos similares
- Reserva de stock
- Notificaciones automáticas
- Auditoría de acciones
- Importación/exportación (CSV / XLSX)

## 🐳 Ejecución con Docker

```bash
docker-compose up -d
```
## 🔑 Credenciales de prueba

Usuario: admin@gmail.com  
Contraseña: 123QWEasdzxc@

## 📊 Base de datos

El sistema utiliza **Entity Framework Code First**, generando automáticamente las tablas a partir del modelo de dominio.

## 🧠 Conceptos aplicados

- Clean Architecture (inspirado)
- Repository Pattern
- Strategy Pattern
- DTO Pattern
- Dependency Injection
- Procesamiento de texto (stemming + stopwords)
