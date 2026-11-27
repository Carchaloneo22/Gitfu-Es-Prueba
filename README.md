<div align="center">

<img src="public/mascot.webp" width="120" alt="Mascota de GitFut">

# GitFut

**Tu perfil de GitHub, valorado sobre 99** ⚽

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=2600&pause=800&color=39D353&center=true&vCenter=true&width=680&height=42&lines=Convierte+cualquier+perfil+de+GitHub+en+una+carta+estilo+FIFA;Evaluado+en+vivo+con+commits%2C+estrellas+y+PRs+reales;Ins%C3%A9rtala+donde+quieras+%E2%80%94+se+actualiza+sola" alt="Convierte cualquier perfil de GitHub en una carta de jugador evaluada en vivo">

<br/><br/>

<a href="https://gitfut.com/torvalds"><img src="https://gitfut.com/torvalds.png" width="240" alt="Carta GitFut de torvalds"></a>
<a href="https://gitfut.com/ThePrimeagen"><img src="https://gitfut.com/ThePrimeagen.png" width="240" alt="Carta GitFut de ThePrimeagen"></a>
<a href="https://gitfut.com/t3dotgg"><img src="https://gitfut.com/t3dotgg.png" width="240" alt="Carta GitFut de t3dotgg"></a>

<br/><br/>

</div>

---

## 🃏 Inserta tu carta

Tu carta vive en una URL. Agrégala al `README` de tu perfil, a tu portafolio o donde quieras: **se vuelve a evaluar automáticamente** a medida que cambian tus estadísticas.

```md
[![Mi carta de GitFut](https://gitfut.com/TU_USUARIO.png)](https://gitfut.com/TU_USUARIO)
```

| Recurso | Descripción |
|---|---|
| **`gitfut.com/<usuario>.png`** | Tu carta en formato de imagen en vivo |
| **`gitfut.com/<usuario>`** | El informe completo de ojeo (*scouting*) |
| **`?country=XX`** | Sobrescribe la bandera manualmente (ej. `?country=ES`, `?country=MX`, `?country=AR`) |

---

## ⚙️ Cómo funciona el ojeo (*Scouting*)

Tomamos **seis señales reales** de tu perfil público en GitHub mediante la API GraphQL oficial y las transformamos en atributos futbolísticos. Sin encuestas ni autoevaluaciones: solo código y commits.

| Atributo | Significado | Métrica evaluada en GitHub |
|:--:|:--|:--|
| **RIT** *(PAC)* | Ritmo | Commits realizados en el último año |
| **TIR** *(SHO)* | Tiro | Estrellas acumuladas en tus repositorios |
| **PAS** *(PAS)* | Pase | Pull Requests y seguidores |
| **REG** *(DRI)* | Regate | Diversidad de lenguajes de programación |
| **DEF** *(DEF)* | Defensa | Revisiones de código (*reviews*) e *issues* |
| **FÍS** *(PHY)* | Físico | Contribuciones totales históricas |

Tu **Media General (OVR)** es la protagonista. Las estadísticas base tienen un tope de **88**: superar la barrera de los **90** requiere trayectoria e influencia sostenida, de modo que un solo año brillante no basta para coronarte como **Ícono**.  
Tu **posición** y **arquetipo** se calculan según la forma de tus estadísticas: un pico en *Tiro* define a un delantero goleador, mientras que un perfil fuerte en *Defensa* y *Pase* forma a un mediocentro organizador.

### Rarezas de Carta

<div align="center">

![Bronce](https://img.shields.io/badge/BRONCE-%E2%89%A464-CD7F32?style=flat-square&labelColor=2A1A0C)
![Plata](https://img.shields.io/badge/PLATA-65--74-AAB2BD?style=flat-square&labelColor=262B33)
![Oro](https://img.shields.io/badge/ORO-75--84-E6B422?style=flat-square&labelColor=3A2806)
![En Forma](https://img.shields.io/badge/EN%20FORMA-racha-E03E52?style=flat-square&labelColor=4A0A14)
![TOTY](https://img.shields.io/badge/TOTY-85--89-3B7AFF?style=flat-square&labelColor=10254F)
![Ícono](https://img.shields.io/badge/%C3%8DCONO-90%2B-F3D688?style=flat-square&labelColor=2A1A45)

</div>

---

## 🏆 Logros y Trofeos

Las cartas más destacadas desbloquean trofeos que se muestran en el informe de ojeo y acompañan al jugador en los duelos como cinturones de campeón (los duelos exhiben las vitrinas de cada perfil, pero nunca otorgan trofeos).  
Al hacer clic en cada trofeo puedes ver su historia: el año o edición del Mundial en que se ganó y el motivo exacto. Se renderizan mediante *sprites* precalculados (sin motor 3D en tiempo real; ver `scripts/bake-award-sprites.ts`).

| Trofeo | Cómo se obtiene |
| :---: | :--- |
| **Balón de Oro** | Un año calendario que sobresale por encima del resto de tu carrera, evaluado frente a tu propio historial con escala logarítmica (evita el *spam* de volumen). Repetible hasta 3 veces (4 para cartas **Ícono**). |
| **Balón de Oro del Mundial** | Mejor jugador durante una Copa del Mundo (2010 → 2026): superar tu propio ritmo habitual mientras el torneo estaba en juego, con reglas ajustadas por época. Uno por edición. |
| **Bota de Oro** | Máximo goleador según estado de forma actual: **Tiro (`TIR`) 80+** jugando en posición ofensiva (`DC` / `ED` / `MCO`). |
| **Trofeo Copa del Mundo** | ¡Campeones! España ganó el Mundial 2026: un obsequio especial incluido en todo perfil cuya ubicación en GitHub indique España. |

---

### 📜 El Reglamento

Cada evaluación consulta el historial completo del perfil año por año: commits, PRs, revisiones, *issues* y contribuciones privadas desde la creación de la cuenta. Los premios anuales se puntúan con esta fórmula:

```text
puntuacionAnual = 4·log(commits) + 3·log(PRs) + 3·log(reviews) + 2·log(issues) + 2·log(privadas)
```

Los logaritmos actúan como mecanismo **anti-spam**: cada métrica se satura progresivamente (por ejemplo, 20.000 commits suman `17.2`, apenas por encima de los `13.2` que dan 2.000). En cambio, un año equilibrado con 800 commits, 80 PRs, 80 revisiones y 40 *issues* alcanza `26`. La amplitud suma en todos los frentes, aunque un mantenedor de kernel enfocado solo en commits sigue compitiendo por volumen puro.

Salvo el obsequio conmemorativo de España, todos los trofeos exigen una **Media General (OVR) mínima de 80**. Es un umbral de entrada, no un multiplicador: mantiene fuera del podio a perfiles recién creados sin influir en nada más.

#### 🥇 Balón de Oro
Se evalúa frente a tu propia trayectoria, por lo que requiere al menos **2 años de historial**. Un año gana el premio si cumple las tres condiciones:

1. **2.000+ contribuciones brutas:** No hay Balón de Oro en un año discreto, por más que destaque frente al resto.
2. **Puntuación anual de 16+:** Rendimiento sólido en términos absolutos, no solo relativos.
3. **Cumplir una de estas dos vías:**
   - **El pico:** Superar en **1.2×** la mediana histórica de tu carrera (una temporada inolvidable).
   - **La élite:** Alcanzar **19.5+** puntos, sin importar la mediana (para carreras tan constantes que ningún año sobresale fácilmente).

Los títulos repetidos dependen de tu **OVR**: **80** desbloquea el 1.º, **87** el 2.º y **94** el 3.º. Los **Íconos** pueden ganar un 4.º solo con un año monstruoso (**28+** puntos). El año en curso compite mientras avanza, pero sin proyecciones: solo gana si ya superó los umbrales reales.

#### 🌍 Balón de Oro del Mundial
Uno por edición de la Copa del Mundo. Para candidatos con **OVR 80+** y actividad en un año mundialista, se evalúan las contribuciones dentro de la ventana exacta del torneo, ajustadas a su época:

| Edición | Ventana del torneo | Exigencia |
| :--- | :--- | :--- |
| **Sudáfrica 2010** | 11 jun – 11 jul | Presencia activa: aportar en GitHub en 2010 ya era mérito suficiente. |
| **Brasil 2014** | 12 jun – 13 jul | Un puñado sólido de contribuciones. |
| **Rusia 2018** | 14 jun – 15 jul | Actividad real a un ritmo de **1.2×** respecto a tu media anual. |
| **Catar 2022** | 20 nov – 18 dic | Ventana intensa (~10 contribuciones/día) a **1.3×** de tu ritmo habitual. |
| **Norteamérica 2026** | 11 jun – 19 jul | Ventana intensa (~10 contribuciones/día) a **1.3×** de tu ritmo habitual. |

La prueba de ritmo compara tu promedio diario durante el torneo frente a tu promedio diario en ese mismo año (en el año en curso se divide entre los días transcurridos, nunca entre 365).

#### 🥾 Bota de Oro
Es el único trofeo ligado al **estado de forma actual**, no vitalicio. Se reevalúa en cada análisis: requiere una posición ofensiva (`DC` / `ED` / `MCO`) y **Tiro 80+**. Si baja tu forma, pierdes la bota.

#### 🏆 Trofeo de la Copa del Mundo
España ganó el Mundial 2026 y cada perfil cuya ubicación en GitHub indique España levanta la copa: sin mínimo de OVR ni condiciones extra (cartas de bronce incluidas). Se basa en la ubicación reportada por GitHub, no en el parámetro visual `?country=ES`.

> Toda la vitrina se calcula en el servidor al momento del ojeo y se almacena en caché junto con la carta.

---

<div align="center">

**Construido con** Next.js · TypeScript · Tailwind CSS · Redis

**[gitfut.com](https://gitfut.com)** &nbsp;·&nbsp; evalúa un perfil hoy mismo

<img src="https://capsule-render.vercel.app/api?type=waving&height=90&color=0:39d353,100:006d32&section=footer" alt="" width="100%">

</div>
