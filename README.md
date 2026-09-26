[index.html](https://github.com/user-attachments/files/32685060/index.html)
```html
<!DOCTYPE html>
<html lang="uk">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>PERUKARNIA — Софіївська Борщагівка</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, sans-serif;
    background: #f4f1ec;
    color: #171717;
}

a {
    color: inherit;
    text-decoration: none;
}

/* НАВІГАЦІЯ */

header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 1000;
    padding: 18px 5%;
}

.navbar {
    max-width: 1250px;
    margin: auto;
    padding: 15px 22px;

    display: flex;
    align-items: center;
    justify-content: space-between;

    background: rgba(244,241,236,.92);
    backdrop-filter: blur(15px);

    border: 1px solid #ddd8d0;
    border-radius: 50px;
}

.logo {
    font-family: Georgia, serif;
    font-size: 24px;
    font-weight: bold;
}

nav {
    display: flex;
    gap: 28px;
}

nav a {
    font-size: 14px;
    transition: .3s;
}

nav a:hover {
    opacity: .5;
}

.nav-button {
    background: #171717;
    color: white;
    padding: 12px 21px;
    border-radius: 30px;
}

/* ГОЛОВНИЙ ЕКРАН */

.hero {
    min-height: 100vh;
    padding: 150px 6% 80px;

    display: flex;
    align-items: center;

    color: white;

    background:
        radial-gradient(
            circle at 75% 40%,
            #57514a,
            #262421 35%,
            #0d0d0d 75%
        );
}

.hero-content {
    max-width: 1250px;
    width: 100%;
    margin: auto;
}

.label {
    text-transform: uppercase;
    letter-spacing: 4px;
    font-size: 11px;
    opacity: .6;
    margin-bottom: 20px;
}

.hero h1 {
    font-family: Georgia, serif;
    font-size: clamp(60px, 9vw, 120px);
    line-height: .9;
    font-weight: normal;
}

.hero p {
    max-width: 500px;
    margin-top: 30px;
    color: #d0ccc6;
    line-height: 1.7;
    font-size: 17px;
}

.buttons {
    display: flex;
    gap: 12px;
    margin-top: 35px;
}

.button {
    display: inline-block;
    padding: 15px 25px;
    border-radius: 40px;
    background: white;
    color: #171717;
    font-weight: bold;
}

.button-outline {
    display: inline-block;
    padding: 15px 25px;
    border-radius: 40px;
    border: 1px solid #777;
}

/* СЕКЦІЇ */

section {
    padding: 110px 6%;
}

.container {
    max-width: 1250px;
    margin: auto;
}

h2 {
    font-family: Georgia, serif;
    font-size: clamp(42px, 6vw, 70px);
    font-weight: normal;
}

/* ПРО НАС */

.about {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 70px;
    align-items: center;
}

.about-image {
    height: 500px;
    border-radius: 25px;

    background:
        linear-gradient(145deg, #d7d0c6, #777068);
}

.about-text p {
    margin-top: 25px;
    color: #66615b;
    line-height: 1.8;
    font-size: 17px;
}

.rating {
    margin-top: 35px;
    display: flex;
    align-items: center;
    gap: 15px;
}

.rating-number {
    font-size: 42px;
    font-weight: bold;
}

.stars {
    letter-spacing: 3px;
}

/* ПОСЛУГИ */

.services {
    margin-top: 50px;

    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 15px;
}

.service {
    padding: 30px;

    background: #e7e2da;
    border-radius: 20px;

    display: flex;
    justify-content: space-between;
    gap: 20px;

    transition: .25s;
}

.service:hover {
    transform: translateY(-4px);
}

.service-number {
    font-size: 12px;
    opacity: .45;
}

.service h3 {
    font-size: 21px;
    margin: 8px 0;
}

.service p {
    color: #77716a;
}

.price {
    font-weight: bold;
    white-space: nowrap;
}

/* ГАЛЕРЕЯ */

.gallery {
    margin-top: 50px;

    display: grid;
    grid-template-columns: 2fr 1fr;
    gap: 15px;
}

.gallery-card {
    min-height: 350px;
    border-radius: 20px;

    background:
        linear-gradient(135deg, #b8b0a4, #514c46);

    display: flex;
    align-items: flex-end;
    padding: 30px;
    color: white;
}

.gallery-card:first-child {
    min-height: 500px;
}

.gallery-card h3 {
    font-family: Georgia, serif;
    font-size: 30px;
}

/* ВІДГУКИ */

.reviews {
    margin-top: 50px;

    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 15px;
}

.review {
    padding: 30px;
    background: #e7e2da;
    border-radius: 20px;
}

.review p {
    margin-top: 20px;
    color: #5f5b55;
    line-height: 1.7;
}

.review-name {
    margin-top: 25px;
    font-weight: bold;
}

/* КОНТАКТИ */

.contact {
    padding: 65px;

    background: #171717;
    color: white;

    border-radius: 30px;

    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 60px;
}

.contact h2 {
    margin-bottom: 30px;
}

.contact-info {
    display: flex;
    flex-direction: column;
    gap: 25px;
}

.contact-item span {
    display: block;
    text-transform: uppercase;
    letter-spacing: 2px;
    font-size: 10px;
    opacity: .5;
    margin-bottom: 7px;
}

/* FOOTER */

footer {
    padding: 35px;
    text-align: center;
    color: #77716a;
}

/* МОБІЛЬНА ВЕРСІЯ */

@media (max-width: 800px) {

    nav {
        display: none;
    }

    .hero {
        padding: 140px 7% 70px;
    }

    .hero h1 {
        font-size: 60px;
    }

    section {
        padding: 80px 7%;
    }

    .about,
    .services,
    .reviews,
    .gallery,
    .contact {
        grid-template-columns: 1fr;
    }

    .about-image {
        height: 350px;
    }

    .gallery-card:first-child {
        min-height: 350px;
    }

    .contact {
        padding: 40px 25px;
    }
}
</style>
</head>

<body>

<header>
    <div class="navbar">

        <div class="logo">
            PERUKARNIA
        </div>

        <nav>
            <a href="#about">Про нас</a>
            <a href="#services">Послуги</a>
            <a href="#gallery">Галерея</a>
            <a href="#reviews">Відгуки</a>
            <a href="#contacts">Контакти</a>
        </nav>

        <a class="nav-button" href="tel:0991114190">
            Записатися
        </a>

    </div>
</header>


<section class="hero">

    <div class="hero-content">

        <div class="label">
            Софіївська Борщагівка · Київ
        </div>

        <h1>
            Твій стиль.<br>
            Твоя історія.
        </h1>

        <p>
            Сучасна перукарня, де увага до деталей
            поєднується з комфортом та індивідуальним підходом.
        </p>

        <div class="buttons">

            <a class="button" href="tel:0991114190">
                Записатися
            </a>

            <a class="button-outline" href="#services">
                Послуги
            </a>

        </div>

    </div>

</section>


<section id="about">

    <div class="container">

        <div class="about">

            <div class="about-image"></div>

            <div class="about-text">

                <div class="label">
                    Про нас
                </div>

                <h2>
                    Краса<br>
                    в деталях
                </h2>

                <p>
                    Місце, де можна оновити свій образ,
                    отримати якісне обслуговування
                    та провести час у приємній атмосфері.
                </p>

                <div class="rating">

                    <div class="rating-number">
                        5,0
                    </div>

                    <div>
                        <div class="stars">★★★★★</div>
                        <small>7 відгуків</small>
                    </div>

                </div>

            </div>

        </div>

    </div>

</section>


<section id="services">

    <div class="container">

        <div class="label">
            Наші послуги
        </div>

        <h2>
            Послуги
        </h2>

        <div class="services">

            <div class="service">
                <div>
                    <div class="service-number">01</div>
                    <h3>Жіноча стрижка</h3>
                    <p>Стрижка та укладка</p>
                </div>
                <div class="price">300 ₴</div>
            </div>

            <div class="service">
                <div>
                    <div class="service-number">02</div>
                    <h3>Чоловіча стрижка</h3>
                    <p>Класична або сучасна</p>
                </div>
                <div class="price">250 ₴</div>
            </div>

            <div class="service">
                <div>
                    <div class="service-number">03</div>
                    <h3>Укладка</h3>
                    <p>Стильна укладка волосся</p>
                </div>
                <div class="price">250 ₴</div>
            </div>

            <div class="service">
                <div>
                    <div class="service-number">04</div>
                    <h3>Фарбування</h3>
                    <p>Індивідуальний підбір кольору</p>
                </div>
                <div class="price">700 ₴</div>
            </div>

        </div>

    </div>

</section>


<section id="gallery">

    <div class="container">

        <div class="label">
            Атмосфера
        </div>

        <h2>
            Галерея
        </h2>

        <div class="gallery">

            <div class="gallery-card">
                <h3>Стиль починається тут</h3>
            </div>

            <div class="gallery-card">
                <h3>Ваш образ</h3>
            </div>

        </div>

    </div>

</section>


<section id="reviews">

    <div class="container">

        <div class="label">
            Відгуки клієнтів
        </div>

        <h2>
            5,0 ★
        </h2>

        <div class="reviews">

            <div class="review">
                <div class="stars">★★★★★</div>
                <p>
                    Дуже приємна атмосфера
                    та гарне обслуговування.
                </p>
                <div class="review-name">Клієнт</div>
            </div>

            <div class="review">
                <div class="stars">★★★★★</div>
                <p>
                    Все акуратно, красиво
                    та професійно.
                </p>
                <div class="review-name">Клієнт</div>
            </div>

            <div class="review">
                <div class="stars">★★★★★</div>
                <p>
                    Залишилася дуже задоволена
                    результатом.
                </p>
                <div class="review-name">Клієнт</div>
            </div>

        </div>

    </div>

</section>


<section id="contacts">

    <div class="container">

        <div class="contact">

            <div>

                <div class="label">
                    Запис
                </div>

                <h2>
                    Будемо раді
                    бачити вас
                </h2>

                <a class="button" href="tel:0991114190">
                    099 111 4190
                </a>

            </div>

            <div class="contact-info">

                <div class="contact-item">
                    <span>Адреса</span>
                    вул. Андрія Малишка, 102,
                    Софіївська Борщагівка
                </div>

                <div class="contact-item">
                    <span>Графік</span>
                    Щодня · 10:00–20:00
                </div>

                <div class="contact-item">
                    <span>Телефон</span>
                    099 111 4190
                </div>

            </div>

        </div>

    </div>

</section>


<footer>
    © 2026 PERUKARNIA
</footer>

</body>
</html>
```
