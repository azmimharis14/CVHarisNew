<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio - Muhammad Haris Azmi</title>
    <style>
        /* Reset Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f9f9f9;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }

        /* Header */
        .header {
            background-color: white;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 0;
        }

        .logo {
            font-size: 1.5rem;
            color: #0071e3;
            font-weight: bold;
        }

        .navbar ul {
            list-style: none;
            display: flex;
            gap: 20px;
        }

        .navbar ul li a {
            text-decoration: none;
            color: #333;
            font-size: 1rem;
            transition: color 0.3s ease;
        }

        .navbar ul li a:hover {
            color: #0071e3;
        }

        /* Section Styles */
        .section {
            display: none;
            text-align: center;
            padding: 50px 20px;
            flex: 1;
        }

        .section.active {
            display: block;
        }

        .section h1 {
            font-size: 2.5rem;
            color: #0071e3;
            margin-bottom: 20px;
        }

        .section p {
            font-size: 1rem;
            color: #555;
            margin-bottom: 10px;
        }

        .biodata {
            text-align: left;
            margin: 0 auto;
            max-width: 600px;
            background-color: #f5f5f7;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        .biodata p {
            margin: 10px 0;
        }

        /* Footer */
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px 0;
            margin-top: auto;
        }

        footer p {
            margin: 0;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="container">
            <div class="logo">azmimharis</div>
            <nav class="navbar">
                <ul>
                    <li><a href="javascript:void(0);" onclick="showSection('about')">Tentang</a></li>
                    <li><a href="javascript:void(0);" onclick="showSection('portfolio')">Portfolio</a></li>
                    <li><a href="javascript:void(0);" onclick="showSection('contact')">Kontak</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Welcome Section -->
    <section id="welcome" class="section active">
        <div class="container">
            <h1>Selamat Datang</h1>
            <p>Selamat datang di portfolio saya. Silakan pilih menu navigasi di atas untuk melihat lebih lanjut.</p>
        </div>
    </section>

    <!-- Tentang Section -->
    <section id="about" class="section">
        <div class="container">
            <h1>Tentang Saya</h1>
            <div class="biodata">
                <p><strong>Nama:</strong> Muhammad Haris Azmi</p>
                <p><strong>Tempat, Tanggal Lahir:</strong> Rantau Prapat, 14 Maret 2005</p>
                <p><strong>Biodata:</strong></p>
                <p>Saya adalah mahasiswa yang bersemangat dan berdedikasi dalam mengejar pendidikan di bidang S1 Informatika.</p>
                <p>Saya memiliki hasrat untuk mempelajari teknologi lebih mendalam dan bercita-cita menjadi Analis Sistem dan Konsultan TI.</p>
            </div>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section id="portfolio" class="section">
        <div class="container">
            <h1>Portfolio</h1>
            <p><strong>Skill:</strong></p>
            <p>- Video Editing</p>
            <p>- Photo Editing</p>
            <p>- Creative Thinking</p>
            <p>- Communication</p>
            <p>- Problem Solving</p>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="section">
        <div class="container">
            <h1>Kontak</h1>
            <p><strong>Email:</strong> mharisazmi6@gmail.com</p>
            <p><strong>Telepon:</strong> (+62) 813-6196-6686</p>
            <p><strong>Instagram:</strong> <a href="https://instagram.com/azmim.haris" target="_blank">@azmim.haris</a></p>
            <p><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/muhammad-haris-azmi-a7b75a18b" target="_blank">LinkedIn Profile</a></p>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2025 Muhammad Haris Azmi. All Rights Reserved.</p>
        </div>
    </footer>

    <script>
        // Function to show specific section
        function showSection(sectionId) {
            const sections = document.querySelectorAll('.section');
            sections.forEach(section => {
                section.classList.remove('active');
            });
            document.getElementById(sectionId).classList.add('active');
        }
    </script>
</body>
</html>
