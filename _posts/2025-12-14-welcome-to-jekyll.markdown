---
layout: post
title: "Análisis y Solución: Control de Stock Crítico en SOS Food (PHP/Laravel)"
date: 2025-12-15 10:00:00 -0500 
author: "Juan Jesús Torres Aspajo"
categories: [FullStack, PHP, NODE, Desarrollo Web, Algoritmos, Portafolio]
---

# Título: Solución de Stock Crítico en un Ambiente FoodTech
*Autor: Juan Jesús Torres Aspajo, Estudiante de 4to Semestre, Informática y Desarrollo de Aplicaciones Web - SENATI*

Mi especialidad es el **Desarrollo Web Full-Stack**, manejando lenguajes como **PHP, Java, HTML, CSS, NODE.js, SCSS, etc.** Para este proyecto en mi primera experiencia con SOS Food, utilicé **XAMPP** como entorno de desarrollo local, donde interconecté eficientemente mi lógica de *backend* (PHP) con el *frontend*. El desafío fue aplicar mis conocimientos de arquitectura MVC para desarrollar un sistema de alerta de stock crítico.

---

## 1. El Reto y el Diseño de la Solución

El reto era crear un mecanismo eficiente que notificara al inventario de SOS Food cuando el stock de cualquier ingrediente cayera por debajo de un umbral específico. Opté por utilizar un *Scope* de Eloquent en el modelo de Laravel por su limpieza y reusabilidad.

## 2. El Código Fuente (PHP/Laravel)

El siguiente código se encuentra en el modelo `Ingredient` y nos permite consultar rápidamente los ítems críticos desde cualquier controlador.

{% highlight php %}
// app/Models/Ingredient.php

use Illuminate\Database\Eloquent\Builder;

class Ingredient extends Model
{
    // ... otros atributos y métodos

    /**
     * Scope para identificar ingredientes con un nivel de stock bajo o "crítico".
     */
    public function scopeCriticalStock(Builder $query): Builder
    {
        // Se define un umbral crítico de 10 unidades.
        $critical_threshold = 10; 

        return $query->where('current_stock', '<=', $critical_threshold);
    }
}
{% endhighlight %}

## 3. Valor Agregado como Desarrollador Júnior

Haber diseñado e implementado esta función como parte de mi experiencia inicial en SOS Food subraya mi compromiso con las metodologías modernas de desarrollo web (como el patrón MVC) y mi habilidad para entregar valor desde el comienzo de mi carrera profesional.