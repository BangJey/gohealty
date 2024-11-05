<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <title>Selamat Datang di Go Health</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        .container {
            display: flex;
        }
        .navbar {
            width: 200px;
            background: #007BFF;
            padding: 15px;
            color: white;
            position: fixed;
            height: 100%;
            overflow-y: auto;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .navbar a {
            color: white;
            text-decoration: none;
            padding: 10px 0;
            display: flex;
            align-items: center;
            width: 100%;
        }
        .navbar a i {
            margin-right: 10px;
        }
        .content {
            margin-left: 220px; /* Space for navbar */
            padding: 20px;
            flex: 1;
        }
        h1, h2, h3 {
            text-align: center;
        }
        section {
            display: none; /* Initially hide sections */
            margin-bottom: 20px;
            padding: 10px;
            background: white;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        .back-button {
            display: inline-block;
            margin: 10px 0;
            padding: 5px 10px;
            background-color: #007BFF;
            color: white;
            text-decoration: none;
            border-radius: 5px;
        }
        .table-container {
            overflow-x: auto;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 10px;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
        th {
            background-color: #007BFF;
            color: white;
        }
        .team-icon {
            width: 20px;
            margin-right: 5px;
        }
        .video-container {
            display: flex;
            justify-content: center;
            margin: 20px 0;
        }
        iframe {
            width: 100%;
            max-width: 560px;
            height: 315px;
            border: none;
        }
    </style>
</head>
<body>

<div class="navbar">
    <h2>Yuk Belajar Sehat Bersama Kami</h2>
    <a href="#" onclick="showSection('nutrisi-diet')"><i class="fas fa-apple-alt"></i>Nutrisi & Diet</a>
    <a href="#" onclick="showSection('olahraga-aktivitas')"><i class="fas fa-dumbbell"></i>Olahraga & Aktivitas Fisik</a>
    <a href="#" onclick="showSection('kesehatan-mental')"><i class="fas fa-brain"></i>Kesehatan Mental</a>
    <a href="#" onclick="showSection('pola-tidur')"><i class="fas fa-bed"></i>Pola Tidur</a>
    <a href="#" onclick="showSection('tips-pencegahan')"><i class="fas fa-shield-alt"></i>Tips Pencegahan Penyakit</a>
    <a href="#" onclick="showSection('resep-makanan')"><i class="fas fa-utensils"></i>Resep Makanan Sehat</a>
    <a href="#" onclick="showSection('kalkulator-bmi')"><i class="fas fa-weight"></i>Kalkulator BMI</a>
    <a href="#" onclick="showSection('my-team')"><i class="fas fa-users"></i>My Team</a>
</div>

<div class="content">
    <h1>Selamat Datang di Go Health</h1>
    <h3>Temukan cara hidup sehat dan bahagia bersama kami!</h3>

    <section id="nutrisi-diet">
        <h3>Nutrisi & Diet</h3>
        <a class="back-button" href="#" onclick="hideAllSections()">Kembali</a>
        <ul>
            <li>
                <strong>Apa itu Pola Makan Seimbang?</strong>
                <p>Pola makan seimbang adalah pendekatan nutrisi yang melibatkan konsumsi berbagai jenis makanan dalam proporsi yang tepat untuk memenuhi kebutuhan nutrisi tubuh. Ini berarti menggabungkan makanan dari semua kelompok makanan, termasuk karbohidrat, protein, lemak sehat, vitamin, mineral, dan air, sehingga tubuh mendapatkan semua nutrisi yang dibutuhkan untuk berfungsi dengan baik. Pola makan seimbang membantu menjaga berat badan yang sehat, mendukung pertumbuhan dan perkembangan, serta mengurangi risiko penyakit kronis.</p>
            </li>
            <li>
                <strong>Panduan Piring Makan Seimbang:</strong>
                <p>Panduan piring makan seimbang adalah metode visual yang memudahkan pemahaman tentang proporsi makanan yang seharusnya dimakan. Bayangkan piring Anda dibagi menjadi tiga bagian: </p>
                <ul>
                    <li><strong>Setengah piring:</strong> Diisi dengan sayuran dan buah-buahan. Pilihlah beragam warna untuk mendapatkan berbagai vitamin dan mineral.</li>
                    <li><strong>Satu perempat piring:</strong> Diisi dengan sumber karbohidrat, seperti nasi, pasta, roti, atau kentang. Utamakan karbohidrat kompleks yang kaya serat.</li>
                    <li><strong>Satu perempat piring:</strong> Diisi dengan protein, seperti daging tanpa lemak, ikan, telur, kacang-kacangan, atau produk susu. Pilih sumber protein yang sehat dan rendah lemak.</li>
                </ul>
                <p>Dengan menggunakan panduan ini, Anda dapat merencanakan porsi makanan yang lebih seimbang dan lebih sehat setiap kali makan.</p>
            </li>
            <li>
                <strong>Tips Menerapkan Pola Makan Seimbang:</strong>
                <p>Berikut adalah beberapa tips praktis untuk menerapkan pola makan seimbang dalam kehidupan sehari-hari:</p>
                <ul>
                    <li><strong>Rencanakan makanan Anda:</strong> Buatlah rencana menu mingguan yang mencakup berbagai jenis makanan dari semua kelompok. Ini membantu Anda untuk tetap pada jalur dan menghindari pilihan yang tidak sehat.</li>
                    <li><strong>Belanja dengan bijak:</strong> Saat berbelanja, prioritaskan bahan makanan segar dan utuh. Bacalah label gizi untuk memastikan Anda membeli produk yang sehat.</li>
                    <li><strong>Masak di rumah:</strong> Memasak makanan sendiri memberi Anda kontrol lebih besar atas bahan-bahan dan cara pengolahannya. Cobalah resep sehat yang memanfaatkan bahan-bahan alami.</li>
                    <li><strong>Perhatikan porsi makan:</strong> Makanlah dalam porsi yang wajar dan perhatikan rasa kenyang Anda. Menggunakan piring yang lebih kecil bisa membantu mengontrol porsi.</li>
                    <li><strong>Hindari makanan olahan:</strong> Batasi konsumsi makanan yang mengandung banyak gula, garam, dan lemak jenuh. Pilih makanan segar atau yang diproses minimal.</li>
                    <li><strong>Minum cukup air:</strong> Air penting untuk menjaga hidrasi. Usahakan untuk minum setidaknya 8 gelas air sehari, dan lebih banyak jika Anda aktif berolahraga.</li>
                </ul>
            </li>
            <li>
                <strong>Informasi Kandungan Gizi Makanan:</strong>
                <p>Mengetahui kandungan gizi pada berbagai makanan sangat penting untuk membuat pilihan diet yang lebih baik. Anda dapat menggunakan tabel gizi atau aplikasi ponsel untuk memeriksa informasi ini. Fokus pada:</p>
                <ul>
                    <li><strong>Makronutrien:</strong> Karbohidrat, protein, dan lemak. Pastikan Anda mendapatkan proporsi yang tepat dari masing-masing.</li>
                    <li><strong>Mikronutrien:</strong> Vitamin dan mineral yang dibutuhkan dalam jumlah kecil tetapi sangat penting bagi kesehatan. Contohnya termasuk vitamin A, C, D, kalsium, dan zat besi.</li>
                </ul>
            </li>
            <li>
                <strong>Tips Memilih Makanan Sehat:</strong>
                <p>Cara memilih makanan yang baik untuk kesehatan meliputi pemilihan bahan makanan segar dan utuh. Berikut adalah beberapa tips untuk memilih makanan sehat:</p>
                <ul>
                    <li>Pilih makanan segar dan alami, seperti buah-buahan dan sayuran musiman.</li>
                    <li>Baca label gizi untuk memilih produk yang rendah gula tambahan, sodium, dan lemak jenuh.</li>
                    <li>Hindari makanan yang mengandung bahan pengawet dan aditif buatan.</li>
                    <li>Pilih sumber protein yang sehat, seperti ikan, kacang-kacangan, dan produk susu rendah lemak.</li>
                </ul>
            </li>
            <li>
                <strong>Mitos vs Fakta tentang Diet:</strong>
                <p>Banyak mitos beredar tentang diet dan nutrisi. Berikut beberapa mitos umum yang perlu diperhatikan:</p>
                <ul>
                    <li><strong>Mitos:</strong> Semua lemak buruk. <strong>Fakta:</strong> Lemak sehat seperti yang ditemukan dalam alpukat dan ikan sangat penting bagi kesehatan.</li>
                    <li><strong>Mitos:</strong> Diet ketat adalah cara terbaik untuk menurunkan berat badan. <strong>Fakta:</strong> Mengubah kebiasaan makan secara bertahap dan berkelanjutan lebih efektif dan sehat.</li>
                </ul>
            </li>
            <li>
                <strong>Makanan Superfood dan Manfaatnya:</strong>
                <p>Makanan superfood adalah makanan yang kaya akan nutrisi dan memiliki banyak manfaat kesehatan. Berikut adalah beberapa contoh:</p>
                <ul>
                    <li><strong>Blueberry:</strong> Kaya akan antioksidan yang dapat meningkatkan kesehatan otak dan mengurangi risiko penyakit jantung.</li>
                    <li><strong>Quinoa:</strong> Sumber protein lengkap yang juga tinggi serat dan bebas gluten, baik untuk pencernaan dan menjaga berat badan.</li>
                    <li><strong>Kale:</strong> Sayuran hijau yang kaya vitamin K, C, dan A, serta mengandung senyawa anti-inflamasi yang baik untuk kesehatan jantung.</li>
                </ul>
            </li>
        </ul>
    </section>
    
    

    <section id="olahraga-aktivitas">
        <h3>Olahraga & Aktivitas Fisik</h3>
        <a class="back-button" href="#" onclick="hideAllSections()">Kembali</a>
        <ul>
            <li><strong>Panduan olahraga untuk pemula:</strong>
                <div class="video-container">
                    <iframe src="https://www.youtube.com/embed/bD4DdPGkSzw" allowfullscreen></iframe>
                </div>
            </li>
            <li><strong>Berbagai jenis latihan:</strong>
                <div class="video-container">
                    <iframe src="https://www.youtube.com/embed/cqseq21pIu4" allowfullscreen></iframe>
                </div>
            <li><strong>Video tutorial gerakan olahraga:</strong>
                    <div class="video-container">
                        <iframe src="https://www.youtube.com/embed/8p-72mZwDbI" allowfullscreen></iframe>
                    </div>
                </li>
            <li><strong>Program latihan mingguan:</strong> 
                <div class="table-container">
                    <table>
                        <tr>
                            <th>Hari</th>
                            <th>Fokus Latihan</th>
                            <th>Durasi</th>
                            <th>Intensitas</th>
                        </tr>
                        <tr>
                            <td>Senin</td>
                            <td>Kardio</td>
                            <td>30 Menit</td>
                            <td>Rendah</td>
                        </tr>
                        <tr>
                            <td>Selasa</td>
                            <td>Angkat Beban</td>
                            <td>45 Menit</td>
                            <td>Sedang</td>
                        </tr>
                        <tr>
                            <td>Rabu</td>
                            <td>Yoga</td>
                            <td>30 Menit</td>
                            <td>Rendah</td>
                        </tr>
                        <tr>
                            <td>Kamis</td>
                            <td>Plyometrics</td>
                            <td>30 Menit</td>
                            <td>Tinggi</td>
                        </tr>
                        <tr>
                            <td>Jumat</td>
                            <td>Istirahat</td>
                            <td>-</td>
                            <td>-</td>
                        </tr>
                        <tr>
                            <td>Sabtu</td>
                            <td>Olahraga Tim</td>
                            <td>60 Menit</td>
                            <td>Sedang</td>
                        </tr>
                        <tr>
                            <td>Minggu</td>
                            <td>Jalan Santai</td>
                            <td>30 Menit</td>
                            <td>Rendah</td>
                        </tr>
                    </table>
                </div>
            </li>
            <li><strong>Tips Motivasi Berolahraga:</strong>
                <ul>
                    <li><strong>Tetapkan Tujuan yang Jelas:</strong> 
                        Buatlah tujuan spesifik, terukur, dan realistis. Misalnya, "Saya ingin berlari sejauh 5 km dalam waktu 30 menit" daripada hanya mengatakan "Saya ingin berlari lebih banyak." Tujuan yang jelas membantu Anda fokus dan memberikan arah pada latihan Anda.</li>
                    
                    <li><strong>Mulai dengan Rencana:</strong> 
                        Buatlah jadwal latihan yang teratur. Tentukan hari dan waktu spesifik untuk berolahraga, dan anggaplah itu sebagai janji yang tidak bisa diabaikan. Misalnya, "Saya akan berolahraga setiap Senin, Rabu, dan Jumat pukul 18.00." Ini membantu membangun rutinitas.</li>
                    
                    <li><strong>Cari Teman Berolahraga:</strong> 
                        Bergabunglah dengan teman atau kelompok olahraga. Berolahraga bersama orang lain membuat aktivitas lebih menyenangkan dan memberikan dukungan sosial. Anda juga lebih cenderung untuk tidak melewatkan sesi latihan jika ada yang menunggu Anda.</li>
                    
                    <li><strong>Variasi Latihan:</strong> 
                        Cobalah berbagai jenis olahraga untuk menghindari kebosanan. Jika Anda biasanya berlari, coba bersepeda, berenang, atau mengikuti kelas aerobik. Variasi juga membantu melatih berbagai kelompok otot dan menjaga semangat tetap tinggi.</li>
                    
                    <li><strong>Catat Kemajuan Anda:</strong> 
                        Buatlah jurnal latihan untuk mencatat kemajuan Anda, seperti waktu lari, berat yang diangkat, atau jarak yang ditempuh. Melihat kemajuan Anda secara visual dapat menjadi motivasi yang kuat untuk terus berolahraga.</li>
                    
                    <li><strong>Rayakan Pencapaian Kecil:</strong> 
                        Berikan diri Anda penghargaan setiap kali mencapai tujuan kecil, seperti menyelesaikan satu minggu latihan atau meningkatkan jumlah repetisi. Ini bisa berupa sesuatu yang sederhana, seperti menonton film favorit atau menikmati makanan lezat.</li>
                    
                    <li><strong>Temukan Aktivitas yang Anda Nikmati:</strong> 
                        Fokuslah pada olahraga yang Anda nikmati. Jika Anda menyukai aktivitas tersebut, Anda akan lebih termotivasi untuk melakukannya secara teratur. Jika berlari terasa membosankan, pertimbangkan alternatif seperti menari, bersepeda, atau hiking.</li>
                    
                    <li><strong>Tetap Positif:</strong> 
                        Ubah pola pikir Anda menjadi positif. Alihkan fokus dari rasa sakit atau ketidaknyamanan selama latihan ke manfaat jangka panjang yang akan Anda peroleh. Ingatkan diri Anda tentang alasan mengapa Anda berolahraga dan bagaimana hal itu meningkatkan kualitas hidup Anda.</li>
                    
                    <li><strong>Ikuti Kelas atau Workshop:</strong> 
                        Mengikuti kelas olahraga atau workshop dapat memberikan motivasi tambahan. Anda akan mendapatkan bimbingan profesional dan bersosialisasi dengan orang lain yang memiliki tujuan yang sama, yang dapat membuat Anda merasa lebih terlibat.</li>
                    
                    <li><strong>Gunakan Teknologi:</strong> 
                        Manfaatkan aplikasi kebugaran atau perangkat pelacak aktivitas untuk memantau kemajuan Anda. Banyak aplikasi juga memiliki fitur komunitas yang memungkinkan Anda untuk berbagi pencapaian dan berinteraksi dengan orang lain.</li>
                </ul>
            </li>
                </section>

    <section id="kesehatan-mental">
        <h3>Kesehatan Mental</h3>
        <a class="back-button" href="#" onclick="hideAllSections()">Kembali</a>
        <ul>
            <li><strong>Panduan Meditasi dan Mindfulness:</strong>
                <ul>
                    <li><strong>Pengertian:</strong> Meditasi adalah praktik mental yang melibatkan teknik fokus untuk mencapai ketenangan pikiran dan kesadaran yang lebih tinggi. Mindfulness adalah bentuk meditasi yang menekankan perhatian penuh terhadap saat ini, tanpa menghakimi atau mengabaikan pengalaman yang muncul.</li>
                    <li><strong>Manfaat:</strong>
                        <ul>
                            <li>Mengurangi tingkat stres dan kecemasan, sehingga membantu individu merasa lebih tenang.</li>
                            <li>Meningkatkan kemampuan konsentrasi dan fokus, yang berkontribusi pada produktivitas yang lebih baik.</li>
                            <li>Membantu mengelola emosi negatif dan meningkatkan kesejahteraan mental secara keseluruhan.</li>
                            <li>Meningkatkan kualitas tidur, karena meditasi dapat membantu menenangkan pikiran sebelum tidur.</li>
                        </ul>
                    </li>
                    <li><strong>Teknik:</strong>
                        <ul>
                            <li><strong>Meditasi Pernapasan:</strong> Fokus pada pernapasan, sadari setiap tarikan dan hembusan napas tanpa mengubahnya.</li>
                            <li><strong>Body Scan:</strong> Mengamati dan merasakan setiap bagian tubuh dari kepala hingga kaki, mengenali ketegangan dan relaksasi.</li>
                            <li><strong>Meditasi Mengamati Pikiran:</strong> Amati pikiran yang muncul tanpa menghakimi, izinkan mereka datang dan pergi tanpa terjebak pada mereka.</li>
                        </ul>
                    </li>
                </ul>
            </li>
            
            <li><strong>Manajemen Stres:</strong>
                <ul>
                    <li><strong>Pengertian:</strong> Manajemen stres adalah rangkaian teknik dan strategi yang digunakan untuk mengurangi tingkat stres dan meningkatkan kesejahteraan mental. Ini melibatkan pemahaman pemicu stres dan penerapan strategi untuk mengatasinya.</li>
                    <li><strong>Manfaat:</strong>
                        <ul>
                            <li>Meningkatkan kesehatan fisik dan mental, mengurangi risiko penyakit akibat stres.</li>
                            <li>Menambah energi dan fokus, memungkinkan individu untuk lebih produktif.</li>
                            <li>Meningkatkan kualitas hubungan interpersonal dengan mengurangi ketegangan.</li>
                        </ul>
                    </li>
                    <li><strong>Cara-cara:</strong>
                        <ul>
                            <li><strong>Olahraga Teratur:</strong> Aktivitas fisik yang rutin dapat membantu melepaskan endorfin, yang merupakan bahan kimia otak yang meningkatkan suasana hati.</li>
                            <li><strong>Teknik Relaksasi:</strong> Praktik seperti pernapasan dalam, yoga, dan meditasi untuk menenangkan pikiran dan tubuh.</li>
                            <li><strong>Jurnal Stres:</strong> Menulis tentang pengalaman dan perasaan terkait stres untuk memahami pemicu dan menemukan solusi yang tepat.</li>
                            <li><strong>Mengatur Waktu:</strong> Membuat daftar tugas dan menentukan prioritas untuk menghindari rasa kewalahan.</li>
                        </ul>
                    </li>
                </ul>
            </li>
            
            <li><strong>Tips untuk Tidur yang Lebih Baik:</strong>
                <ul>
                    <li><strong>Pengertian:</strong> Tidur yang berkualitas adalah kondisi di mana tubuh dan pikiran dapat beristirahat dan memulihkan diri sepenuhnya. Tidur yang baik penting untuk kesehatan fisik dan mental.</li>
                    <li><strong>Manfaat:</strong>
                        <ul>
                            <li>Meningkatkan fungsi kognitif, termasuk perhatian dan konsentrasi.</li>
                            <li>Mendukung kesehatan fisik dengan memperkuat sistem kekebalan tubuh.</li>
                            <li>Mengurangi risiko gangguan mental seperti depresi dan kecemasan.</li>
                        </ul>
                    </li>
                    <li><strong>Strategi:</strong>
                        <ul>
                            <li><strong>Tetapkan Rutinitas Tidur:</strong> Tidur dan bangun pada waktu yang sama setiap hari untuk mengatur ritme sirkadian tubuh.</li>
                            <li><strong>Lingkungan Tidur yang Nyaman:</strong> Pastikan kamar tidur gelap, tenang, dan sejuk untuk menciptakan lingkungan yang kondusif untuk tidur.</li>
                            <li><strong>Batasi Paparan Layar:</strong> Hindari menggunakan perangkat elektronik setidaknya satu jam sebelum tidur untuk mengurangi paparan cahaya biru.</li>
                            <li><strong>Hindari Kafein dan Makanan Berat:</strong> Batasi konsumsi kafein dan makanan berat beberapa jam sebelum tidur untuk mencegah gangguan tidur.</li>
                        </ul>
                    </li>
                </ul>
            </li>
            
            <li><strong>Informasi tentang Gangguan Mental:</strong>
                <ul>
                    <li><strong>Pengertian:</strong> Gangguan mental adalah kondisi yang memengaruhi pemikiran, perasaan, dan perilaku seseorang, dan dapat mengganggu fungsi sehari-hari serta kualitas hidup.</li>
                    <li><strong>Contoh Gangguan Mental:</strong>
                        <ul>
                            <li><strong>Depresi:</strong> Suasana hati yang terus-menerus sedih dan kehilangan minat dalam aktivitas sehari-hari.</li>
                            <li><strong>Kecemasan:</strong> Perasaan khawatir yang berlebihan yang dapat mengganggu aktivitas sehari-hari.</li>
                            <li><strong>Gangguan Bipolar:</strong> Perubahan suasana hati yang ekstrem, dari depresi hingga manik.</li>
                            <li><strong>Skizofrenia:</strong> Gangguan yang memengaruhi pemikiran, perasaan, dan perilaku, seringkali menyebabkan halusinasi.</li>
                        </ul>
                    </li>
                    <li><strong>Sumber Daya:</strong>
                        <ul>
                            <li>Konselor dan psikolog untuk terapi individual yang membantu mengatasi masalah kesehatan mental.</li>
                            <li>Grup dukungan untuk berbagi pengalaman dan mendapatkan dukungan dari orang-orang dengan masalah serupa.</li>
                            <li>Informasi dari situs web kesehatan mental yang terpercaya untuk meningkatkan pemahaman tentang gangguan mental.</li>
                        </ul>
                    </li>
                </ul>
            </li>
            
            <li><strong>Pentingnya Dukungan Sosial:</strong>
                <ul>
                    <li><strong>Pengertian:</strong> Dukungan sosial adalah bantuan emosional, informasi, atau fisik yang diberikan oleh orang-orang di sekitar kita, yang dapat membantu mengatasi stres dan tantangan hidup.</li>
                    <li><strong>Peran Dukungan Sosial dalam Kesehatan Mental:</strong>
                        <ul>
                            <li>Meningkatkan rasa memiliki dan mengurangi perasaan kesepian, yang dapat memperbaiki kesehatan mental.</li>
                            <li>Memberikan perspektif yang berbeda dan dukungan dalam menghadapi masalah, sehingga individu merasa tidak sendirian.</li>
                            <li>Meningkatkan rasa percaya diri dan kemampuan mengatasi masalah, berkontribusi pada pengembangan keterampilan koping.</li>
                        </ul>
                    </li>
                    <li><strong>Cara Mencari Dukungan Sosial:</strong>
                        <ul>
                            <li>Bergabung dengan kelompok atau komunitas yang memiliki minat yang sama untuk bertemu dengan orang baru.</li>
                            <li>Berbicara dengan teman dekat atau keluarga tentang perasaan Anda untuk mendapatkan dukungan emosional.</li>
                            <li>Mencari bantuan profesional jika merasa kesulitan mengatasi stres atau emosi, seperti terapis atau konselor.</li>
                        </ul>
                    </li>
                </ul>
            </li>
                    </ul>
    </section>
    <section id="pola-tidur">
        <h3>Pola Tidur</h3>
        <a class="back-button" href="#" onclick="hideAllSections()">Kembali</a>
    
        <div class="table-container">
            <h4>1. Tips Tidur Berkualitas</h4>
            <table>
                <tr>
                    <th>Hari</th>
                    <th>Jam Tidur</th>
                    <th>Jam Bangun</th>
                    <th>Durasi Tidur</th>
                </tr>
                <tr>
                    <td>Senin</td>
                    <td>22:00</td>
                    <td>06:00</td>
                    <td>8 Jam</td>
                </tr>
                <tr>
                    <td>Selasa</td>
                    <td>23:00</td>
                    <td>07:00</td>
                    <td>8 Jam</td>
                </tr>
                <tr>
                    <td>Rabu</td>
                    <td>22:30</td>
                    <td>06:30</td>
                    <td>8 Jam</td>
                </tr>
                <tr>
                    <td>Kamis</td>
                    <td>22:45</td>
                    <td>06:45</td>
                    <td>8 Jam</td>
                </tr>
                <tr>
                    <td>Jumat</td>
                    <td>23:15</td>
                    <td>07:15</td>
                    <td>8 Jam</td>
                </tr>
                <tr>
                    <td>Sabtu</td>
                    <td>23:00</td>
                    <td>08:00</td>
                    <td>9 Jam</td>
                </tr>
                <tr>
                    <td>Minggu</td>
                    <td>22:00</td>
                    <td>07:00</td>
                    <td>9 Jam</td>
                </tr>
            </table>
        </div>
    
        <div class="tracking-container">
            <h4>2. Tracking Jadwal Tidur</h4>
            <label for="sleepDate">Tanggal:</label>
            <input type="date" id="sleepDate" name="sleepDate" class="styled-input"><br><br>
            
            <label for="sleepTime">Waktu Tidur:</label>
            <input type="time" id="sleepTime" name="sleepTime" class="styled-input"><br><br>
    
            <label for="wakeTime">Waktu Bangun:</label>
            <input type="time" id="wakeTime" name="wakeTime" class="styled-input"><br><br>
    
            <label for="sleepQuality">Kualitas Tidur:</label>
            <input type="text" id="sleepQuality" name="sleepQuality" class="styled-input" readonly><br><br>
    
            <button class="save-button" onclick="saveSleepData()">Simpan</button>
            <button class="delete-button" onclick="clearHistory()">Hapus Riwayat</button>
    
            <h5>Riwayat Tidur:</h5>
            <ul id="sleepHistory"></ul>
        </div>
    
        <div class="insomnia-container">
            <h4>3. Cara Mengatasi Insomnia</h4>
            <p>Jika Anda mengalami kesulitan tidur, kami sarankan untuk menonton video berikut tentang cara mengatasi insomnia:</p>
            <iframe width="560" height="315" src="https://www.youtube.com/embed/-p-FFFe-AiQ" title="Cara Mengatasi Insomnia" frameborder="0" allowfullscreen></iframe>
        </div>
    
        <div class="benefits-container">
            <h4>4. Manfaat Tidur Cukup untuk Kesehatan</h4>
            <ul>
                <li><strong>Kesehatan Fisik:</strong> Tidur yang cukup mendukung sistem kekebalan tubuh, membantu pemulihan fisik, dan mengurangi risiko penyakit kronis.</li>
                <li><strong>Kesehatan Mental:</strong> Tidur yang berkualitas dapat meningkatkan mood, mengurangi stres, dan mengurangi risiko gangguan mental.</li>
                <li><strong>Fungsi Pemulihan:</strong> Selama tidur, tubuh memperbaiki sel dan jaringan, memproduksi hormon pertumbuhan, dan mengatur metabolisme.</li>
            </ul>
        </div>
    </section>
    
    <style>
        .styled-input, .styled-select {
            width: 100%;
            padding: 10px;
            margin: 5px 0 20px 0;
            border: 2px solid #4CAF50; /* Border color */
            border-radius: 5px; /* Rounded corners */
            background-color: #f9f9f9; /* Background color */
            transition: border 0.3s;
        }
    
        .styled-input:focus, .styled-select:focus {
            border: 2px solid #007BFF; /* Border color when focused */
            outline: none; /* Remove default outline */
        }
    
        .save-button, .delete-button {
            background-color: #4CAF50; /* Green background */
            color: white; /* White text */
            padding: 10px 20px; /* Padding */
            border: none; /* Remove border */
            border-radius: 5px; /* Rounded corners */
            cursor: pointer; /* Pointer cursor on hover */
            font-size: 16px; /* Font size */
            margin-right: 10px; /* Space between buttons */
        }
    
        .save-button:hover {
            background-color: #45a049; /* Darker green on hover */
        }
    
        .delete-button {
            background-color: #f44336; /* Red background */
        }
    
        .delete-button:hover {
            background-color: #d32f2f; /* Darker red on hover */
        }
    
        h3, h4 {
            color: #333; /* Darker text color for headings */
        }
    
        label {
            font-weight: bold; /* Bold labels */
        }
    </style>
    
    <script>
        const sleepHistory = [];
    
        function saveSleepData() {
            const sleepDate = document.getElementById("sleepDate").value;
            const sleepTime = document.getElementById("sleepTime").value;
            const wakeTime = document.getElementById("wakeTime").value;
    
            if (sleepDate && sleepTime && wakeTime) {
                const sleepQuality = calculateSleepQuality(sleepTime, wakeTime);
                const sleepRecord = `Tanggal: ${sleepDate}, Waktu Tidur: ${sleepTime}, Waktu Bangun: ${wakeTime}, Kualitas Tidur: ${sleepQuality}`;
                sleepHistory.push(sleepRecord);
                document.getElementById("sleepQuality").value = sleepQuality; // Update the sleep quality input
                displaySleepHistory();
                clearInputs();
            } else {
                alert("Silakan isi semua field.");
            }
        }
    
        function calculateSleepQuality(sleepTime, wakeTime) {
            const sleepHour = parseInt(sleepTime.split(':')[0]);
            const sleepMinute = parseInt(sleepTime.split(':')[1]);
            const wakeHour = parseInt(wakeTime.split(':')[0]);
            const wakeMinute = parseInt(wakeTime.split(':')[1]);
    
            // Calculate total sleep duration in hours
            const totalSleepMinutes = (wakeHour * 60 + wakeMinute) - (sleepHour * 60 + sleepMinute);
            if (totalSleepMinutes >= 480 && totalSleepMinutes < 540) {
                return 'Baik'; // 8 Jam
            } else if (totalSleepMinutes >= 540) {
                return 'Sangat Baik'; // > 8 Jam
            } else if (totalSleepMinutes >= 420) {
                return 'Cukup'; // 7 Jam
            } else {
                return 'Kurang'; // < 7 Jam
            }
        }
    
        function displaySleepHistory() {
            const historyList = document.getElementById("sleepHistory");
            historyList.innerHTML = "";
            sleepHistory.forEach(record => {
                const li = document.createElement("li");
                li.textContent = record;
                historyList.appendChild(li);
            });
        }
    
        function clearInputs() {
            document.getElementById("sleepDate").value = "";
            document.getElementById("sleepTime").value = "";
            document.getElementById("wakeTime").value = "";
            document.getElementById("sleepQuality").value = ""; // Clear quality input
        }
    
        function clearHistory() {
            sleepHistory.length = 0; // Clear the sleep history array
            displaySleepHistory(); // Update the displayed history
        }
    </script>
        
    <section id="tips-pencegahan">
        <h3>Tips Pencegahan Penyakit</h3>
        <a class="back-button" href="#" onclick="hideAllSections()">Kembali</a>
        <ul>
            <li><strong>Vaksinasi yang dianjurkan:</strong>
                <p>Vaksinasi adalah proses pemberian vaksin untuk membangun kekebalan tubuh terhadap penyakit tertentu. Vaksin bekerja dengan memperkenalkan antigen ke dalam tubuh, yang merangsang sistem kekebalan untuk memproduksi antibodi dan menciptakan memori imunologis. Vaksinasi penting dalam mencegah penyakit menular yang bisa menyebabkan komplikasi serius.</p>
                <p><strong>Cara Vaksinasi:</strong></p>
                <ul>
                    <li><strong>Jadwal Vaksinasi:</strong> Vaksinasi biasanya dimulai sejak usia bayi. Vaksin yang dianjurkan termasuk vaksin DPT (Difteri, Pertusis, dan Tetanus), vaksin polio, vaksin hepatitis B, serta vaksinasi tambahan seperti MMR (Campak, Gondong, dan Rubella) pada usia anak-anak. Vaksin lanjutan atau booster diberikan pada usia tertentu untuk menjaga kekebalan.</li>
                    <li><strong>Tipe Vaksin:</strong> Terdapat berbagai jenis vaksin, termasuk vaksin hidup yang dilemahkan, vaksin mati, dan vaksin subunit. Masing-masing memiliki metode pemberian yang berbeda, seperti injeksi, oral, atau intranasal.</li>
                    <li><strong>Pentingnya Vaksinasi:</strong> Vaksinasi tidak hanya melindungi individu tetapi juga membantu menciptakan kekebalan kelompok (herd immunity), yang sangat penting untuk melindungi mereka yang tidak dapat divaksinasi, seperti bayi dan orang dengan sistem kekebalan yang lemah.</li>
                </ul>
            </li>
            <li><strong>Pola hidup sehat:</strong>
                <p>Pola hidup sehat mencakup serangkaian kebiasaan yang mendukung kesehatan fisik dan mental. Kebiasaan ini meliputi pola makan yang seimbang, olahraga teratur, serta istirahat yang cukup. Menerapkan pola hidup sehat dapat mencegah berbagai penyakit, meningkatkan kualitas hidup, dan memperpanjang harapan hidup.</p>
                <p><strong>Komponen Pola Hidup Sehat:</strong></p>
                <ul>
                    <li><strong>Pola Makan Sehat:</strong> Penting untuk mengonsumsi berbagai makanan bergizi, termasuk sayuran, buah-buahan, biji-bijian utuh, protein tanpa lemak, dan lemak sehat. Membatasi konsumsi gula, garam, dan lemak jenuh juga sangat dianjurkan.</li>
                    <li><strong>Olahraga Teratur:</strong> Disarankan untuk melakukan aktivitas fisik minimal 150 menit per minggu. Olahraga tidak hanya membantu mengontrol berat badan, tetapi juga meningkatkan kesehatan jantung, mengurangi risiko diabetes, dan meningkatkan kesehatan mental.</li>
                    <li><strong>Istirahat yang Cukup:</strong> Tidur yang berkualitas sangat penting untuk pemulihan tubuh. Orang dewasa disarankan untuk tidur antara 7 hingga 9 jam setiap malam. Tidur yang cukup membantu menjaga fungsi kognitif, kesehatan emosional, dan sistem kekebalan tubuh.</li>
                    <li><strong>Manajemen Stres:</strong> Mengelola stres melalui teknik relaksasi seperti meditasi, yoga, atau aktivitas fisik dapat membantu menjaga kesehatan mental. Mengatur waktu untuk diri sendiri dan melakukan aktivitas yang menyenangkan juga berkontribusi pada pola hidup sehat.</li>
                </ul>
            </li>
            <li><strong>Pemeriksaan kesehatan rutin:</strong>
                <p>Pemeriksaan kesehatan rutin adalah serangkaian tes dan evaluasi yang dilakukan untuk memantau kesehatan dan mendeteksi masalah kesehatan sedini mungkin. Melakukan pemeriksaan kesehatan secara teratur dapat membantu mencegah dan mengelola penyakit dengan lebih efektif.</p>
                <p><strong>Pentingnya Pemeriksaan Rutin:</strong></p>
                <ul>
                    <li><strong>Deteksi Dini Penyakit:</strong> Pemeriksaan rutin dapat membantu mengidentifikasi kondisi seperti hipertensi, diabetes, dan kolesterol tinggi sebelum berkembang menjadi masalah serius. Semakin dini masalah kesehatan terdeteksi, semakin besar peluang untuk penanganan yang efektif.</li>
                    <li><strong>Monitoring Kesehatan:</strong> Dengan melakukan pemeriksaan kesehatan, individu dapat memantau perubahan dalam kesehatan mereka seiring waktu. Ini juga membantu mendapatkan rekomendasi untuk perubahan gaya hidup jika diperlukan.</li>
                    <li><strong>Konsultasi dengan Tenaga Medis:</strong> Pemeriksaan kesehatan juga memberikan kesempatan untuk berdiskusi dengan dokter tentang masalah kesehatan, mendapatkan saran yang tepat, dan melakukan tes yang sesuai berdasarkan usia, riwayat kesehatan, dan risiko.</li>
                    <li><strong>Pemantauan Kesehatan Mental:</strong> Pemeriksaan kesehatan rutin juga termasuk evaluasi kesehatan mental. Diskusi tentang perasaan dan kondisi mental Anda penting untuk pencegahan dan pengelolaan masalah kesehatan mental.</li>
                </ul>
            </li>
            <li><strong>Tips menghindari penyakit menular:</strong>
                <p>Penyakit menular dapat menyebar melalui kontak langsung, udara, atau permukaan yang terkontaminasi. Mengadopsi kebiasaan sehat adalah cara terbaik untuk melindungi diri dari infeksi.</p>
                <p><strong>Cara Menghindari Penyakit Menular:</strong></p>
                <ul>
                    <li><strong>Mencuci Tangan Secara Teratur:</strong> Mencuci tangan dengan sabun dan air mengalir selama minimal 20 detik sangat efektif dalam mencegah penyebaran infeksi. Gunakan pembersih tangan berbasis alkohol jika sabun tidak tersedia.</li>
                    <li><strong>Vaksinasi:</strong> Mengikuti jadwal vaksinasi yang dianjurkan untuk melindungi diri dari penyakit menular. Vaksinasi mencegah infeksi dan penyebaran virus ke orang lain.</li>
                    <li><strong>Menghindari Keramaian:</strong> Menghindari tempat ramai, terutama saat terjadi wabah penyakit menular, dapat membantu mengurangi risiko infeksi. Jika harus berada di keramaian, gunakan masker dan pertahankan jarak sosial.</li>
                    <li><strong>Kebersihan Lingkungan:</strong> Menjaga kebersihan lingkungan dan mendisinfeksi permukaan yang sering disentuh, seperti gagang pintu dan meja, dapat membantu mencegah penyebaran penyakit.</li>
                    <li><strong>Etika Batuk dan Bersin:</strong> Menutupi mulut dan hidung dengan tisu atau siku saat batuk atau bersin, serta membuang tisu dengan benar, membantu melindungi orang lain dari penularan penyakit.</li>
                </ul>
            </li>
            <li><strong>Perawatan kesehatan mental:</strong>
                <p>Perawatan kesehatan mental sangat penting dalam mencegah dan mengelola masalah kesehatan mental. Kesehatan mental yang baik membantu individu mengelola stres, berinteraksi dengan orang lain, dan membuat keputusan yang baik. Perawatan ini mencakup berbagai pendekatan, mulai dari terapi hingga perubahan gaya hidup.</p>
                <p><strong>Cara Merawat Kesehatan Mental:</strong></p>
                <ul>
                    <li><strong>Berbicara dengan Profesional:</strong> Jika merasa tertekan atau cemas, penting untuk berbicara dengan profesional kesehatan mental, seperti psikolog atau psikiater, untuk mendapatkan dukungan dan bimbingan. Terapi kognitif-perilaku, terapi psikodinamik, dan konseling adalah beberapa bentuk terapi yang bisa dipertimbangkan.</li>
                    <li><strong>Aktivitas yang Menyenangkan:</strong> Luangkan waktu untuk melakukan kegiatan yang disukai, seperti hobi, olahraga, atau berkumpul dengan teman. Aktivitas ini membantu mengurangi stres dan meningkatkan suasana hati.</li>
                    <li><strong>Mindfulness dan Meditasi:</strong> Praktik mindfulness dan meditasi dapat membantu menenangkan pikiran dan meningkatkan kesadaran diri. Teknik ini juga dapat mengurangi gejala kecemasan dan depresi.</li>
                    <li><strong>Dukungan Sosial:</strong> Berinteraksi dengan keluarga dan teman dapat memberikan dukungan emosional, mengurangi perasaan kesepian, dan membantu dalam mengatasi masalah. Membangun jaringan sosial yang kuat dapat menjadi pelindung terhadap masalah kesehatan mental.</li>
                    <li><strong>Aktivitas Fisik:</strong> Olahraga teratur terbukti dapat meningkatkan suasana hati dan mengurangi gejala depresi. Aktivitas fisik melepaskan endorfin, yang berfungsi sebagai penghilang stres alami.</li>
                    <li><strong>Pentingnya Istirahat:</strong> Memberikan diri Anda waktu untuk beristirahat dan bersantai adalah penting untuk menjaga kesehatan mental. Cobalah untuk tidak membebani diri Anda dengan tanggung jawab yang berlebihan dan prioritaskan waktu untuk diri sendiri.</li>
                </ul>
            </li>        </ul>
    </section>

    <section id="resep-makanan">
        <h3>Resep Makanan Sehat</h3>
        <a class="back-button" href="#" onclick="hideAllSections()">Kembali</a>
        <ul>
            <li><strong>Rekomendasi Sarapan Sehat:</strong>
                <p>Untuk memulai hari dengan energi yang cukup, sarapan sehat sangat penting. Sarapan yang kaya serat, protein, dan vitamin dapat meningkatkan fokus dan produktivitas sepanjang hari.</p>
                <p><strong>Resep Oatmeal Buah:</strong></p>
                <ul>
                    <li><strong>Bahan:</strong>
                        <ul>
                            <li>1 cangkir oatmeal</li>
                            <li>2 cangkir susu almond (atau air)</li>
                            <li>1/2 pisang, diiris</li>
                            <li>1/4 cangkir blueberry</li>
                            <li>1 sdm madu atau maple syrup (opsional)</li>
                            <li>Sejumput kayu manis</li>
                        </ul>
                    </li>
                    <li><strong>Cara Membuat:</strong>
                        <ol>
                            <li>Didihkan susu almond dalam panci.</li>
                            <li>Tambahkan oatmeal dan masak selama 5-7 menit hingga oatmeal menjadi lembut.</li>
                            <li>Angkat dari api, tambahkan pisang, blueberry, dan madu/maple syrup.</li>
                            <li>Taburi dengan kayu manis sebelum disajikan.</li>
                        </ol>
                    </li>
                </ul>
            </li>
            <li><strong>Makanan Rendah Kalori:</strong>
                <p>Makanan rendah kalori adalah pilihan cerdas untuk menjaga berat badan ideal tanpa mengorbankan rasa. Pilihan makanan ini dapat membantu Anda merasa kenyang lebih lama.</p>
                <p><strong>Resep Salad Sayuran Segar:</strong></p>
                <ul>
                    <li><strong>Bahan:</strong>
                        <ul>
                            <li>2 cangkir campuran sayuran hijau (selada, bayam, arugula)</li>
                            <li>1/2 mentimun, diiris tipis</li>
                            <li>1/2 paprika merah, dipotong dadu</li>
                            <li>1/4 bawang merah, diiris tipis</li>
                            <li>1/4 cangkir cuka balsamik</li>
                            <li>1 sdm minyak zaitun</li>
                            <li>Garam dan merica secukupnya</li>
                        </ul>
                    </li>
                    <li><strong>Cara Membuat:</strong>
                        <ol>
                            <li>Campurkan sayuran dalam mangkuk besar.</li>
                            <li>Dalam wadah terpisah, campurkan cuka balsamik, minyak zaitun, garam, dan merica.</li>
                            <li>Tuangkan dressing ke atas salad dan aduk hingga merata.</li>
                            <li>Sajikan segera.</li>
                        </ol>
                    </li>
                </ul>
            </li>
            <li><strong>Smoothie Sehat:</strong>
                <p>Smoothie adalah cara yang lezat untuk mendapatkan nutrisi dari buah dan sayuran. Smoothie yang sehat dapat menjadi camilan atau sarapan yang kaya vitamin.</p>
                <p><strong>Resep Smoothie Hijau:</strong></p>
                <ul>
                    <li><strong>Bahan:</strong>
                        <ul>
                            <li>1 cangkir bayam segar</li>
                            <li>1/2 pisang</li>
                            <li>1/2 cangkir yogurt plain</li>
                            <li>1 cangkir susu almond</li>
                            <li>1 sdm selai kacang</li>
                            <li>Es batu secukupnya</li>
                        </ul>
                    </li>
                    <li><strong>Cara Membuat:</strong>
                        <ol>
                            <li>Masukkan semua bahan ke dalam blender.</li>
                            <li>Blender hingga halus dan semua bahan tercampur rata.</li>
                            <li>Tuangkan ke dalam gelas dan nikmati segera.</li>
                        </ol>
                    </li>
                </ul>
            </li>
            <li><strong>Camilan Bergizi:</strong>
                <p>Camilan bergizi adalah alternatif sehat untuk menghindari camilan tidak sehat. Memilih camilan yang kaya protein dan serat akan membantu Anda tetap kenyang dan berenergi.</p>
                <p><strong>Resep Camilan Energy Balls:</strong></p>
                <ul>
                    <li><strong>Bahan:</strong>
                        <ul>
                            <li>1 cangkir oat</li>
                            <li>1/2 cangkir selai kacang</li>
                            <li>1/4 cangkir madu</li>
                            <li>1/4 cangkir cokelat chip atau kismis</li>
                            <li>1/4 cangkir biji chia atau biji rami (opsional)</li>
                        </ul>
                    </li>
                    <li><strong>Cara Membuat:</strong>
                        <ol>
                            <li>Campurkan semua bahan dalam mangkuk besar.</li>
                            <li>Aduk hingga semua bahan tercampur rata.</li>
                            <li>Ambil sejumput adonan dan bulatkan menjadi bola kecil.</li>
                            <li>Letakkan bola di atas loyang dan masukkan ke dalam lemari es selama 30 menit sebelum disajikan.</li>
                        </ol>
                    </li>
                    </ul>
    </section>

    <section id="kalkulator-bmi">
        <h3>Kalkulator BMI</h3>
        <a class="back-button" href="#" onclick="hideAllSections()">Kembali</a>
        <p>Masukkan nama, berat badan (kg), dan tinggi badan (m) untuk menghitung BMI Anda:</p>
        <form id="bmi-form" onsubmit="return calculateBMI();">
            <input type="text" id="name" placeholder="Nama Anda" required>
            <input type="number" id="weight" placeholder="Berat Badan (kg)" required>
            <input type="number" id="height" placeholder="Tinggi Badan (m)" required>
            <button type="submit" class="calculate-button">Hitung BMI</button>
            <button type="button" class="reset-button" onclick="resetBMI()">Hapus</button>
        </form>
        <p id="bmi-result"></p>
    </section>
    
    <section id="kalkulator-bmi">
        <h3>Kalkulator BMI</h3>
        <a class="back-button" href="#" onclick="hideAllSections()">Kembali</a>
        <p>Masukkan nama, berat badan (kg), dan tinggi badan (m) untuk menghitung BMI Anda:</p>
        <form id="bmi-form" onsubmit="return calculateBMI();">
            <input type="text" id="name" placeholder="Nama Anda" required>
            <input type="number" id="weight" placeholder="Berat Badan (kg)" required>
            <input type="number" id="height" placeholder="Tinggi Badan (m)" required>
            <button type="submit" class="calculate-button">Hitung BMI</button>
            <button type="button" class="reset-button" onclick="resetBMI()">Hapus</button>
        </form>
        <p id="bmi-result"></p>
    
        <h4>Riwayat BMI</h4>
        <table id="history-table">
            <thead>
                <tr>
                    <th>Nama</th>
                    <th>Berat Badan (kg)</th>
                    <th>Tinggi Badan (m)</th>
                    <th>BMI</th>
                </tr>
            </thead>
            <tbody id="history-list"></tbody>
        </table>
    </section>
    
    <style>
        #kalkulator-bmi {
            padding: 20px;
            border: 1px solid #ccc;
            border-radius: 8px;
            background-color: #f9f9f9;
            max-width: 600px;
            margin: 0 auto;
        }
    
        input[type="text"],
        input[type="number"] {
            width: calc(100% - 20px);
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 4px;
            font-size: 16px;
        }
    
        .calculate-button {
            background-color: #4CAF50; /* Hijau */
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
            margin-right: 10px;
        }
    
        .calculate-button:hover {
            background-color: #45a049; /* Warna hijau lebih gelap saat hover */
        }
    
        .reset-button {
            background-color: #f44336; /* Merah */
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
        }
    
        .reset-button:hover {
            background-color: #e53935; /* Warna merah lebih gelap saat hover */
        }
    
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 10px;
        }
    
        th, td {
            border: 1px solid #ccc;
            padding: 8px;
            text-align: left;
        }
    
        th {
            background-color: #f2f2f2;
        }
    </style>
    
    <script>
        function calculateBMI() {
            var name = document.getElementById('name').value;
            var weight = parseFloat(document.getElementById('weight').value);
            var height = parseFloat(document.getElementById('height').value);
            var resultElement = document.getElementById('bmi-result');
    
            if (weight > 0 && height > 0) {
                var bmi = (weight / (height * height)).toFixed(2);
                resultElement.textContent = name + ", BMI Anda adalah: " + bmi;
    
                // Menambahkan riwayat ke tabel
                addToHistory(name, weight, height, bmi);
            } else {
                resultElement.textContent = "Mohon masukkan angka yang valid.";
            }
    
            return false; // Mencegah form submit
        }
    
        function addToHistory(name, weight, height, bmi) {
            var tableBody = document.getElementById('history-list');
            var row = document.createElement('tr');
    
            row.innerHTML = `
                <td>${name}</td>
                <td>${weight}</td>
                <td>${height}</td>
                <td>${bmi}</td>
            `;
            tableBody.appendChild(row);
        }
    
        function resetBMI() {
            document.getElementById('name').value = '';
            document.getElementById('weight').value = '';
            document.getElementById('height').value = '';
            document.getElementById('bmi-result').textContent = '';
            document.getElementById('history-list').innerHTML = ''; // Menghapus riwayat
        }
    </script>            
    
    <section id="my-team">
        <h3>My Team</h3>
        <a class="back-button" href="#" onclick="hideAllSections()">Kembali</a>
        <ul>
            <li>
                <button class="member-button">
                    Sintia Adea Ananda ✨ Nim. 1420123051
                </button>
            </li>
            <li>
                <button class="member-button">
                    Gita Rahma Putri ✨ Nim. 1420123059
                </button>
            </li>
            <li>
                <button class="member-button">
                    Baiq I'is Maulida ✨ Nim. 1420123077
                </button>
            </li>
            <li>
                <button class="member-button">
                    Firman Ali Fikri ✨ Nim. 1420123088
                </button>
            </li>
            <li>
                <button class="member-button">
                    Septy Aulia ✨ Nim. 1420123089
                </button>
            </li>
            <li>
                <button class="member-button">
                    Fahmi Idris ✨ Nim. 1420123095
                </button>
            </li>
            <li>
                <button class="member-button">
                    Aulia Safitri ✨ Nim. 1420123097
                </button>
            </li>
        </ul>
    </section>
    
    <style>
        #my-team {
            padding: 20px;
            border: 2px solid #4CAF50; /* Hijau */
            border-radius: 8px;
            background-color: #f9f9f9;
            max-width: 600px;
            margin: 20px auto;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }
    
        h3 {
            text-align: center;
            color: #333;
            font-family: Arial, sans-serif;
        }
    
        .back-button {
            display: inline-block;
            margin: 10px 0;
            text-decoration: none;
            background-color: #f44336; /* Merah */
            color: white;
            padding: 8px 16px;
            border-radius: 4px;
            transition: background-color 0.3s ease;
        }
    
        .back-button:hover {
            background-color: #e53935; /* Merah lebih gelap saat hover */
        }
    
        ul {
            list-style: none;
            padding: 0;
        }
    
        li {
            margin: 10px 0;
        }
    
        .member-button {
            width: 100%;
            padding: 12px;
            border: none;
            border-radius: 5px;
            background-color: #0000FF; /* Hijau */
            color: white;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            transition: background-color 0.3s ease;
            text-align: left;
        }
    
        .member-button:hover {
            background-color: #45a049; /* Hijau lebih gelap saat hover */
        }
    </style>
    </div>

<script>
    function showSection(sectionId) {
        hideAllSections();
        document.getElementById(sectionId).style.display = 'block';
    }

    function hideAllSections() {
        const sections = document.querySelectorAll('.content > section');
        sections.forEach(section => section.style.display = 'none');
    }

    function calculateBMI() {
        const weight = document.getElementById('weight').value;
        const height = document.getElementById('height').value;
        const bmi = weight / (height * height);
        document.getElementById('bmi-result').innerText = `BMI Anda adalah: ${bmi.toFixed(2)}`;
        return false; // Prevent form submission
    }
</script>

</body>
</html>

