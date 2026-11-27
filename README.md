<div align="center">

# ⚽ GitFut ES

**Tu perfil de GitHub convertido en Carta Ultimate Team, Auditoría de Repositorios y Duelo 1v1 en el Estadio**

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=2600&pause=800&color=10B981&center=true&vCenter=true&width=680&height=42&lines=Convierte+tu+GitHub+en+una+carta+FUT+interactiva+3D;Eval%C3%BAa+tus+repositorios+y+desbloquea+8+trofeos;Enfr%C3%A9ntate+en+Duelos+1v1+con+partido+animado+5v5" alt="GitFut ES - Carta FUT, Auditoría GitHub y Duelo 1v1">

<br/>

![HTML5](https://img.shields.io/badge/HTML5-Archivo_%C3%9Anico-E34F26?style=flat-square&logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-CDN-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![GitHub API](https://img.shields.io/badge/GitHub-REST_API-181717?style=flat-square&logo=github&logoColor=white)

</div>

---

## 📋 Descripción

**GitFut ES** es una aplicación web 100% del lado del cliente (contenida en [index.html](index.html)) que consume en tiempo real la **API REST pública de GitHub** para transformar cualquier cuenta de desarrollador en una **carta estilo Ultimate Team**, auditar la calidad de sus repositorios y enfrentar a dos programadores en un **Duelo 1v1 con partido caricaturesco animado**.

No requiere servidor, base de datos ni compilación: solo abre [index.html](index.html) en tu navegador.

---

## ✨ Características Principales

### 1. 🃏 Modo Perfil Individual
- **Carta FUT Interactiva 3D**: Efecto de perspectiva y brillo holográfico dinámico al mover el cursor.
- **Exportación y Compartido**: Descarga tu carta como imagen **PNG** (mediante `html2canvas`) o copia un resumen listo para compartir en el portapapeles.
- **Auditoría de Repositorios**: Evalúa repositorios públicos (con filtro opcional para ocultar *forks*), asignando una calificación (`A+` hasta `D`) basada en documentación, licencia, estrellas y actividad.
- **Plan de Entrenamiento (Coaching Técnico)**: Calcula cuánto falta para la siguiente rareza de carta, identifica tu atributo más débil y recomienda acciones concretas sobre tus repositorios.

### 2. ⚡ Modo Duelo 1v1 (VS)
- **Estadio Animado Caricaturesco 5v5**: Al iniciar un duelo, dos equipos de 5 jugadores caricaturescos (Esmeralda FC vs Cian United, con el avatar real de GitHub en cada **Capitán #10**) disputan un partido de `00'` a `90'` sobre un campo SVG con marcador estilo TV, confeti, narración en vivo y efectos de sonido opcionales con Web Audio API (silenciados por defecto).
- **Puntaje Compuesto**: Combina `75% Media General (OVR) + 25% Calidad promedio de repositorios`.
- **Veredicto y Comparativa Cara a Cara**: Enfrenta 12 métricas clave (OVR, calidad de repos, 6 atributos FUT, estrellas, PRs, issues y pushes) junto con el plan de entrenamiento de ambos jugadores.

### 3. 🔑 Soporte Opcional de Token (PAT)
- Funciona sin autenticación con el límite estándar de la API pública de GitHub (**60 peticiones/hora**).
- Puedes ingresar un **Personal Access Token (PAT)** en el panel superior (guardado únicamente en el `localStorage` de tu navegador) para ampliar el límite hasta **5,000 peticiones/hora**.

---

## ⚙️ Cómo se Calculan los Atributos (0–99)

Los seis atributos se calculan mediante **escalado logarítmico** (`logScale`) para evitar inflación artificial y premiar el impacto real y la constancia:

| Atributo | Significado | Señales evaluadas en GitHub |
|:--:|:--|:--|
| **RIT** | Ritmo | Eventos *push* recientes, commits y repositorios activos en los últimos 90 días |
| **TIR** | Tiro | Estrellas totales acumuladas y seguidores |
| **PAS** | Pase | Pull Requests realizados y *forks* generados en tus proyectos |
| **REG** | Regate | Diversidad de lenguajes de programación y repositorios propios |
| **DEF** | Defensa | *Issues* reportados/abiertos, documentación y licencias en repositorios propios |
| **FÍS** | Físico | Años de antigüedad de la cuenta, volumen de repositorios públicos y actividad reciente |

La **Media General (OVR)** pondera estos seis atributos (con un ligero bono por hitos de `1,000+` y `10,000+` estrellas) y determina automáticamente la **posición táctica** (`DC`, `MCO`, `ED`, `DFC`, `MI`, `MCD`, `MC`) y el **arquetipo** del jugador.

### Rarezas de Carta

<div align="center">

![Bronce](https://img.shields.io/badge/BRONCE-%3C65-CD7F32?style=flat-square&labelColor=2A1A0C)
![Plata](https://img.shields.io/badge/PLATA-65--74-AAB2BD?style=flat-square&labelColor=262B33)
![Oro](https://img.shields.io/badge/ORO-75--84-E6B422?style=flat-square&labelColor=3A2806)
![Especial TOTY](https://img.shields.io/badge/ESPECIAL_TOTY-85--91-3B7AFF?style=flat-square&labelColor=10254F)
![Ícono Legendario](https://img.shields.io/badge/%C3%8DCONO_LEGENDARIO-92%2B-EAB308?style=flat-square&labelColor=1E293B)

</div>

---

## 🏆 Vitrina de Trofeos (8 Logros Desbloqueables)

Cada perfil individual evalúa automáticamente 8 trofeos según sus métricas reales:

| Trofeo | Condición para desbloquear |
| :--- | :--- |
| **Balón de Oro Open Source** | Alcanzar una Media General (`OVR`) de **88 o superior** |
| **Bota de Oro de Estrellas** | Acumular **500 o más estrellas** en repositorios |
| **Maestro del Pull Request** | Registrar **50 o más Pull Requests** |
| **Cazador de Bugs e Issues** | Contar con **30 o más Issues** reportados o abiertos |
| **Motor Incombustible** | Registrar **10 o más eventos push** recientes |
| **Políglota del Código** | Utilizar **5 o más lenguajes** distintos en repositorios propios |
| **Veterano del Estadio** | Tener **5 o más años** de trayectoria en GitHub |
| **Fábrica de Proyectos** | Contar con **25 o más repositorios públicos** |

---

## 🛠️ Tecnologías Utilizadas

- **HTML5**: Estructura semántica en un único archivo ([index.html](index.html)).
- **Tailwind CSS (CDN) & CSS3**: Diseño *responsive*, cartas 3D holográficas y animaciones keyframe del estadio.
- **JavaScript (Vanilla)**: Consumo asíncrono de la API REST de GitHub, cálculo de métricas, auditoría, coaching y motor SVG del partido 5v5 (`CartoonMatchEngine`).
- **Librerías CDN**: `html2canvas` (exportación a PNG), Font Awesome 6 (iconografía) y Google Fonts (`Oswald` e `Inter`).

---

## 🚀 Cómo Usarlo

1. Clona o descarga este repositorio.
2. Abre el archivo [index.html](index.html) directamente en cualquier navegador moderno (o sírvelo con una extensión como *Live Server*).
3. Ingresa cualquier usuario de GitHub en **Perfil Individual** o enfrenta a dos desarrolladores en **Modo Duelo 1v1 (VS)**.

