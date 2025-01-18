# fatmonkeymusic2

![immagine_scimmia](https://github.com/user-attachments/assets/32805663-26a5-4f19-856b-5c6522a00202)

<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FATMONKEYMUSIC</title>
    <!-- Aggiungiamo AOS per le animazioni -->
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;800&display=swap');

        :root {
            --primary-color: #ff0000;
            --secondary-color: #1a1a1a;
            --accent-color: #ff3333;
        }

        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #0a0a0a;
            color: white;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary-color), var(--accent-color));
            color: white;
            text-align: center;
            padding: 4rem 2rem;
            position: relative;
            overflow: hidden;
        }

        header h1 {
            font-size: 3.5rem;
            margin: 0;
            text-transform: uppercase;
            letter-spacing: 2px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        header p {
            font-size: 1.2rem;
            margin-top: 1rem;
            opacity: 0.9;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 4rem 2rem;
        }

        .video-section {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
            background: rgba(255,255,255,0.05);
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 8px 32px rgba(0,0,0,0.1);
        }

        .cta-button {
            display: inline-block;
            background: linear-gradient(45deg, var(--primary-color), var(--accent-color));
            color: white;
            padding: 1rem 2.5rem;
            text-decoration: none;
            border-radius: 50px;
            margin-top: 1.5rem;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(255,0,0,0.2);
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(255,0,0,0.3);
        }

        .social-links {
            text-align: center;
            margin-top: 4rem;
            padding: 2rem;
            background: rgba(255,255,255,0.03);
            border-radius: 20px;
        }

        .profile-image {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            margin-bottom: 2rem;
            object-fit: cover;
            border: 4px solid var(--primary-color);
            box-shadow: 0 0 20px rgba(255,0,0,0.3);
            transition: transform 0.3s ease;
        }

        .profile-image:hover {
            transform: scale(1.05);
        }

        section {
            margin-bottom: 4rem;
            padding: 2rem;
            background: rgba(255,255,255,0.03);
            border-radius: 20px;
            transition: transform 0.3s ease;
        }

        section:hover {
            transform: translateY(-5px);
        }

        h2 {
            color: var(--primary-color);
            font-size: 2.2rem;
            margin-bottom: 1.5rem;
            position: relative;
            display: inline-block;
        }

        h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 50%;
            height: 3px;
            background: linear-gradient(to right, var(--primary-color), transparent);
        }

        footer {
            text-align: center;
            padding: 2rem;
            background-color: var(--secondary-color);
            color: white;
            margin-top: 4rem;
        }

        /* Animazione per gli elementi che entrano nella viewport */
        .fade-up {
            opacity: 0;
            transform: translateY(20px);
            transition: all 0.6s ease;
        }

        .fade-up.visible {
            opacity: 1;
            transform: translateY(0);
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 2.5rem;
            }
            
            .container {
                padding: 2rem 1rem;
            }
        }
    </style>
</head>
<body>
    <header data-aos="fade-down">
        <h1>FATMONKEYMUSIC</h1>
        <p>La musica più bella di sempre!</p>
    </header>

    <div class="container">
        <section data-aos="fade-up">
            <h2>Chi Siamo</h2>
            <p>Ciao! noi siamo fatmonkeymusic e creiamo contenuti sulla musica. Sul nostro canale troverai canzoni fatte o su persone o su fatti personali.</p>
        </section>

        <section class="video-section" data-aos="fade-up" data-aos-delay="100">
            <div>
                <h3>Ultimo Video</h3>
                <iframe width="100%" height="315" src="https://www.youtube.com/embed/2pYBpRK7UOk" frameborder="0" allowfullscreen></iframe>
            </div>
        </section>

        <section class="social-links" data-aos="fade-up" data-aos-delay="200">
            <h2>Seguici</h2>
            <img src="immagine_scimmia.jpg" 
                 alt="Fatmonkeymusic Profile - Monkey DJ" 
                 class="profile-image">
            <br>
            <a href="https://www.youtube.com/@Fatmonkeymusic" class="cta-button">Iscriviti al Canale</a>
        </section>
    </div>

    <footer data-aos="fade-up">
        <p>&copy; 2024 FATMONKEYMUSIC. Tutti i diritti riservati.</p>
    </footer>

    <!-- Script per le animazioni -->
    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        AOS.init({
            duration: 800,
            once: true
        });
    </script>
</body>
</html>


