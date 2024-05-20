19gym-site-web
Realizat de Pica Ovidiu Stefan

Documentație  pentru Website-ul 19Gym

Această documentație detaliază procesul de creare a website-ului 19Gym, utilizând HTML, CSS, JavaScript și jQuery. Include descrierea tehnologiilor folosite, pașii de dezvoltare și explicații detaliate pentru fiecare etapă.

---

introducere

Website-ul 19Gym a fost creat ca parte a unui concurs de pagini web, având ca scop prezentarea unei săli de fitness. Site-ul oferă informații despre sală, programul de lucru, modalități de contact și abonamente disponibile. Utilizatorii pot să se aboneze la newsletter și să contacteze sala printr-un formular dedicat.

---

Limbaje de Programare și Tehnologii Utilizate

1. HTML (HyperText Markup Language)
   - Limbaj de marcare folosit pentru a structura conținutul paginilor web.
   - A fost utilizat pentru a crea structura de bază a paginilor, incluzând titluri, paragrafe, imagini și link-uri.

2. CSS (Cascading Style Sheets)
   - Limbaj de stilizare folosit pentru a defini aspectul vizual al paginilor web.
   - A fost utilizat pentru a stiliza elementele HTML, adăugând culori, fonturi, margini și layout-uri responsive.

3. JavaScript (JS)
   - Limbaj de programare folosit pentru a adăuga interactivitate și dinamism paginilor web.
   - A fost utilizat pentru validarea formularelor și adăugarea de funcționalități dinamice.

4. jQuery
   - Librărie JavaScript care simplifică manipularea DOM, gestionarea evenimentelor și efectuarea apelurilor AJAX.
   - A fost utilizată pentru a simplifica codul JavaScript și pentru a crea animații.

---

Pași pentru Crearea Website-ului

1. Planificarea și Designul

- Definirea Scopului și Publicului Țintă
  - Scopul site-ului este de a prezenta informații despre sala de fitness 19Gym și de a atrage noi membri.
  - Publicul țintă include persoane interesate de fitness și sănătate, atât începători cât și sportivi experimentați.

- Crearea Wireframe-urilor și Prototipurilor
  - Au fost create wireframe-uri și prototipuri vizuale folosind instrumente precum Adobe XD sau Figma pentru a vizualiza structura și designul paginilor.

 2. Crearea Structurii HTML

- *Definirea Structurii de Bază*
  - A fost creată structura de bază a paginilor web folosind HTML5.
  - Elementele principale includ header, footer, secțiunea principală și formularele de contact și newsletter.
Aici este o mica parte a codului html
<!DOCTYPE html>
<html lang="ro">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>19Gym</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>19Gym</h1>
        <nav>
            <ul>
                <li><a href="#despre-noi">Despre Noi</a></li>
                <li><a href="#abonamente">Abonamente</a></li>
                <li><a href="#contact">Contactează-ne</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="despre-noi">
            <h2>Despre Noi</h2>
            <p>La 19Gym, suntem dedicați să te ajutăm să îți atingi obiectivele de fitness...</p>
        </section>

        <section id="abonamente">
            <h2>Abonamente</h2>
            <p>Oferim o varietate de opțiuni de abonament...</p>
        </section>

        <section id="contact">
            <h2>Contactează-ne</h2>
            <address>
                19Gym, București, România<br>
                Strada Sportului, nr. 19, Sector 1<br>
                +40 (21) 555 1234<br>
                <a href="mailto:support@19gym.ro">support@19gym.ro</a>
            </address>
        </section>
    </main>

    <footer>
        <p>Copyright ©2024 Toate drepturile rezervate | Acest șablon este realizat de Colorlib</p>
    </footer>
    
    <script src="script.js"></script>
</body>
</html>


 3. Stilizarea cu CSS

- *Adăugarea de Stiluri CSS*
  - Au fost adăugate stiluri CSS pentru a defini aspectul vizual al elementelor HTML.
  - Media queries au fost utilizate pentru a crea un design responsive.
Aici este o mica parte a codului css

css
/* styles.css */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

header {
    background-color: #333;
    color: white;
    padding: 1rem;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 1rem;
}

main {
    padding: 2rem;
}

section {
    margin-bottom: 2rem;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 1rem;
    position: fixed;
    bottom: 0;
    width: 100%;
}

@media (max-width: 600px) {
    nav ul li {
        display: block;
        margin: 0.5rem 0;
    }
}


 4. Adăugarea Interactivității cu JavaScript și jQuery

- *Validarea Formularului de Newsletter*
  - JavaScript a fost utilizat pentru a valida formularul de newsletter, asigurându-se că utilizatorii introduc un e-mail valid.

javascript
Aici este o mica parte a codului javascript

// script.js
$(document).ready(function() {
    $('#newsletterForm').on('submit', function(e) {
        e.preventDefault();
        let email = $('#email').val();
        if (validateEmail(email)) {
            alert('Mulțumim pentru abonare!');
        } else {
            alert('Vă rugăm să introduceți un email valid.');
        }
    });

    function validateEmail(email) {
        var re = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
        return re.test(email);
    }
});


 5. Testare și Debugging

- *Testare pe Diverse Browsere și Dispozitive*
  - Website-ul a fost testat pe multiple browsere (Chrome, Firefox, Safari) și dispozitive (desktop, tabletă, mobil) pentru a asigura compatibilitatea și funcționalitatea corectă.
  
- *Rezolvarea Erorilor și Optimizarea Performanței*
  - Erorile identificate au fost corectate, iar codul a fost optimizat pentru performanță și viteză de încărcare.

6. Publicare

- *Încărcarea pe Server și Publicarea Online*
  - După finalizarea testelor și optimizărilor, site-ul a fost încărcat pe un server de hosting și publicat online.

---

 Concluzie

Aceasta a fost documentația procesului de creare a website-ului 19Gym. Folosind HTML, CSS, JavaScript și jQuery, am reușit să dezvolt un site atractiv, funcțional și ușor de utilizat. Sper că această prezentare v-a oferit o imagine clară asupra modului în care am realizat acest proiect. Dacă aveți întrebări sau doriți să aflați mai multe detalii, sunt aici pentru a răspunde. Vă mulțumesc pentru atenție.
