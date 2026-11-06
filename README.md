<div align="center">
  <svg viewBox="0 0 1200 300" xmlns="http://www.w3.org/2000/svg" width="100%" height="auto">
    <defs>
      <!-- Градиент фона -->
      <linearGradient id="bgGradient" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" style="stop-color:#1E1E1E;stop-opacity:1" />
        <stop offset="100%" style="stop-color:#2D2D2D;stop-opacity:1" />
      </linearGradient>
      
      <!-- Свечение для акцентов -->
      <filter id="glow">
        <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
        <feMerge>
          <feMergeNode in="coloredBlur"/>
          <feMergeNode in="SourceGraphic"/>
        </feMerge>
      </filter>
    </defs>
    
    <!-- Фон -->
    <rect width="1200" height="300" fill="url(#bgGradient)" rx="10" />
    
    <!-- Сетка (как в редакторе кода) -->
    <g opacity="0.05">
      <pattern id="grid" width="20" height="20" patternUnits="userSpaceOnUse">
        <path d="M 20 0 L 0 0 0 20" fill="none" stroke="#FFFFFF" stroke-width="0.5"/>
      </pattern>
      <rect width="1200" height="300" fill="url(#grid)" />
    </g>
    
    <!-- Анимированные частицы -->
    <circle r="3" fill="#007ACC" opacity="0.6">
      <animate attributeName="cx" from="0" to="1200" dur="10s" repeatCount="indefinite" />
      <animate attributeName="cy" values="50;100;80;120;60" dur="8s" repeatCount="indefinite" />
    </circle>
    <circle r="2" fill="#007ACC" opacity="0.4">
      <animate attributeName="cx" from="1200" to="0" dur="12s" repeatCount="indefinite" />
      <animate attributeName="cy" values="200;150;180;140;220" dur="9s" repeatCount="indefinite" />
    </circle>
    <circle r="4" fill="#61DAFB" opacity="0.5">
      <animate attributeName="cx" from="0" to="1200" dur="15s" repeatCount="indefinite" />
      <animate attributeName="cy" values="250;200;230;190;260" dur="11s" repeatCount="indefinite" />
    </circle>
    
    <!-- Окно терминала -->
    <rect x="50" y="40" width="500" height="220" fill="#252526" rx="5" opacity="0.9" />
    <rect x="50" y="40" width="500" height="30" fill="#333333" rx="5" />
    
    <!-- Кнопки терминала -->
    <circle cx="65" cy="55" r="6" fill="#FF5F56" />
    <circle cx="85" cy="55" r="6" fill="#FFBD2E" />
    <circle cx="105" cy="55" r="6" fill="#27C93F" />
    
    <!-- Текст терминала -->
    <text x="70" y="60" font-family="monospace" font-size="10" fill="#8B949E">user@github:~</text>
    
    <!-- Команды в терминале с анимацией появления -->
    <g font-family="monospace" font-size="14">
      <text x="70" y="90" fill="#8B949E">
        <tspan>$ npm install experience</tspan>
      </text>
      
      <text x="70" y="115" fill="#007ACC" filter="url(#glow)">
        <tspan>✓ 4 years development</tspan>
        <animate attributeName="opacity" from="0" to="1" dur="0.3s" begin="1s" fill="freeze" />
      </text>
      
      <text x="70" y="140" fill="#8B949E">
        <tspan>$ npm install teaching</tspan>
        <animate attributeName="opacity" from="0" to="1" dur="0.3s" begin="1.5s" fill="freeze" />
      </text>
      
      <text x="70" y="165" fill="#007ACC" filter="url(#glow)">
        <tspan>✓ 2 years mentoring</tspan>
        <animate attributeName="opacity" from="0" to="1" dur="0.3s" begin="2.5s" fill="freeze" />
      </text>
      
      <text x="70" y="195" fill="#8B949E">
        <tspan>$ whoami</tspan>
        <animate attributeName="opacity" from="0" to="1" dur="0.3s" begin="3s" fill="freeze" />
      </text>
      
      <text x="70" y="220" fill="#FFFFFF" font-weight="bold" filter="url(#glow)">
        <tspan>&gt; Nnnekita</tspan>
        <animate attributeName="opacity" from="0" to="1" dur="0.3s" begin="3.5s" fill="freeze" />
      </text>
      
      <text x="70" y="240" fill="#61DAFB">
        <tspan>Fullstack Developer &amp; Teacher</tspan>
        <animate attributeName="opacity" from="0" to="1" dur="0.3s" begin="4s" fill="freeze" />
      </text>
    </g>
    
    <!-- Правая часть с кодом -->
    <rect x="580" y="40" width="570" height="220" fill="#1E1E1E" rx="5" opacity="0.9" />
    
    <!-- Подсветка синтаксиса (анимированная) -->
    <g font-family="monospace" font-size="13">
      <!-- Строка 1 -->
      <text x="600" y="70">
        <tspan fill="#C586C0">const</tspan>
        <tspan fill="#9CDCFE" x="640">developer</tspan>
        <tspan fill="#FFFFFF" x="730">=</tspan>
        <tspan fill="#B5CEA8" x="750">{</tspan>
      </text>
      
      <!-- Строка 2 -->
      <text x="620" y="95">
        <tspan fill="#9CDCFE">name</tspan>
        <tspan fill="#FFFFFF">:</tspan>
        <tspan fill="#CE9178" x="680">'Nnnekita'</tspan>
        <tspan fill="#FFFFFF" x="780">,</tspan>
      </text>
      
      <!-- Строка 3 -->
      <text x="620" y="120">
        <tspan fill="#9CDCFE">role</tspan>
        <tspan fill="#FFFFFF">:</tspan>
        <tspan fill="#CE9178" x="680">'Fullstack Dev'</tspan>
        <tspan fill="#FFFFFF" x="820">,</tspan>
      </text>
      
      <!-- Строка 4 -->
      <text x="620" y="145">
        <tspan fill="#9CDCFE">skills</tspan>
        <tspan fill="#FFFFFF">:</tspan>
        <tspan fill="#B5CEA8" x="690">[</tspan>
      </text>
      
      <!-- Строка 5 -->
      <text x="640" y="170">
        <tspan fill="#CE9178">'React'</tspan>
        <tspan fill="#FFFFFF" x="710">,</tspan>
        <tspan fill="#CE9178" x="730">'Laravel'</tspan>
        <tspan fill="#FFFFFF" x="810">,</tspan>
        <tspan fill="#CE9178" x="830">'Node.js'</tspan>
      </text>
      
      <!-- Строка 6 -->
      <text x="620" y="195">
        <tspan fill="#B5CEA8">]</tspan>
        <tspan fill="#FFFFFF" x="640">,</tspan>
      </text>
      
      <!-- Строка 7 -->
      <text x="620" y="220">
        <tspan fill="#9CDCFE">available</tspan>
        <tspan fill="#FFFFFF">:</tspan>
        <tspan fill="#569CD6" x="720">true</tspan>
      </text>
      
      <!-- Строка 8 -->
      <text x="600" y="245">
        <tspan fill="#B5CEA8">}</tspan>
        <tspan fill="#FFFFFF" x="620">;</tspan>
      </text>
      
      <!-- Мигающий курсор -->
      <rect x="635" y="250" width="8" height="15" fill="#FFFFFF">
        <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite" />
      </rect>
    </g>
    
    <!-- Декоративные элементы по углам -->
    <g stroke="#007ACC" stroke-width="2" fill="none" opacity="0.3">
      <path d="M 10 10 L 40 10 L 40 15 M 10 10 L 10 40">
        <animate attributeName="opacity" values="0.3;0.6;0.3" dur="3s" repeatCount="indefinite" />
      </path>
      <path d="M 1190 10 L 1160 10 L 1160 15 M 1190 10 L 1190 40">
        <animate attributeName="opacity" values="0.3;0.6;0.3" dur="3s" begin="0.5s" repeatCount="indefinite" />
      </path>
      <path d="M 10 290 L 40 290 L 40 285 M 10 290 L 10 260">
        <animate attributeName="opacity" values="0.3;0.6;0.3" dur="3s" begin="1s" repeatCount="indefinite" />
      </path>
      <path d="M 1190 290 L 1160 290 L 1160 285 M 1190 290 L 1190 260">
        <animate attributeName="opacity" values="0.3;0.6;0.3" dur="3s" begin="1.5s" repeatCount="indefinite" />
      </path>
    </g>
  </svg>
</div>

<div align="center">
  <h3>Fullstack-разработчик & Преподаватель</h3>
  <p>Превращаю идеи в работающие веб-приложения и помогаю студентам делать первые шаги в IT через реальные проекты.</p>
  
  [![Website](https://img.shields.io/badge/🌐_Личный_сайт-007ACC?style=for-the-badge&logo=google-chrome&logoColor=white)](https://nnnekita.github.io/My_Lending/)
</div>

---

## 📐 Обо мне

- 💻 **Опыт:** 4 года в коммерческой и pet-разработке, 2 года преподавания и менторства.
- 🚀 **Специализация:** Создание адаптивных лендингов, многостраничных сайтов и полноценных веб-приложений.
- 🎯 **Подход:** Чистая архитектура, переиспользуемые компоненты и структурированный код, который легко поддерживать.

---

## 🛠 Стек технологий

**Frontend:**
![HTML5](https://img.shields.io/badge/HTML5-1E1E1E?style=flat-square&logo=html5&logoColor=E34F26)
![CSS3](https://img.shields.io/badge/CSS3-1E1E1E?style=flat-square&logo=css3&logoColor=1572B6)
![JavaScript](https://img.shields.io/badge/JavaScript-1E1E1E?style=flat-square&logo=javascript&logoColor=F7DF1E)
![React](https://img.shields.io/badge/React-1E1E1E?style=flat-square&logo=react&logoColor=61DAFB)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-1E1E1E?style=flat-square&logo=tailwindcss&logoColor=38B2AC)
![Vite](https://img.shields.io/badge/Vite-1E1E1E?style=flat-square&logo=vite&logoColor=646CFF)
![SCSS](https://img.shields.io/badge/SCSS-1E1E1E?style=flat-square&logo=sass&logoColor=CC6699)

**Backend & Базы данных:**
![PHP](https://img.shields.io/badge/PHP-1E1E1E?style=flat-square&logo=php&logoColor=777BB4)
![Laravel](https://img.shields.io/badge/Laravel-1E1E1E?style=flat-square&logo=laravel&logoColor=FF2D20)
![MySQL](https://img.shields.io/badge/MySQL-1E1E1E?style=flat-square&logo=mysql&logoColor=4479A1)

**Инструменты:**
![Git](https://img.shields.io/badge/Git-1E1E1E?style=flat-square&logo=git&logoColor=F05032)
![VS Code](https://img.shields.io/badge/VS_Code-1E1E1E?style=flat-square&logo=visualstudiocode&logoColor=007ACC)

---

## 📂 Избранные проекты

| Проект | Описание | Стек |
| :--- | :--- | :--- |
| 🌐 **[My Lending](https://github.com/Nnnekita/My_Lending)** | Персональный сайт-портфолио. Адаптивная верстка, современный UI и чистая структура. | HTML, CSS, JS |
| 💅 **[MNails Studio](https://github.com/Nnnekita/nails-studio-sample)** | Лендинг для бизнеса. Плавные анимации, мобильное меню, работа с формами. | SCSS, Vite, JS |
| 📝 **[Guestbook PHP](https://github.com/Nnnekita/guestbook_php)** | Классическое fullstack-приложение. CRUD-операции, работа с БД и сессиями. | PHP, MySQL |
| 🎮 **[Neon Mini Game](https://github.com/Nnnekita/neon-mini-web-game)** | Интерактивная мини-игра. Работа с DOM, состоянием и CSS-анимациями. | HTML, CSS, JS |

---

## 📊 Активность и статистика

<p align="center">
  
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Nnnekita&theme=react-dark&hide_border=true&bg_color=00000000&color=8B949E&line=007ACC&point=FFFFFF" width="100%" alt="Activity Graph" />
</p>

<p align="center">
  
  <img src="https://github-readme-stats.vercel.app/api?username=Nnnekita&show_icons=true&theme=transparent&hide_border=true&title_color=FFFFFF&icon_color=007ACC&text_color=8B949E&bg_color=00000000" width="45%" alt="GitHub Stats" />
  
  
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Nnnekita&layout=compact&theme=transparent&hide_border=true&title_color=FFFFFF&text_color=8B949E&bg_color=00000000" width="45%" alt="Top Languages" />
</p>

<p align="center">
  
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Nnnekita&theme=transparent&hide_border=true&stroke=FFFFFF&fire=007ACC&ring=007ACC&sideLabels=FFFFFF&dates=8B949E" width="45%" alt="Streak Stats" />
</p>

---

## 📬 Связаться со мной

- 🌐 **Сайт:** [nnnekita.github.io/My_Lending](https://nnnekita.github.io/My_Lending/)
- ✈️ **Telegram:** [@KeepYM](https://t.me/KeepYM)
- 📧 **Email:** [kosmit.play@mail.ru](mailto:kosmit.play@mail.ru)
- 💬 **VK:** [vk.com/nnnekita](https://vk.com/nnnekita)

---

<div align="center">
  <p><em>Открыт для обсуждения fullstack-проектов, фриланса и менторства.</em></p>
</div>
