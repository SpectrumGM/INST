# YC W26 Demo Day — Best Startups

**Категория:** YC Batch / Startup Trends
**Источник:** Instagram (сохранённый пост)
**Дата добавления:** 2026-05-17

> Подборка заметных стартапов из Demo Day батча Y Combinator Winter 2026.

---

## Список стартапов

1. **ARC Prize Foundation** — Creates benchmarks and competitions to measure progress toward artificial general intelligence systems.
2. **Asimov** — Collects human movement videos to build datasets for training humanoid robots.
3. **Avoice** — Automates document review and administrative tasks for architecture firms using AI.
4. **Button Computer** — Wearable AI device that connects apps and executes tasks through voice commands.
5. **CodeWisp** — Allows users to create video games by describing ideas to AI systems.
6. **Crosslayer Labs** — Detects and monitors spoofed websites to protect companies from online threats.
7. **Doomersion** — Language learning app delivering short-form videos in target language through a scrolling feed.
8. **Lexius** — Adds AI intelligence to security cameras for real-time incident detection and alerts.
9. **Librar Labs** — AI-powered system for managing library inventory, cataloging, and operations in schools.
10. **Milliray** — Sensor-based radar system designed to detect and track small aerial drones.
11. **MouseCat** — Analyzes cloud data to detect fraud patterns and recommend response actions.
12. **Opalite Health** — AI medical translator enabling communication between healthcare providers and non-English-speaking patients.
13. **Sequence Markets** — Unified platform for trading across crypto, prediction, and other financial markets.
14. **ShoFo** — Indexes and organizes large-scale video datasets for AI training and search.
15. **Sonarly** — Monitors software systems, identifies issues, and suggests or applies automated fixes.
16. **Terranox AI** — Uses AI models to identify uranium deposits for nuclear energy development.

---

# 🔍 Аналитический разбор

### 1. ARC Prize Foundation

Бенчмарки и соревнования для измерения прогресса к AGI. Это «инфраструктура оценки» — на чём индустрия меряет, насколько модели реально умнеют.

- **Актуальность:** высокая — все спорят про AGI, а объективных метрик мало.
- **Стек:** Python для генерации задач и оценки. Веб-платформа соревнований — Next.js + PostgreSQL. Прогон сабмишенов — Docker, изолированные среды исполнения.
- **Скиллы:** дизайн бенчмарков, ML-evaluation, бэкенд для лидербордов.
- **Конкуренция:** низкая по числу игроков, но это скорее некоммерческая модель (foundation), не классический бизнес.

### 2. Asimov

Сбор видео человеческих движений → датасеты для обучения человекоподобных роботов. Данные — узкое место всей робототехники.

- **Актуальность:** очень высокая — гонка гуманоидов (Figure, Tesla) упирается именно в данные.
- **Стек:** Python + PyTorch. Захват движений — компьютерное зрение, pose estimation (MediaPipe, OpenPose). Хранение видео — S3-подобное облако. Разметка — собственный пайплайн.
- **Скиллы:** computer vision, pose estimation, работа с большими видеоданными, имитационное обучение.
- **Конкуренция:** умеренная, рынок молодой — данные продают всем, кто строит роботов.

### 3. Avoice

Автоматизация ревью документов и админ-задач для архитектурных бюро. Классический «вертикальный AI» под узкую индустрию.

- **Актуальность:** высокая — конкретная боль, понятный платящий клиент.
- **Стек:** Python. Парсинг чертежей и спецификаций — OCR (Tesseract, AWS Textract), для DWG/чертежей — CAD-парсеры. LLM API для анализа. Бэкенд FastAPI, фронт Next.js.
- **Скиллы:** обработка документов, OCR, понимание workflow архитекторов, RAG.
- **Конкуренция:** низкая в этой нише — выигрыш за счёт глубокого знания индустрии.

### 4. Button Computer

Носимое AI-устройство, управляет приложениями голосом. Hardware + AI.

- **Актуальность:** средняя — категория «AI-гаджетов» уже обожглась (Humane, Rabbit), скепсиса много.
- **Стек:** embedded — C/C++, прошивка. Голос — speech-to-text (Whisper). Связь с приложениями — мобильное приложение (Swift/Kotlin), API-интеграции. LLM для интента.
- **Скиллы:** embedded-разработка, аппаратный дизайн, голосовые интерфейсы, мобильная разработка.
- **Конкуренция:** высокая и рискованная — железо дорого, провалов в категории много.

### 5. CodeWisp

Создание видеоигр через описание идей словами для AI. «Vibe coding» применительно к геймдеву.

- **Актуальность:** высокая, хайповая — democratization геймдева.
- **Стек:** LLM API для генерации кода/ассетов. Игровой движок-таргет — обычно веб (JavaScript, Phaser, Three.js) для мгновенного запуска в браузере. Бэкенд Node.js/Python.
- **Скиллы:** интеграция LLM, геймдев на вебе, кодогенерация, промпт-инжиниринг.
- **Конкуренция:** растёт быстро (Rosebud AI и др.) — нужен сильный продукт и качество вывода.

### 6. Crosslayer Labs

Детекция и мониторинг поддельных (spoofed) сайтов для защиты компаний. Близко к твоей идее black-swan-detector.

- **Актуальность:** высокая — фишинг и брендовый спуфинг растут.
- **Стек:** Python. Скан и краулинг доменов — Scrapy, Playwright. Сравнение визуала — computer vision (perceptual hashing, CNN). Анализ доменов — DNS/WHOIS API, threat-intel фиды. Бэкенд FastAPI.
- **Скиллы:** кибербезопасность, web-краулинг, computer vision для сравнения страниц, домен-аналитика.
- **Конкуренция:** умеренная — сегмент brand protection устоявшийся, но место есть.

### 7. Doomersion

Изучение языка через короткие видео в ленте на изучаемом языке. TikTok-механика + EdTech.

- **Актуальность:** средняя-высокая — формат залипательный, удержание хорошее.
- **Стек:** мобильное приложение — React Native или Swift/Kotlin. Лента и рекомендации — рекомендательная модель (Python). Субтитры/перевод — speech-to-text + перевод. Бэкенд для контента и прогресса.
- **Скиллы:** мобильная разработка, рекомендательные системы, продуктовый UX, контент-пайплайн.
- **Конкуренция:** очень плотная (Duolingo и десятки других) — выживание за счёт формата и удержания.

### 8. Lexius

AI поверх камер видеонаблюдения — детекция инцидентов в реальном времени.

- **Актуальность:** высокая — рынок видеоаналитики большой и растущий.
- **Стек:** Python + PyTorch. Детекция — YOLO, action recognition. Real-time инференс на edge — NVIDIA Jetson, TensorRT. Потоки видео — RTSP, GStreamer. Бэкенд для алертов.
- **Скиллы:** computer vision, real-time видео, edge-вычисления, action recognition.
- **Конкуренция:** высокая (Verkada и др.) — нужна ниша или цена.

### 9. Librar Labs

AI-система управления библиотечным фондом, каталогизацией и операциями в школах. Вертикальный нишевый SaaS.

- **Актуальность:** средняя — узкий рынок, но мало конкуренции и понятный клиент (школы).
- **Стек:** стандартный веб-SaaS — Python/FastAPI или Node.js бэкенд, Next.js фронт, PostgreSQL. LLM для каталогизации и поиска. Сканирование — OCR/штрихкоды.
- **Скиллы:** фуллстек-веб, проектирование SaaS, базовая интеграция LLM.
- **Конкуренция:** низкая — нишевый сегмент, но и потолок рынка небольшой.

### 10. Milliray

Радарная сенсорная система для обнаружения и трекинга малых дронов. Hardware + сигнальная обработка.

- **Актуальность:** очень высокая — антидрон-тематика на пике (безопасность, военка).
- **Стек:** обработка сигналов — C/C++, MATLAB. Железо радара — mmWave-чипы (Texas Instruments). Классификация целей — ML (Python, PyTorch). Embedded — прошивка.
- **Скиллы:** DSP (обработка сигналов), RF-инженерия, embedded, ML для классификации.
- **Конкуренция:** умеренная, высокий технический барьер — не софтовый pet-проект.

### 11. MouseCat

Анализ облачных данных для детекции мошенничества и рекомендаций по реакции.

- **Актуальность:** высокая — фрод-детекшн вечно востребован.
- **Стек:** Python. ML для аномалий — scikit-learn, XGBoost (твой профильный инструмент), PyTorch для глубоких моделей. Облачные логи — интеграции с AWS CloudTrail, GCP. Обработка потоков — Kafka, Spark.
- **Скиллы:** anomaly detection, ML на табличных данных (XGBoost — прямо твоё), облачная безопасность, data engineering.
- **Конкуренция:** высокая (Datadog, Sift) — нужна ниша или точность.

### 12. Opalite Health

AI-медицинский переводчик между врачами и пациентами без английского.

- **Актуальность:** высокая — реальная боль в здравоохранении США, понятен платящий клиент (клиники).
- **Стек:** speech-to-text (Whisper) + машинный перевод, дообученный на медицинской лексике. LLM API. Мобильное/планшетное приложение. Бэкенд с соблюдением HIPAA.
- **Скиллы:** NLP/перевод, speech-to-text, медицинский комплаенс, мобильная разработка.
- **Конкуренция:** умеренная — спецификой (медицина + комплаенс) отстраиваешься от общих переводчиков.

### 13. Sequence Markets

Единая платформа для торговли крипто, prediction-рынками и другими активами. Прямо в твоей теме quant finance.

- **Актуальность:** высокая — prediction-рынки на хайпе, фрагментация площадок реальна.
- **Стек:** бэкенд с низкой задержкой — Rust или Go, либо Python для логики. Интеграции бирж — REST/WebSocket API. Фронт — React/Next.js. Кошельки/блокчейн — web3-библиотеки. БД — PostgreSQL + time-series.
- **Скиллы:** финансовые API, low-latency бэкенд, blockchain-интеграции, понимание рыночной микроструктуры (твой опыт IMC Prosperity тут в тему).
- **Конкуренция:** высокая и зарегулированная — финансы, лицензии, серьёзный барьер.

### 14. ShoFo

Индексация и организация больших видеодатасетов для обучения AI и поиска. «Инфраструктура данных» для видео-AI.

- **Актуальность:** высокая — видеомодели и робототехника требуют управляемых датасетов.
- **Стек:** Python. Эмбеддинги видео — CLIP-подобные модели, PyTorch. Векторный поиск — Qdrant, Milvus, FAISS. Хранение — S3. Обработка — ffmpeg, распределённые пайплайны (Ray).
- **Скиллы:** computer vision, векторный поиск, data engineering, работа с большими медиаданными.
- **Конкуренция:** умеренная — рынок инфраструктуры для AI-данных молодой.

### 15. Sonarly

Мониторинг ПО, поиск проблем и автоматическое применение фиксов. AIOps + автономный agent.

- **Актуальность:** высокая — observability + auto-remediation востребованы.
- **Стек:** Python/Go для бэкенда. Сбор метрик/логов — OpenTelemetry, Prometheus. Анализ инцидентов — LLM API + anomaly detection. Применение фиксов — агентная логика, интеграции с CI/CD, Kubernetes API.
- **Скиллы:** observability, DevOps/SRE, агентные пайплайны, anomaly detection.
- **Конкуренция:** высокая (Datadog, PagerDuty добавляют AI) — нужна реально работающая автономность.

### 16. Terranox AI

AI-модели для поиска месторождений урана под ядерную энергетику.

- **Актуальность:** высокая — ренессанс атомной энергетики, спрос на уран растёт.
- **Стек:** Python. Геопространственный ML — `rasterio`, `geopandas`, PyTorch для анализа спутниковых и геофизических данных. Обработка снимков — спутниковые данные (Sentinel, Landsat). Визуализация — QGIS, PostGIS.
- **Скиллы:** геопространственный ML, обработка спутниковых снимков, базовая геология/геофизика.
- **Конкуренция:** низкая по числу игроков — узкая экспертная ниша, высокий доменный барьер.

---
