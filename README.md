<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Дискорд 2.0 - Только для Русских | Discord Сервер</title>
    <meta name="description" content="Дискорд 2.0 - эксклюзивное русскоязычное сообщество. Присоединяйтесь к лучшему Discord серверу для русских!">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary: #5865F2;
            --primary-dark: #4752C4;
            --russian-red: #D52B1E;
            --russian-blue: #0033A0;
            --background: #1e1f29;
            --surface: #2b2d3b;
            --text: #ffffff;
            --text-secondary: #b9bbbe;
            --success: #57F287;
        }

        body {
            font-family: 'Arial', sans-serif;
            background: var(--background);
            color: var(--text);
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Навигация */
        .navbar {
            background: rgba(30, 31, 41, 0.95);
            backdrop-filter: blur(10px);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 70px;
        }

        .nav-logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--text);
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .russian-flag {
            display: inline-flex;
            height: 20px;
            width: 30px;
            border-radius: 3px;
            overflow: hidden;
        }

        .flag-stripe {
            flex: 1;
        }

        .flag-white { background: white; }
        .flag-blue { background: var(--russian-blue); }
        .flag-red { background: var(--russian-red); }

        .nav-menu {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-menu a {
            color: var(--text-secondary);
            text-decoration: none;
            font-weight: 600;
            transition: color 0.3s;
        }

        .nav-menu a:hover {
            color: var(--text);
        }

        .nav-cta {
            background: linear-gradient(135deg, var(--russian-blue), var(--russian-red));
            padding: 0.5rem 1rem;
            border-radius: 8px;
            color: white !important;
        }

        .nav-cta:hover {
            background: linear-gradient(135deg, #002288, #B22222);
        }

        /* Герой секция */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            padding: 100px 20px 50px;
            max-width: 1200px;
            margin: 0 auto;
            gap: 4rem;
            background: linear-gradient(135deg, rgba(0, 51, 160, 0.1), rgba(213, 43, 30, 0.1));
        }

        .hero-content {
            flex: 1;
        }

        .hero-title {
            font-size: 3.5rem;
            font-weight: 700;
            margin-bottom: 1rem;
            line-height: 1.2;
        }

        .highlight {
            background: linear-gradient(135deg, var(--russian-blue), var(--russian-red));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .hero-subtitle {
            font-size: 1.2rem;
            color: var(--text-secondary);
            margin-bottom: 2rem;
            max-width: 500px;
        }

        .russian-badge {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            background: rgba(0, 51, 160, 0.2);
            padding: 8px 16px;
            border-radius: 20px;
            border: 1px solid var(--russian-blue);
            margin-bottom: 1rem;
        }

        .hero-buttons {
            display: flex;
            gap: 1rem;
            margin-bottom: 3rem;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-block;
            padding: 1rem 2rem;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s;
            border: none;
            cursor: pointer;
            font-size: 1rem;
        }

        .btn-primary {
            background: linear-gradient(135deg, var(--russian-blue), var(--russian-red));
            color: white;
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(0, 51, 160, 0.3);
        }

        .btn-secondary {
            background: transparent;
            color: var(--text);
            border: 2px solid var(--surface);
        }

        .btn-secondary:hover {
            border-color: var(--russian-blue);
            transform: translateY(-2px);
        }

        .btn-large {
            padding: 1.2rem 2.5rem;
            font-size: 1.1rem;
        }

        .hero-stats {
            display: flex;
            gap: 2rem;
        }

        .stat {
            text-align: center;
        }

        .stat-number {
            font-size: 2rem;
            font-weight: 700;
            color: var(--russian-blue);
        }

        .stat-label {
            color: var(--text-secondary);
            font-size: 0.9rem;
        }

        .hero-image {
            flex: 1;
            display: flex;
            justify-content: center;
        }

        .discord-preview {
            background: var(--surface);
            border-radius: 15px;
            padding: 1.5rem;
            width: 300px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
            border: 1px solid var(--russian-blue);
        }

        .server-header {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin-bottom: 1.5rem;
            padding-bottom: 1rem;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }

        .server-icon {
            font-size: 2rem;
            background: linear-gradient(135deg, var(--russian-blue), var(--russian-red));
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .server-info h3 {
            margin-bottom: 0.2rem;
        }

        .server-info p {
            color: var(--text-secondary);
            font-size: 0.9rem;
        }

        .channel-category {
            color: var(--text-secondary);
            font-size: 0.8rem;
            margin: 1rem 0 0.5rem;
            text-transform: uppercase;
            font-weight: 600;
        }

        .channel {
            padding: 0.5rem 1rem;
            border-radius: 5px;
            margin: 0.2rem 0;
            cursor: pointer;
            transition: background 0.3s;
            color: var(--text-secondary);
        }

        .channel:hover {
            background: rgba(0, 51, 160, 0.2);
        }

        .channel.active {
            background: rgba(0, 51, 160, 0.3);
            color: var(--russian-blue);
        }

        /* Секции */
        section {
            padding: 80px 0;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            font-weight: 700;
        }

        /* Особенности */
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .feature-card {
            background: var(--surface);
            padding: 2rem;
            border-radius: 15px;
            text-align: center;
            transition: transform 0.3s;
            border: 1px solid transparent;
        }

        .feature-card:hover {
            transform: translateY(-5px);
            border-color: var(--russian-blue);
        }

        .feature-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .feature-card h3 {
            margin-bottom: 1rem;
            font-size: 1.3rem;
        }

        .feature-card p {
            color: var(--text-secondary);
        }

        /* Правила */
        .rules {
            background: var(--surface);
        }

        .rules-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
        }

        .rule-item {
            text-align: center;
            padding: 2rem;
            background: rgba(0, 51, 160, 0.1);
            border-radius: 15px;
            border: 1px solid var(--russian-blue);
        }

        .rule-item h3 {
            margin-bottom: 1rem;
            font-size: 1.2rem;
        }

        /* Статистика */
        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
            max-width: 800px;
            margin: 0 auto;
        }

        .stat-card {
            background: var(--surface);
            padding: 2rem;
            border-radius: 15px;
            display: flex;
            align-items: center;
            gap: 1rem;
            border: 1px solid var(--russian-blue);
        }

        .stat-icon {
            font-size: 2.5rem;
        }

        .stat-value {
            font-size: 2rem;
            font-weight: 700;
            color: var(--russian-blue);
        }

        .stat-label {
            color: var(--text-secondary);
        }

        /* Русская тематика */
        .russian-theme {
            background: linear-gradient(135deg, rgba(0, 51, 160, 0.05), rgba(213, 43, 30, 0.05));
            padding: 4rem 0;
            text-align: center;
        }

        .russian-message {
            max-width: 600px;
            margin: 0 auto;
            font-size: 1.1rem;
            line-height: 1.8;
        }

        /* Присоединиться */
        .join {
            text-align: center;
            background: linear-gradient(135deg, var(--russian-blue), var(--russian-red));
            position: relative;
            overflow: hidden;
        }

        .join::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><text y=".9em" font-size="90">🇷🇺</text></svg>') repeat;
            opacity: 0.1;
            pointer-events: none;
        }

        .join-content {
            position: relative;
            z-index: 2;
        }

        .join-content h2 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .join-content p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }

        .join-features {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin-top: 2rem;
            flex-wrap: wrap;
        }

        .feature {
            background: rgba(255, 255, 255, 0.2);
            padding: 0.5rem 1rem;
            border-radius: 20px;
            backdrop-filter: blur(10px);
        }

        /* Футер */
        .footer {
            background: var(--surface);
            padding: 2rem 0;
            text-align: center;
            color: var(--text-secondary);
            border-top: 1px solid var(--russian-blue);
        }

        /* Адаптивность */
        @media (max-width: 768px) {
            .hero {
                flex-direction: column;
                text-align: center;
                padding: 120px 20px 50px;
            }

            .hero-title {
                font-size: 2.5rem;
            }

            .hero-stats {
                justify-content: center;
            }

            .nav-menu {
                display: none;
            }

            .features-grid,
            .rules-grid {
                grid-template-columns: 1fr;
            }
        }

        /* Анимации */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .fade-in {
            animation: fadeInUp 0.6s ease-out;
        }

        /* Русские узоры */
        .russian-pattern {
            background-image: 
                radial-gradient(circle at 25% 25%, rgba(0, 51, 160, 0.1) 2px, transparent 2px),
                radial-gradient(circle at 75% 75%, rgba(213, 43, 30, 0.1) 2px, transparent 2px);
            background-size: 50px 50px;
        }
    </style>
</head>
<body class="russian-pattern">
    <!-- Навигация -->
    <nav class="navbar">
        <div class="nav-container">
            <div class="nav-logo">
                <div class="russian-flag">
                    <div class="flag-stripe flag-white"></div>
                    <div class="flag-stripe flag-blue"></div>
                    <div class="flag-stripe flag-red"></div>
                </div>
                Дискорд 2.0
            </div>
            <ul class="nav-menu">
                <li><a href="#home">Главная</a></li>
                <li><a href="#about">О сервере</a></li>
                <li><a href="#rules">Правила</a></li>
                <li><a href="#russian">Для Русских</a></li>
                <li><a href="#join" class="nav-cta">Вступить</a></li>
            </ul>
        </div>
    </nav>

    <!-- Герой секция -->
    <section id="home" class="hero">
        <div class="hero-content">
            <div class="russian-badge">
                <span>🇷🇺</span>
                <span>Только для русскоязычных</span>
            </div>
            <h1 class="hero-title">Добро пожаловать в <span class="highlight">Дискорд 2.0</span></h1>
            <p class="hero-subtitle">Эксклюзивное русскоязычное сообщество нового поколения. Общение, игры и развитие только на русском языке!</p>
            <div class="hero-buttons">
                <a href="https://discord.gg/ВАША_ССЫЛКА" class="btn btn-primary">🇷🇺 Вступить в сообщество</a>
                <a href="#about" class="btn btn-secondary">Узнать больше</a>
            </div>
            <div class="hero-stats">
                <div class="stat">
                    <div class="stat-number">2,000+</div>
                    <div class="stat-label">Русскоязычных</div>
                </div>
                <div class="stat">
                    <div class="stat-number">100+</div>
                    <div class="stat-label">Онлайн</div>
                </div>
                <div class="stat">
                    <div class="stat-number">24/7</div>
                    <div class="stat-label">На русском</div>
                </div>
            </div>
        </div>
        <div class="hero-image">
            <div class="discord-preview">
                <div class="server-header">
                    <div class="server-icon">🇷🇺</div>
                    <div class="server-info">
                        <h3>Дискорд 2.0</h3>
                        <p>Только для русских</p>
                    </div>
                </div>
                <div class="channels-list">
                    <div class="channel-category">🇷🇺 РУССКИЙ ЧАТ</div>
                    <div class="channel active">💬-общение</div>
                    <div class="channel">🎮-игры</div>
                    <div class="channel">📚-развитие</div>
                    
                    <div class="channel-category">🎪 РАЗВЛЕЧЕНИЯ</div>
                    <div class="channel">🎵-музыка</div>
                    <div class="channel">🎬-кино</div>
                    <div class="channel">📺-стримы</div>
                    
                    <div class="channel-category">🛡️ МОДЕРАЦИЯ</div>
                    <div class="channel">📜-правила</div>
                    <div class="channel">❓-помощь</div>
                </div>
            </div>
        </div>
    </section>

    <!-- О сервере -->
    <section id="about" class="about">
        <div class="container">
            <h2 class="section-title">Почему Дискорд 2.0?</h2>
            <div class="features-grid">
                <div class="feature-card">
                    <div class="feature-icon">🇷🇺</div>
                    <h3>Только Русские</h3>
                    <p>Эксклюзивное сообщество для русскоязычных пользователей</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">🚀</div>
                    <h3>Современный</h3>
                    <p>Дискорд нового поколения с улучшенным функционалом</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">🛡️</div>
                    <h3>Безопасность</h3>
                    <p>Строгая верификация и русская модерация 24/7</p>
                </div>
                <div class="feature-card">
                    <div class="feature-icon">🎯</div>
                    <h3>Активность</h3>
                    <p>Ежедневные ивенты и мероприятия на русском языке</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Русская тематика -->
    <section id="russian" class="russian-theme">
        <div class="container">
            <h2 class="section-title">🇷🇺 Только для Русских</h2>
            <div class="russian-message">
                <p>Мы создали уникальное пространство, где все общение происходит на русском языке. 
                Здесь вы найдете единомышленников, сможете обсуждать интересные темы и участвовать 
                в мероприятиях, созданных специально для русскоязычного сообщества.</p>
                
                <p><strong>Наш сервер - это дом для тех, кто ценит русскую культуру и язык!</strong></p>
            </div>
        </div>
    </section>

    <!-- Правила -->
    <section id="rules" class="rules">
        <div class="container">
            <h2 class="section-title">Основные правила</h2>
            <div class="rules-grid">
                <div class="rule-item">
                    <h3>🇷🇺 Русский язык</h3>
                    <p>Общение только на русском языке</p>
                </div>
                <div class="rule-item">
                    <h3>📝 Уважение</h3>
                    <p>Уважайте всех участников сообщества</p>
                </div>
                <div class="rule-item">
                    <h3>🚫 Без спама</h3>
                    <p>Запрещен флуд и массовые упоминания</p>
                </div>
                <div class="rule-item">
                    <h3>🔞 Контент 18+</h3>
                    <p>Запрещен NSFW контент</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Статистика -->
    <section id="stats" class="stats">
        <div class="container">
            <h2 class="section-title">Наша статистика</h2>
            <div class="stats-container">
                <div class="stat-card">
                    <div class="stat-icon">👥</div>
                    <div class="stat-content">
                        <div class="stat-value" id="memberCount">0</div>
                        <div class="stat-label">Русскоязычных</div>
                    </div>
                </div>
                <div class="stat-card">
                    <div class="stat-icon">💬</div>
                    <div class="stat-content">
                        <div class="stat-value" id="onlineCount">0</div>
                        <div class="stat-label">Онлайн сейчас</div>
                    </div>
                </div>
                <div class="stat-card">
                    <div class="stat-icon">🎮</div>
                    <div class="stat-content">
                        <div class="stat-value" id="gameCount">20+</div>
                        <div class="stat-label">Активных чатов</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Присоединиться -->
    <section id="join" class="join">
        <div class="container">
            <div class="join-content">
                <h2>Готовы присоединиться?</h2>
                <p>Станьте частью эксклюзивного русскоязычного сообщества Дискорд 2.0!</p>
                <a href="https://discord.gg/ВАША_ССЫЛКА" class="btn btn-large">🇷🇺 Вступить в Дискорд 2.0</a>
                <div class="join-features">
                    <div class="feature">✅ Только для русских</div>
                    <div class="feature">✅ Русская модерация</div>
                    <div class="feature">✅ Мероприятия на русском</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Футер -->
    <footer class="footer">
        <div class="container">
            <p>&copy; 2024 Дискорд 2.0 - Эксклюзивное русскоязычное сообщество.</p>
            <p>🇷🇺 Создано русскими для русских</p>
        </div>
    </footer>

    <script>
        // Анимации при скролле
        document.addEventListener('DOMContentLoaded', function() {
            // Плавная прокрутка
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    e.preventDefault();
                    const target = document.querySelector(this.getAttribute('href'));
                    if (target) {
                        target.scrollIntoView({
                            behavior: 'smooth',
                            block: 'start'
                        });
                    }
                });
            });

            // Анимация появления элементов
            const observerOptions = {
                threshold: 0.1,
                rootMargin: '0px 0px -50px 0px'
            };

            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('fade-in');
                    }
                });
            }, observerOptions);

            // Наблюдаем за всеми секциями
            document.querySelectorAll('section').forEach(section => {
                observer.observe(section);
            });

            // Динамическая статистика
            animateCounter('memberCount', 0, 2150, 2000);
            animateCounter('onlineCount', 0, 127, 1500);
        });

        // Анимация счетчиков
        function animateCounter(elementId, start, end, duration) {
            const element = document.getElementById(elementId);
            if (!element) return;

            let startTimestamp = null;
            const step = (timestamp) => {
                if (!startTimestamp) startTimestamp = timestamp;
                const progress = Math.min((timestamp - startTimestamp) / duration, 1);
                const value = Math.floor(progress * (end - start) + start);
                element.textContent = value.toLocaleString();
                
                if (progress < 1) {
                    window.requestAnimationFrame(step);
                }
            };
            window.requestAnimationFrame(step);
        }

        // Фиксированная навигация
        window.addEventListener('scroll', function() {
            const nav = document.querySelector('.navbar');
            if (window.scrollY > 100) {
                nav.style.background = 'rgba(30, 31, 41, 0.98)';
            } else {
                nav.style.background = 'rgba(30, 31, 41, 0.95)';
            }
        });

        // Интерактивное превью Discord
        document.querySelectorAll('.channel').forEach(channel => {
            channel.addEventListener('click', function() {
                document.querySelectorAll('.channel').forEach(c => c.classList.remove('active'));
                this.classList.add('active');
            });
        });

        // Русская тематика - случайные смайлики флага
        setInterval(() => {
            const emojis = ['🇷🇺', '🚀', '🎮', '💬', '🎯'];
            const randomEmoji = emojis[Math.floor(Math.random() * emojis.length)];
            const flagElement = document.querySelector('.server-icon');
            if (flagElement) {
                flagElement.textContent = randomEmoji;
            }
        }, 3000);
    </script>
</body>
</html>
