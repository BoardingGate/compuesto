# ⚡ BoardingGate | Calculadora de Interés Compuesto y Renta de Jubilación

Simulador financiero avanzado de **acumulación de patrimonio** y **desacumulación ordenada (fase de retiro/jubilación)**, desarrollado por **BoardingGate**.

---

## 🌐 Enlaces de Acceso Rápido

* **Plataforma Integral de Inversión en Bolsa:** [https://boardinggate.github.io/BOLSA/BOLSA2.HTML](https://boardinggate.github.io/BOLSA/BOLSA2.HTML)
* **Contacto y Actualizaciones:** [@BoardingGate en X (Twitter)](https://x.com/boardinggate)

---

## 📌 Características Principales

### 1. Fase de Creación de Patrimonio (Acumulación)
* **Ajuste Real por Inflación:** Cálculo simultáneo del valor nominal íntegro y del poder adquisitivo real (descontando la inflación anual proyectada).
* **Parámetros Temporales y del Sujeto:** Configuración del año de partida y edad actual, proyectando con exactitud a qué año calendario y a qué edad finalizarán las aportaciones.
* **Capitalización Flexible:** Simulación de frecuencia de capitalización (de 1 a 12 veces por año) y momento de las aportaciones (inicio o final de periodo).
* **Hitos de Rentabilidad (Baggers):** Identificación automática de multiplicadores patrimoniales (`1-Bagger`, `2-Bagger`, etc.) a lo largo del tiempo.
* **Punto de Inflexión:** Detección del año exacto en el que los intereses generados superan al capital total aportado por el inversor.
* **Desglose Anual Detallado:** Tabla desplegable año a año con fechas, edades, aportaciones acumuladas, intereses generados, valor nominal y valor real.

### 2. Fase de Retiro y Renta de Jubilación (Desacumulación)
Permite estimar el consumo del capital alcanzado al finalizar el periodo de ahorro, asumiendo que el saldo remanente que aún no se ha extraído continúa revalorizándose en el mercado al tipo de interés pactado:

* **Modo A: Fijar Renta Mensual Deseada:**
  * Determina cuántos meses y años de disponibilidad real ofrece el fondo hasta agotarse por completo.
  * Si la renta mensual solicitada es menor o igual a los rendimientos generados por el capital, alerta de **renta vitalicia/perpetua** (el capital principal no se agota nunca).
  * Informa del año exacto y edad a la que se extinguiría el fondo.
* **Modo B: Fijar Plazo de Cobertura en Años:**
  * Calcula la **renta mensual máxima extraíble** para consumir ordenadamente el patrimonio durante los años elegidos (ej. 20, 25 o 30 años de jubilación).
  * Informa de las fechas y edades cubiertas (desde el inicio del retiro hasta su conclusión).
* **Base de Cálculo Seleccionable:** Posibilidad de conmutar entre el capital nominal total o el capital en términos de poder adquisitivo real deflactado.
* **Desglose Desacumulación Año a Año:** Tabla independiente que muestra para cada año de retiro: saldo inicial, retiros acumulados (12 pagas), rendimientos anuales generados por el saldo vivo y saldo remanente al cierre.

---

## 🛠️ Tecnologías y Arquitectura

* **Página Web Única (SPA Autocontenida):** Ejecutable en local con doble clic o alojable en cualquier servidor estático (GitHub Pages, Vercel, Netlify).
* **React 18 & Babel Standalone:** Lógica reactiva sin necesidad de proceso de compilación previo (`Node.js`/`npm`).
* **Tailwind CSS:** Diseño moderno, responsivo y adaptado para dispositivos móviles, tablets y monitores de escritorio.
* **Persistencia Local:** Los datos introducidos se preservan automáticamente en el almacenamiento local del navegador (`localStorage`).

---

## 🚀 Instalación y Despliegue

1. Clona o descarga este repositorio:
   ```bash
   git clone https://github.com/boardinggate/BOLSA.git
