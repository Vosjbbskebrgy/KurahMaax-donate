<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Страница доната</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap');

        body {
            font-family: 'Press Start 2P', sans-serif;
            background-color: #121212;
            color: #ffffff;
            margin: 10;
            padding: 10 20px;
            background-image: url('your-vine-background.png');
            background-size: cover;
            line-height: 1.6;
            font-size: 92%; /* Уменьшение размера шрифта на 8% */
        }

        .header {
            background-color: #1a1a1a;
            color: #00d200;
            text-align: center;
            padding: 20px;
            font-size: 22px;
            margin-bottom: 10px;
            position: relative;
        }

        .social-links {
            text-align: center;
            margin-bottom: 7px;
        }

        .social-links a {
            display: inline-block;
            margin: 0 10px;
            transition: transform 0.3s ease-in-out;
        }

        .social-links img {
            width: 32px;
            height: 32px;
        }

        .social-links a:hover {
            transform: scale(1.1);
        }

        .button-container {
            display: flex;
            justify-content: space-between;
            margin-bottom: 7px;
        }

        .btn {
            padding: 10px 30px;
            background-color: #00994c; /* Более тусклый зелёный цвет */
            color: #ffffff;
            border: 2px solid #006633;
            cursor: pointer;
            font-size: 14px;
            transition: background-color 0.3s;
            margin-bottom: 5px;
        }

        .btn:hover {
            background-color: #00cc66; /* При наведении чуть ярче */
        }

        .description-text {
            background-color: #1a1a1a;
            color: #cccccc;
            text-align: center;
            padding: 10px 20px;
            font-size: 11px;
            margin-top: 10px;
            line-height: 1.8;
        }

        .dinwkeidybse-text {
            background-color: #1a1a1a;
            color: #00d200;
            text-align: center;
            padding: 10px 20px;
            font-size: 11px;
            margin-top: -8px;
            line-height: 1.8;
        }
        
        .section-title {
            background-color: #1a1a1a;
            color: #ffcc00;
            padding: 15px;
            font-size: 12px; /* Уменьшен шрифт */
            margin: 20px 0;
            cursor: pointer;
            position: relative;
        }

        .section-title::after {
            content: "Открыть полностью";
            color: #EBB34B;
            font-size: 10px;
            position: absolute;
            bottom: 3px;
            right: 4px;
        }

        .photo-gallery {
            display: flex;
            overflow-x: auto;
            white-space: nowrap;
            padding: 10px;
            background-color: #1a1a1a;
            margin-bottom: 20px;
        }

        .photo-gallery img {
            height: 138px; /* Уменьшено на 8% */
            margin-right: 10px;
            image-rendering: pixelated;
        }

        .info-text, .info-text-alt {
            background-color: #1a1a1a;
            color: #00d200;
            padding: 15px;
            font-size: 12px; /* Уменьшен шрифт */
            margin: 20px 0;
        }

        .donation-info {
            background-color: #1a1a1a;
            color: #ffffff;
            padding: 15px;
            font-size: 12px; /* Уменьшен шрифт */
            margin: 20px 0;
            cursor: pointer;
            overflow: hidden;
            transition: max-height 0.5s ease-out, opacity 0.5s ease-out;
            max-height: 50px;
            opacity: 0.8;
            position: relative;
            padding-bottom: 238px; /* Добавлено 7 пикселей заднего фона */
        }

        .donation-info.expanded {
            max-height: none;
            opacity: 1;
            white-space: normal;
        }

        .donation-info::after {
            content: ";)  ";
            color: #006611;
            font-size: 10px;
            position: absolute;
            bottom: 3px; /* Опущено, чтобы не перекрывало текст */
            right: 9px;
        }

        .donation-info.highlighted {
            animation: highlight 1s ease-out 2; /* Анимация с двумя повторениями */
        }

        @keyframes highlight {
            0% {
                background-color: rgba(0, 255, 102, 0.2);
            }
            100% {
                background-color: transparent;
            }
        }

        .extra-text {
            display: none;
            background-color: #1a1a1a;
            padding: 15px;
            margin-top: 10px;
            opacity: 0;
            overflow: hidden;
            transition: max-height 0.5s ease-out, opacity 0.5s ease-out;
            font-size: 12px; /* Уменьшен шрифт */
        }

        .extra-text.visible {
            display: block;
            max-height: none;
            opacity: 1;
        }

        .confirmation-box {
            background-color: #1a1a1a;
            text-align: center;
            padding: 10px;
            margin-top: 10px;
        }

        .confirmation-btn {
            padding: 10px 30px;
            background-color: #00994c;
            color: #ffffff;
            border: 2px solid #006633;
            cursor: pointer;
            font-size: 14px;
            transition: background-color 0.3s;
        }

        .confirmation-btn:hover {
            background-color: #00cc66;
        }

    </style>
</head>
<body>

    <div class="header">Страница доната</div>

    <div class="social-links">
        <a href="https://t.me/+g5NZi8kQ2KRkMmIy"><img src="IMG_20240903_184149_156.jpg" alt="Telegram"></a>
        <a href="https://youtube.com/@kurahmaax?si=Io0Iy2MyisbfuzHa"><img src="trashed-1727970226-97440.jpg" alt="YouTube"></a>
        <a href="https://www.instagram.com/kurah_maax?igsh=cTkxMmxucW5rYW9n"><img src="98cf57621f6a.jpg" alt="Instagram"></a>
    </div>

    <div class="button-container">
        <button class="btn" onclick="window.location.href='https://donate.stream/kurahmaax';">Задонатить</button>
        <button class="btn" onclick="scrollToDonationInfo();">Важное</button>
    </div>

    <div class="description-text">
        Добро пожаловать на сайт!<br><br>
        Вы попали на уникальную страницу, где можете сделать пожертвование или поддержать наш проект и приобрести проходку в закрытый телеграмм канал.<br><br>
        В этом закрытом ТГК вас ждут эксклюзивные карты из видео КурахМакса, которые вы сможете использовать в своих собственных проектах.<br><br>
        Поддержите нас, и получите доступ к уникальному контенту за небольшую плату!
    </div>

    <div class="section-title" onclick="toggleExtraText()">Для чего может быть полезна покупка?</div>

    <div class="extra-text">
        Начнем с того что проект уникален и такого вы нигде не найдете)<br><br>
        Карту можно использовать в своих целях или извлечь из неё полезности на примере (команд)<br><br>
        Наш продукт может быть полезен для начинающих проектов, где понадобится имеющаяся в наличии постройка или карта<br><br>
        Карту можно использовать в целях улучшения своего контента<br><br>
        Вы можете играть на карте вместе с друзьями
    </div>

    <div class="info-text-alt">• Вот что вы получаете при покупке проходки</div>

    <div class="photo-gallery">
        <img src="IMG_20240829_171453.jpg" alt="Фото 7">
        <img src="IMG_20240829_171427.jpg" alt="Фото 6">
        <img src="IMG_20240829_171146.jpg" alt="Фото 5">
        <img src="IMG_20240829_171133.jpg" alt="Фото 4">
        <img src="IMG_20240829_171113.jpg" alt="Фото 3">
        <img src="IMG_20240829_171055.jpg" alt="Фото 2">
        <img src="Screenshot_2024-08-29-17-10-20-715_com.lemon.lvoverseas.png" alt="Фото 1">
    </div>

    <div id="donation-info" class="donation-info">
        За донат определённой сумы вам будут даваться определенные привилегии)<br><br>
        
        💜 КурахМаан 👾<br>
        [399 грн]<br>
        -------------------------<br>
        • Доступ к картам из видео<br><br>

        🍫 Шторка в закулисье 🎀<br>
        [??? грн]<br>
        -------------------------<br>
        • ??? (В будущем будет доступен мерч)
    </div>

    <div class="confirmation-box">
        <button class="confirmation-btn" onclick="window.location.href='https://donate.stream/kurahmaax';">Я ознакомлен со всей информацией!<br><<Перейти к донату>></button>
    </div>
    
    
    <div class="dinwkeidybse-text">
——————————————————————————<br>
        ‼️ Не забудьте указать свой ник<br>
телеграмма (в комментариях<br>
доната) при покупке проходки<br>
за 399 грн ️‼️
    </div>

    <script>
        // Функция для скролла к блоку с донатом и выполнения других действий
        function scrollToDonationInfo() {
            const donationInfo = document.getElementById("donation-info");

            // Скролл к блоку "donation-info"
            donationInfo.scrollIntoView({ behavior: 'smooth' });

            // Раскрытие текста "За донат определённой сумы вам будут даваться..."
            donationInfo.classList.add("expanded");

            // Подсветка текста с помощью наложения
            donationInfo.classList.add("highlighted");

            // Удаление подсветки после окончания анимации
            setTimeout(() => {
                donationInfo.classList.remove("highlighted");
            }, 2000); // 2 раза по 1 секунде на каждую анимацию
        }

        // Функция для переключения видимости текста "Для чего может быть полезна покупка?"
        function toggleExtraText() {
            const extraText = document.querySelector(".extra-text");
            extraText.classList.toggle("visible");
        }
    </script>
</body>
</html>
