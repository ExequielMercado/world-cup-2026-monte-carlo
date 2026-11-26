# Predictor Estadístico Mundial FIFA 2026 — Simulación Monte Carlo & Backtesting

Aplicación web interactiva de analítica deportiva que modela y estima las probabilidades de resultado de los **72 partidos de la fase de grupos del Mundial FIFA 2026** (12 grupos, A–L), calculando **432 probabilidades trazables** mediante un enfoque cuantitativo explícito en **HTML5, CSS3 y JavaScript puro** (arquitectura *serverless* sin backend propio).

🔗 **Demo Interactiva en Vivo:** [exequielmercado.github.io/world-cup-2026-monte-carlo](https://exequielmercado.github.io/world-cup-2026-monte-carlo/)

---

## 🎯 Problema que Resuelve
Los pronósticos deportivos tradicionales suelen basarse en apreciaciones subjetivas sin trazabilidad. Este proyecto reemplaza la intuición por un **modelo estadístico auditado y reproducible**, donde cada encuentro cuenta con un desglose cuantitativo y cada probabilidad puede rastrearse hasta las variables históricas y contextuales que la originan.

---

## 🧮 Metodología y Arquitectura del Modelo

El motor de cálculo procesa los datos en un pipeline de **5 etapas**:
1. **Recolección y normalización** de indicadores multi-fuente.
2. **Evaluación de fuerza relativa** ofensiva y defensiva por selección.
3. **Ajuste de probabilidades** mediante ponderación multifactorial.
4. **Simulación estocástica** de escenarios de partido.
5. **Consolidación y auditoría** de probabilidades finales vs. resultados reales (*backtesting*).

### Variables y Ponderaciones
| Variable | Peso | Fuente de Datos |
| :--- | :---: | :--- |
| **Rating Elo Internacional** | **35%** | Elo Ratings |
| **Forma Reciente (últimos 10 partidos)** | **25%** | Registros públicos de rendimiento |
| **Calidad del Plantel (Valor de mercado)** | **15%** | Transfermarkt |
| **Expected Goals (xG ofensivo y defensivo)** | **15%** | FBref |
| **Lesiones y Ausencias Clave** | **5%** | Reportes oficiales de convocatoria |
| **Factores Contextuales (localía / viaje)** | **5%** | Parámetros de sede y calendario |

### Motor de Simulación Monte Carlo / Poisson
Para proyectar distribuciones de goles y resultados (Victoria Local, Empate, Victoria Visitante), el sistema ejecuta **100.000 iteraciones Monte Carlo** bajo un esquema de **distribución de Poisson**, generando estimaciones calibradas y transparentes sobre sus márgenes de incertidumbre.

---

## 📊 Funcionalidades Principales
* **Explorador de Fase de Grupos (72 Partidos):** Filtrado dinámico por grupo (A–L) con desglose de probabilidades y variables por encuentro.
* **Comparador Radar Cara a Cara:** Selección de dos equipos nacionales para contrastar visualmente su rendimiento en 5 dimensiones (*Elo, xG, Goles, Valor de Mercado y Forma*).
* **Ranking Probabilístico de Candidatos:** Distribución de probabilidades de campeón antes del inicio del torneo (destacando a Francia 16,8%, España 16,2% y Argentina 12,4%).
* **Auditoría & Backtesting Post-Torneo:** Contraste directo entre las probabilidades estimadas pre-partido y los marcadores reales ocurridos durante el certamen.
* **Transparencia Metodológica:** Documentación abierta dentro de la interfaz sobre supuestos estadísticos, alcance y limitaciones del modelo.

---

## 🛠️ Stack Tecnológico
* **Frontend & Lógica Estadística:** JavaScript (ES6+), HTML5, CSS3.
* **Visualización de Datos:** Gráficos radar interactivos y tablas dinámicas.
* **Despliegue:** GitHub Pages (CI/CD estático).

---

## 👨‍💻 Autor
**Exequiel David Mercado** — Analista de Datos & Operaciones (GTR / BI) | Automatización con IA  
* **GitHub:** [github.com/ExequielMercado](https://github.com/ExequielMercado)
* **LinkedIn:** [linkedin.com/in/exequiel-mercado-9b38561ab](https://www.linkedin.com/in/exequiel-mercado-9b38561ab/)
