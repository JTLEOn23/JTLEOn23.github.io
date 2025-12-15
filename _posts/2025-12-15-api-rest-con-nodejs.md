---
title: "Creando una API REST simple con Express y NODE.js"
date: 2025-12-15
categories:
  - Desarrollo Web
  - Backend
tags:
  - NODE.js
  - Express
  - REST
  - JavaScript
last_modified_at: 2025-12-15
layout: single
---

## 🚀 Introducción

Como desarrollador Full-Stack, es crucial dominar las tecnologías del lado del servidor que permiten la comunicación de datos. En este post, mostraré cómo implementar una API REST básica utilizando **NODE.js** y el popular framework **Express** para gestionar una colección simple de productos.

### Requisitos Previos

Antes de empezar, necesitas tener instalado:
* NODE.js (versión 16+)
* npm (gestor de paquetes)

## 🛠️ Configuración del Proyecto

### 1. Inicialización e Instalación de Express

Primero, crea tu carpeta de proyecto e inicializa `npm` (estos pasos son solo explicativos, no necesitas hacerlos en tu blog):

```bash
mkdir proyecto-api-node
cd proyecto-api-node
npm init -y
npm install express