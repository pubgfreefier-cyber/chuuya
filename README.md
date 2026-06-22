<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>كايدن - أكبر مكتبة للقصص المصورة المترجمة | 1000+ عمل</title>
    <style>
        :root {
            --bg: #0D0618;
            --card: #150A24;
            --primary: #7C3AED;
            --light: #A78BFA;
            --neon: #C4B5FD;
            --gold: #FBBF24;
            --text: #EDE9FE;
            --muted: #8B7AA8;
            --border: #2D1B4E;
            --radius: 14px;
        }
        *{margin:0;padding:0;box-sizing:border-box}
        body{font-family:'Segoe UI',Tahoma,sans-serif;background:var(--bg);color:var(--text);line-height:1.6}
        
        .header{position:fixed;top:0;left:0;width:100%;z-index:999;background:rgba(13,6,24,0.92);backdrop-filter:blur(16px);border-bottom:1px solid var(--border);padding:10px 0}
        .header-inner{max-width:1300px;margin:0 auto;padding:0 20px;display:flex;align-items:center;justify-content:space-between;gap:12px;flex-wrap:wrap}
        .logo{display:flex;align-items:center;gap:8px;text-decoration:none;color:var(--text);font-size:1.6rem;font-weight:900}
        .logo-icon{font-size:1.8rem}
        .logo span{background:linear-gradient(135deg,#7C3AED,#C4B5FD);-webkit-background-clip:text;-webkit-text-fill-color:transparent}
        .search-box{display:flex;align-items:center;gap:6px}
        .search-box input{padding:10px 16px;border-radius:50px;border:2px solid var(--border);background:rgba(255,255,255,0.04);color:var(--text);font-size:0.9rem;width:220px;outline:none;font-family:inherit}
        .search-box input:focus{border-color:var(--primary)}
        .btn{padding:10px 20px;border-radius:50px;border:none;cursor:pointer;font-weight:700;font-size:0.85rem;transition:all 0.3s;font-family:inherit}
        .btn-primary{background:linear-gradient(135deg,#7C3AED,#A78BFA);color:white}
        .btn-outline{border:2px solid var(--light);background:transparent;color:var(--neon)}
        .btn:hover{transform:translateY(-2px);box-shadow:0 0 20px rgba(124,58,237,0.3)}
        .nav-links{display:flex;gap:2px;flex-wrap:wrap;padding:4px 20px;max-width:1300px;margin:0 auto}
        .nav-links a{color:var(--muted);text-decoration:none;padding:7px 14px;border-radius:50px;font-size:0.82rem;font-weight:500}
        .nav-links a:hover,.nav-links a.active{color:var(--text);background:rgba(124,58,237,0.15)}

        .main-content{margin-top:130px;max-width:1300px;margin-left:auto;margin-right:auto;padding:0 20px 60px}
        .hero{background:linear-gradient(135deg,#150A24,#2D1B4E);border-radius:var(--radius);padding:40px;text-align:center;margin-bottom:30px;border:1px solid var(--border)}
        .hero h1{font-size:2rem;margin-bottom:8px;background:linear-gradient(135deg,#C4B5FD,#FBBF24);-webkit-background-clip:text;-webkit-text-fill-color:transparent}
        .hero p{color:var(--muted);margin-bottom:16px;font-size:1rem}
        .stats-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:16px;margin-bottom:30px}
        .stat-card{background:var(--card);border:1px solid var(--border);border-radius:var(--radius);padding:20px;text-align:center;transition:all 0.3s}
        .stat-card:hover{border-color:var(--primary);transform:translateY(-3px)}
        .stat-icon{font-size:2rem;margin-bottom:6px}
        .stat-num{font-size:1.8rem;font-weight:900;background:linear-gradient(135deg,#A78BFA,#C4B5FD);-webkit-background-clip:text;-webkit-text-fill-color:transparent}
        .stat-label{color:var(--muted);font-size:0.82rem}

        .section{margin-bottom:40px}
        .section-header{display:flex;align-items:center;justify-content:space-between;margin-bottom:18px;flex-wrap:wrap;gap:10px}
        .section-title{font-size:1.3rem;font-weight:700;display:flex;align-items:center;gap:8px}
        .filters{display:flex;gap:8px;flex-wrap:wrap}
        .filter-btn{padding:7px 14px;border-radius:50px;border:1px solid var(--border);background:transparent;color:var(--muted);cursor:pointer;font-size:0.78rem;transition:all 0.3s;font-family:inherit}
        .filter-btn:hover,.filter-btn.active{border-color:var(--primary);color:var(--text);background:rgba(124,58,237,0.1)}

        .books-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(150px,1fr));gap:14px}
        .book-card{background:var(--card);border:1px solid var(--border);border-radius:var(--radius);overflow:hidden;cursor:pointer;transition:all 0.3s}
        .book-card:hover{border-color:var(--primary);transform:translateY(-5px);box-shadow:0 8px 30px rgba(0,0,0,0.4)}
        .book-cover{width:100%;aspect-ratio:3/4;overflow:hidden;background:#1E1035;position:relative}
        .book-cover img{width:100%;height:100%;object-fit:cover;transition:all 0.4s}
        .book-card:hover .book-cover img{transform:scale(1.07)}
        .book-badge{position:absolute;top:6px;right:6px;padding:3px 8px;border-radius:50px;font-size:0.6rem;font-weight:700;z-index:2}
        .badge-complete{background:#10B981;color:#fff}
        .badge-ongoing{background:#EF4444;color:#fff}
        .badge-popular{background:#8B5CF6;color:#fff}
        .book-info{padding:10px}
        .book-title{font-weight:700;font-size:0.82rem;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
        .book-meta{font-size:0.68rem;color:var(--muted);margin-top:3px;display:flex;gap:6px;align-items:center}
        .book-rating{color:var(--gold)}

        .trending-list{display:flex;flex-direction:column;gap:10px}
        .trending-item{display:flex;align-items:center;gap:12px;background:var(--card);border:1px solid var(--border);border-radius:var(--radius);padding:12px 16px;cursor:pointer;transition:all 0.3s}
        .trending-item:hover{border-color:var(--primary)}
        .trending-rank{font-size:1.5rem;font-weight:900;min-width:38px;text-align:center}
        .rank-1{color:#FFD700}.rank-2{color:#C0C0C0}.rank-3{color:#CD7F32}
        .trending-cover{width:45px;height:62px;border-radius:6px;overflow:hidden;flex-shrink:0}
        .trending-cover img{width:100%;height:100%;object-fit:cover}
        .trending-info{flex:1}
        .trending-title{font-weight:700;font-size:0.9rem}
        .trending-meta{font-size:0.7rem;color:var(--muted)}

        .modal-overlay{position:fixed;top:0;left:0;width:100%;height:100%;background:rgba(0,0,0,0.85);z-index:9999;display:flex;align-items:center;justify-content:center;opacity:0;visibility:hidden;transition:all 0.3s}
        .modal-overlay.active{opacity:1;visibility:visible}
        .modal{background:var(--card);border:1px solid var(--border);border-radius:var(--radius);padding:24px;max-width:500px;width:90%;max-height:80vh;overflow-y:auto;position:relative}
        .modal-close{position:absolute;top:10px;left:12px;background:none;border:none;color:var(--text);font-size:1.5rem;cursor:pointer}
        .modal-cover{width:120px;height:170px;border-radius:10px;margin:0 auto 14px;overflow:hidden}
        .modal-cover img{width:100%;height:100%;object-fit:cover}
        .modal h2{text-align:center;margin-bottom:6px;font-size:1.2rem}
        .modal-meta{display:flex;justify-content:center;gap:10px;margin:12px 0;flex-wrap:wrap}
        .modal-meta span{background:rgba(124,58,237,0.15);padding:5px 12px;border-radius:50px;font-size:0.78rem}
        .modal-desc{color:var(--muted);font-size:0.85rem;line-height:1.7;margin-bottom:14px}
        .modal-btn{display:block;width:100%;background:linear-gradient(135deg,#7C3AED,#A78BFA);color:white;border:none;padding:12px;border-radius:50px;font-weight:700;font-size:0.95rem;cursor:pointer;font-family:inherit}

        .footer{background:var(--card);border-top:1px solid var(--border);padding:30px 20px;text-align:center}
        .footer-links{display:flex;gap:18px;justify-content:center;flex-wrap:wrap;margin:14px 0}
        .footer-links a{color:var(--muted);text-decoration:none;font-size:0.82rem}
        .footer-text{color:var(--muted);font-size:0.78rem}

        .scroll-top{position:fixed;bottom:24px;left:24px;width:44px;height:44px;border-radius:50%;background:linear-gradient(135deg,#7C3AED,#A78BFA);color:white;border:none;cursor:pointer;font-size:1.2rem;z-index:998;opacity:0;visibility:hidden;transition:all 0.3s}
        .scroll-top.visible{opacity:1;visibility:visible}

        @media(max-width:768px){
            .hero h1{font-size:1.4rem}
            .stats-grid{grid-template-columns:repeat(2,1fr)}
            .books-grid{grid-template-columns:repeat(auto-fill,minmax(120px,1fr))}
            .main-content{margin-top:150px}
        }
    </style>
</head>
<body>

    <header class="header">
        <div class="header-inner">
            <a href="#" class="logo"><span class="logo-icon">⚡</span><span>كايدن</span></a>
            <div class="search-box">
                <input type="text" id="searchInput" placeholder="🔍 بحث عن أي عمل..." oninput="searchWorks()">
                <button class="btn btn-outline" onclick="showWriterPage()">✍️ انضم</button>
                <button class="btn btn-primary">👤 دخول</button>
            </div>
        </div>
        <nav class="nav-links">
            <a href="#" class="active" onclick="filterAll()">الكل</a>
            <a href="#" onclick="filterType('manhwa')">🌏 مانهاوا</a>
            <a href="#" onclick="filterType('manhua')">🀄 مانهوا</a>
            <a href="#" onclick="filterType('manga')">🎭 مانغا</a>
            <a href="#" onclick="filterType('novel')">📚 روايات</a>
            <a href="#" onclick="filterType('chinese')">🇨🇳 صيني</a>
            <a href="#" onclick="filterType('korean')">🇰🇷 كوري</a>
            <a href="#" onclick="filterType('japanese')">🇯🇵 ياباني</a>
        </nav>
    </header>

    <main class="main-content" id="mainPage">
        <div class="hero">
            <h1>⚡ كايدن - أكبر مكتبة للقصص المصورة المترجمة</h1>
            <p>أكثر من <strong>1000 عمل</strong> مترجم للعربية: مانهاوا كورية، مانهوا صينية، مانغا يابانية، وروايات ويب</p>
            <div style="display:flex;gap:10px;justify-content:center;flex-wrap:wrap;margin-top:12px">
                <span style="background:rgba(124,58,237,0.2);color:var(--neon);padding:6px 14px;border-radius:50px;font-size:0.8rem">🌏 +400 مانهاوا</span>
                <span style="background:rgba(124,58,237,0.2);color:var(--neon);padding:6px 14px;border-radius:50px;font-size:0.8rem">🀄 +300 مانهوا</span>
                <span style="background:rgba(124,58,237,0.2);color:var(--neon);padding:6px 14px;border-radius:50px;font-size:0.8rem">🎭 +200 مانغا</span>
                <span style="background:rgba(124,58,237,0.2);color:var(--neon);padding:6px 14px;border-radius:50px;font-size:0.8rem">📚 +150 رواية</span>
            </div>
        </div>

        <div class="stats-grid">
            <div class="stat-card"><div class="stat-icon">📚</div><div class="stat-num" id="totalCount">0</div><div class="stat-label">إجمالي الأعمال</div></div>
            <div class="stat-card"><div class="stat-icon">🌏</div><div class="stat-num" id="manhwaCount">0</div><div class="stat-label">مانهاوا</div></div>
            <div class="stat-card"><div class="stat-icon">🀄</div><div class="stat-num" id="manhuaCount">0</div><div class="stat-label">مانهوا</div></div>
            <div class="stat-card"><div class="stat-icon">🎭</div><div class="stat-num" id="mangaCount">0</div><div class="stat-label">مانغا</div></div>
        </div>

        <div class="section">
            <div class="section-header">
                <h2 class="section-title">🔥 جميع الأعمال</h2>
                <div class="filters">
                    <button class="filter-btn active" onclick="filterAll()">الكل</button>
                    <button class="filter-btn" onclick="filterStatus('complete')">✅ مكتملة</button>
                    <button class="filter-btn" onclick="filterStatus('ongoing')">🔄 مستمرة</button>
                    <button class="filter-btn" onclick="sortWorks('rating')">⭐ الأعلى تقييماً</button>
                    <button class="filter-btn" onclick="sortWorks('newest')">🆕 الأحدث</button>
                </div>
            </div>
            <div class="books-grid" id="worksGrid"></div>
            <div style="text-align:center;margin-top:20px">
                <button class="btn btn-outline" onclick="loadMore()">تحميل المزيد ↓</button>
            </div>
        </div>

        <div class="section">
            <div class="section-header"><h2 class="section-title">📈 الأكثر رواجاً</h2></div>
            <div class="trending-list" id="trendingGrid"></div>
        </div>
    </main>

    <!-- صفحة الكاتب -->
    <main class="main-content" id="writerPage" style="display:none">
        <button class="btn btn-outline" onclick="showMainPage()" style="margin-bottom:20px">← العودة</button>
        <div class="hero"><h2>✍️ انضم إلى أسرة كايدن</h2><p>أضف أعمالك المترجمة وشاركها مع آلاف القراء</p></div>
        <div style="background:var(--card);border:1px solid var(--border);border-radius:var(--radius);padding:24px;max-width:650px;margin:0 auto">
            <div style="margin-bottom:12px"><label style="display:block;margin-bottom:4px;font-weight:600">اسمك</label><input type="text" id="wName" style="width:100%;padding:10px;border-radius:8px;border:2px solid var(--border);background:rgba(255,255,255,0.04);color:var(--text);font-family:inherit;outline:none" placeholder="اسمك أو فريقك"></div>
            <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:12px">
                <div><label style="display:block;margin-bottom:4px;font-weight:600">نوع العمل</label><select id="wType" style="width:100%;padding:10px;border-radius:8px;border:2px solid var(--border);background:rgba(255,255,255,0.04);color:var(--text);font-family:inherit"><option>🌏 مانهاوا</option><option>🀄 مانهوا</option><option>🎭 مانغا</option><option>📚 رواية</option></select></div>
                <div><label style="display:block;margin-bottom:4px;font-weight:600">التصنيف</label><select id="wGenre" style="width:100%;padding:10px;border-radius:8px;border:2px solid var(--border);background:rgba(255,255,255,0.04);color:var(--text);font-family:inherit"><option>أكشن</option><option>رومانسي</option><option>إيسيكاي</option><option>فانتازيا</option><option>رعب</option><option>كوميدي</option></select></div>
            </div>
            <div style="margin-bottom:12px"><label style="display:block;margin-bottom:4px;font-weight:600">اسم العمل</label><input type="text" id="wTitle" style="width:100%;padding:10px;border-radius:8px;border:2px solid var(--border);background:rgba(255,255,255,0.04);color:var(--text);font-family:inherit;outline:none" placeholder="اسم الرواية أو المانغا"></div>
            <div style="margin-bottom:12px"><label style="display:block;margin-bottom:4px;font-weight:600">رابط الصورة</label><input type="text" id="wImage" style="width:100%;padding:10px;border-radius:8px;border:2px solid var(--border);background:rgba(255,255,255,0.04);color:var(--text);font-family:inherit;outline:none" placeholder="رابط صورة الغلاف"></div>
            <div style="display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:12px">
                <div><label style="display:block;margin-bottom:4px;font-weight:600">عدد الفصول</label><input type="text" id="wChapters" style="width:100%;padding:10px;border-radius:8px;border:2px solid var(--border);background:rgba(255,255,255,0.04);color:var(--text);font-family:inherit;outline:none" placeholder="مثلاً: 150"></div>
                <div><label style="display:block;margin-bottom:4px;font-weight:600">الحالة</label><select id="wStatus" style="width:100%;padding:10px;border-radius:8px;border:2px solid var(--border);background:rgba(255,255,255,0.04);color:var(--text);font-family:inherit"><option value="ongoing">مستمر</option><option value="complete">مكتمل</option></select></div>
            </div>
            <div style="margin-bottom:12px"><label style="display:block;margin-bottom:4px;font-weight:600">الوصف</label><textarea id="wDesc" style="width:100%;padding:10px;border-radius:8px;border:2px solid var(--border);background:rgba(255,255,255,0.04);color:var(--text);font-family:inherit;outline:none;min-height:80px;resize:vertical" placeholder="وصف القصة..."></textarea></div>
            <button class="btn btn-primary" style="width:100%" onclick="addWork()">🚀 أضف العمل الآن</button>
            <div id="successMsg" style="display:none;text-align:center;padding:12px;background:rgba(16,185,129,0.1);border:1px solid #10B981;border-radius:8px;color:#10B981;margin-top:12px">✅ تمت الإضافة بنجاح!</div>
        </div>
        <div style="margin-top:24px"><h3 style="color:var(--neon);margin-bottom:10px">📋 أعمالك المضافة</h3><div class="books-grid" id="userWorksGrid"></div></div>
    </main>

    <footer class="footer">
        <div class="footer-links"><a href="#">عن كايدن</a><a href="#">اتصل بنا</a><a href="#">سياسة الخصوصية</a><a href="#" onclick="showWriterPage()">انضم ككاتب</a></div>
        <p class="footer-text">© 2025 كايدن - Kaiden. جميع الحقوق محفوظة</p>
    </footer>

    <div class="modal-overlay" id="modal"><div class="modal" id="modalContent"></div></div>
    <button class="scroll-top" id="scrollTop">↑</button>

    <script>
        // ========== توليد 1000+ عمل تلقائياً ==========
        const titles = {
            manhwa: ['Solo Leveling','The Beginning After The End','Tower of God','Noblesse','Sweet Home','Omniscient Reader\'s Viewpoint','The World After the Fall','Eleceed','Wind Breaker','Mercenary Enrollment','Lookism','Viral Hit','Manager Kim','Quest Supremacy','Reality Quest','Nano Machine','Doom Breaker','SSS-Class Revival Hunter','The Greatest Estate Developer','Damn Reincarnation','Northern Blade','Chronicles of Heavenly Demon','Volcanic Age','Murim Login','Worn and Torn Newbie','The Returner\'s Magic','Second Life Ranker','Talent-Swallowing Magician','Survival Story of a Sword King','Knight King Who Returned','Player That Can\'t Level Up','Return of Mount Hua Sect','Legend of Northern Blade','Skeleton Soldier','Kill the Hero','Overgeared','Ranker Who Lives Twice','Wizard of Arsenia','Dark Magician Transmigrates','Duke Pendragon','Trash of Count\'s Family','Solo Max-Level Newbie','I\'m Not That Kind of Talent','Book Eating Magician','FFF-Class Trash Hero','Warrior Returns','Hero Has Returned','Survival of a Sword King','I Grow Stronger by Eating'],
            manhua: ['Battle Through the Heavens','Apotheosis','Yuan Zun','Star Martial God','Dragon Prince Yuan','Spirit Blade Mountain','Soul Land','Soul Land 2','Soul Land 3','The Great Ruler','Versatile Mage','Tales of Demons and Gods','God of Martial Arts','Peerless Battle Spirit','Rebirth of Urban Immortal','Spare Me Great Lord','Martial Peak','The Invincible','Magic Emperor','Demonic Emperor','I\'m an Evil God','Release That Witch','Douluo Dalu','Battle Frenzy','Master of Gu','Reverend Insanity','I Shall Be Sealed','A Will Eternal','Renegade Immortal','Swallowed Star','Lord Xue Ying','Seeking the Flying Sword Path','Desolate Era','Coiling Dragon','Stellar Transformations','I Eat Tomatoes Collection','Ancient Godly Monarch','Against the Gods','Martial God Asura','Emperor\'s Domination'],
            manga: ['One Piece','Naruto','Bleach','Attack on Titan','Demon Slayer','Jujutsu Kaisen','My Hero Academia','Black Clover','Dragon Ball Super','Hunter x Hunter','One Punch Man','Tokyo Revengers','Chainsaw Man','Spy x Family','Frieren','Berserk','Vagabond','Vinland Saga','Kingdom','Haikyuu!!','Blue Lock','Death Note','Fullmetal Alchemist','Monster','20th Century Boys','Goodnight Punpun','Oyasumi Punpun','Slam Dunk','Rurouni Kenshin','Gintama','Fairy Tail','Edens Zero','Rave Master','Toriko','Assassination Classroom','Mob Psycho 100','Made in Abyss','Promised Neverland','Dr. Stone','Kaguya-sama','Komi Can\'t Communicate'],
            novel: ['I Shall Seal the Heavens','A Will Eternal','Renegade Immortal','Coiling Dragon','Stellar Transformations','Desolate Era','Swallowed Star','Martial World','Against the Gods','Tales of Demons and Gods','The Great Ruler','Battle Through the Heavens (Novel)','Warlock of Magus World','Reverend Insanity','Lord of Mysteries','Shadow Slave','Mother of Learning','Mushoku Tensei','Re:Zero','Overlord','Tensura','Classroom of the Elite','DanMachi','Shield Hero','Sword Art Online','Eminence in Shadow','Second Coming of Gluttony','Omniscient Reader (Novel)','Trash of Count\'s Family (Novel)','SSS-Class Revival Hunter (Novel)']
        };

        const authors = ['Chugong','TurtleMe','SIU','Son Jeho','Kim Carnby','Sing Shong','Yongje Park','Jo Yong-seok','Taejun Pak','Youn In-wan','Heavenly Silkworm Potato','Mad Snail','Tang Jia San Shao','I Eat Tomatoes','Er Gen','Cocooned Cow','Eiichiro Oda','Masashi Kishimoto','Tite Kubo','Hajime Isayama','Gege Akutami','ONE','Tatsuki Fujimoto','Rifujin na Magonote','Tappei Nagatsuki','Kugane Maruyama','Fuse','Reki Kawahara'];

        const genres = ['أكشن','رومانسي','إيسيكاي','فانتازيا','رعب','كوميدي','قتالي','مدرسي','سحر','خارق للطبيعة','دراما','غموض','نفسي','زراعة','فنون قتالية','مغامرة'];

        const images = [
            'https://cdn.myanimelist.net/images/manga/3/218973l.jpg',
            'https://cdn.myanimelist.net/images/manga/2/246489l.jpg',
            'https://cdn.myanimelist.net/images/manga/1/164565l.jpg',
            'https://cdn.myanimelist.net/images/manga/1/230962l.jpg',
            'https://cdn.myanimelist.net/images/manga/2/179432l.jpg',
            'https://cdn.myanimelist.net/images/manga/1/247901l.jpg',
            'https://cdn.myanimelist.net/images/manga/2/273456l.jpg',
            'https://cdn.myanimelist.net/images/manga/1/278912l.jpg',
            'https://cdn.myanimelist.net/images/manga/1/249876l.jpg',
            'https://cdn.myanimelist.net/images/manga/2/188888l.jpg',
            'https://cdn.myanimelist.net/images/manga/1/188990l.jpg',
            'https://cdn.myanimelist.net/images/manga/2/253146l.jpg',
            'https://cdn.myanimelist.net/images/manga/3/249658l.jpg',
            'https://cdn.myanimelist.net/images/manga/2/37846l.jpg',
            'https://cdn.myanimelist.net/images/manga/3/202577l.jpg',
            'https://cdn.myanimelist.net/images/manga/3/219741l.jpg',
            'https://cdn.myanimelist.net/images/manga/1/121153l.jpg',
            'https://cdn.myanimelist.net/images/manga/1/184521l.jpg',
            'https://cdn.myanimelist.net/images/manga/2/156355l.jpg',
            'https://cdn.myanimelist.net/images/manga/1/181655l.jpg'
        ];

        function rand(arr) { return arr[Math.floor(Math.random() * arr.length)]; }
        function randInt(min, max) { return Math.floor(Math.random() * (max - min + 1)) + min; }

        // توليد 1000+ عمل
        let allWorks = [];
        let workId = 0;
        const types = ['manhwa','manhua','manga','novel'];
        const typeConfig = { manhwa: { count: 400, origin: 'korean', flag: '🌏', label: 'مانهاوا' }, manhua: { count: 300, origin: 'chinese', flag: '🀄', label: 'مانهوا' }, manga: { count: 200, origin: 'japanese', flag: '🎭', label: 'مانغا' }, novel: { count: 150, origin: 'chinese', flag: '📚', label: 'رواية' } };

        function generateWork(type) {
            const config = typeConfig[type];
            const titleList = titles[type];
            const title = titleList[workId % titleList.length] + (workId >= titleList.length ? ' ' + (Math.floor(workId / titleList.length) + 2) : '');
            workId++;
            return {
                id: 'w_' + workId,
                title: title,
                author: rand(authors),
                type: type,
                origin: config.origin,
                flag: config.flag,
                label: config.label,
                image: rand(images),
                chapters: randInt(50, 800),
                status: Math.random() > 0.4 ? 'ongoing' : 'complete',
                rating: (Math.random() * 2 + 3).toFixed(1),
                genre: rand(genres),
                desc: 'قصة شيقة مترجمة للعربية بالكامل. ' + title + ' من أشهر الأعمال في مجال ' + config.label + '. تحديثات مستمرة وجودة عالية.'
            };
        }

        for (const type of types) {
            for (let i = 0; i < typeConfig[type].count; i++) {
                allWorks.push(generateWork(type));
            }
        }

        // عرض 20 عمل في البداية
        let displayCount = 20;
        let currentFilter = 'all';
        let currentStatus = 'all';
        let currentSort = 'default';
        let filteredWorks = [...allWorks];

        function getFilteredWorks() {
            let works = [...allWorks];
            if (currentFilter !== 'all') {
                if (['chinese','korean','japanese'].includes(currentFilter)) {
                    works = works.filter(w => w.origin === currentFilter);
                } else {
                    works = works.filter(w => w.type === currentFilter);
                }
            }
            if (currentStatus !== 'all') {
                works = works.filter(w => w.status === currentStatus);
            }
            if (currentSort === 'rating') {
                works.sort((a, b) => parseFloat(b.rating) - parseFloat(a.rating));
            } else if (currentSort === 'newest') {
                works.reverse();
            }
            return works;
        }

        function renderWorks() {
            filteredWorks = getFilteredWorks();
            const container = document.getElementById('worksGrid');
            const toShow = filteredWorks.slice(0, displayCount);
            container.innerHTML = toShow.map(w => `
                <div class="book-card" onclick="openModal('${w.id}')">
                    <div class="book-cover">
                        <img src="${w.image}" alt="${w.title}" loading="lazy" onerror="this.style.display='none';this.parentElement.style.background='linear-gradient(135deg,#4C1D95,#7C3AED)';">
                        <span class="book-badge ${w.status==='complete'?'badge-complete':'badge-ongoing'}">${w.status==='complete'?'مكتملة':'مستمرة'}</span>
                    </div>
                    <div class="book-info">
                        <div class="book-title">${w.flag} ${w.title}</div>
                        <div class="book-meta"><span class="book-rating">⭐${w.rating}</span> · ${w.chapters} فصل</div>
                        <div class="book-meta">${w.genre} · ${w.label}</div>
                    </div>
                </div>
            `).join('');
            document.getElementById('totalCount').textContent = allWorks.length;
            document.getElementById('manhwaCount').textContent = allWorks.filter(w=>w.type==='manhwa').length;
            document.getElementById('manhuaCount').textContent = allWorks.filter(w=>w.type==='manhua').length;
            document.getElementById('mangaCount').textContent = allWorks.filter(w=>w.type==='manga').length;
        }

        function loadMore() {
            displayCount += 20;
            if (displayCount > filteredWorks.length) displayCount = filteredWorks.length;
            renderWorks();
        }

        function searchWorks() {
            const query = document.getElementById('searchInput').value.toLowerCase().trim();
            if (query === '') {
                filteredWorks = getFilteredWorks();
                displayCount = 20;
                renderWorks();
                return;
            }
            filteredWorks = allWorks.filter(w => w.title.toLowerCase().includes(query) || w.author.toLowerCase().includes(query) || w.genre.includes(query));
            displayCount = 20;
            const container = document.getElementById('worksGrid');
            container.innerHTML = filteredWorks.slice(0, displayCount).map(w => `
                <div class="book-card" onclick="openModal('${w.id}')">
                    <div class="book-cover">
                        <img src="${w.image}" alt="${w.title}" loading="lazy" onerror="this.style.display='none';this.parentElement.style.background='linear-gradient(135deg,#4C1D95,#7C3AED)';">
                        <span class="book-badge ${w.status==='complete'?'badge-complete':'badge-ongoing'}">${w.status==='complete'?'مكتملة':'مستمرة'}</span>
                    </div>
                    <div class="book-info">
                        <div class="book-title">${w.flag} ${w.title}</div>
                        <div class="book-meta"><span class="book-rating">⭐${w.rating}</span> · ${w.chapters} فصل</div>
                        <div class="book-meta">${w.genre} · ${w.label}</div>
                    </div>
                </div>
            `).join('');
        }

        function filterType(type) {
            currentFilter = type;
            currentStatus = 'all';
            currentSort = 'default';
            displayCount = 20;
            filteredWorks = getFilteredWorks();
            renderWorks();
            document.querySelectorAll('.nav-links a').forEach(a => a.classList.remove('active'));
            document.querySelectorAll('.filter-btn').forEach(b => b.classList.remove('active'));
        }
        function filterAll() {
            currentFilter = 'all';
            currentStatus = 'all';
            currentSort = 'default';
            displayCount = 20;
            filteredWorks = allWorks;
            renderWorks();
            document.querySelectorAll('.nav-links a').forEach(a => a.classList.remove('active'));
            document.querySelector('.nav-links a[href="#"]').classList.add('active');
        }
        function filterStatus(status) {
            currentStatus = status;
            displayCount = 20;
            filteredWorks = getFilteredWorks();
            renderWorks();
        }
        function sortWorks(sort) {
            currentSort = sort;
            displayCount = 20;
            filteredWorks = getFilteredWorks();
            renderWorks();
        }

        function renderTrending() {
            const trending = allWorks.filter(w => parseFloat(w.rating) >= 4.5).sort((a,b) => parseFloat(b.rating) - parseFloat(a.rating)).slice(0, 5);
            const container = document.getElementById('trendingGrid');
            const ranks = ['rank-1','rank-2','rank-3','',''];
            container.innerHTML = trending.map((w,i) => `
                <div class="trending-item" onclick="openModal('${w.id}')">
                    <span class="trending-rank ${ranks[i]}">#${i+1}</span>
                    <div class="trending-cover"><img src="${w.image}" alt="${w.title}" loading="lazy"></div>
                    <div class="trending-info">
                        <div class="trending-title">${w.flag} ${w.title}</div>
                        <div class="trending-meta">⭐${w.rating} · ${w.chapters} فصل · ${w.genre} · ${w.label}</div>
                    </div>
                    <button class="btn btn-primary" style="padding:7px 14px;font-size:0.72rem">اقرأ 💜</button>
                </div>
            `).join('');
        }

        function openModal(id) {
            const w = allWorks.find(x => x.id === id);
            if (!w) return;
            const overlay = document.getElementById('modal');
            const content = document.getElementById('modalContent');
            content.innerHTML = `
                <button class="modal-close" onclick="closeModal()">✕</button>
                <div class="modal-cover"><img src="${w.image}" alt="${w.title}" onerror="this.style.display='none';this.parentElement.style.background='linear-gradient(135deg,#4C1D95,#7C3AED)';"></div>
                <span class="book-badge ${w.status==='complete'?'badge-complete':'badge-ongoing'}" style="display:inline-block;margin:0 auto 8px;position:static;">${w.status==='complete'?'مكتملة':'مستمرة'}</span>
                <h2>${w.flag} ${w.title}</h2>
                <p style="text-align:center;color:var(--muted);font-size:0.85rem">✍️ ${w.author}</p>
                <div class="modal-meta"><span>⭐${w.rating}</span><span>📖 ${w.chapters} فصل</span><span>📂 ${w.genre}</span><span>${w.label}</span></div>
                <p class="modal-desc">${w.desc}</p>
                <p style="background:rgba(124,58,237,0.1);padding:8px;border-radius:8px;font-size:0.78rem;color:var(--neon);text-align:center;margin-bottom:12px">✅ مترجمة للعربية</p>
                <button class="modal-btn" onclick="closeModal()">📖 ابدأ القراءة الآن 💜</button>
            `;
            overlay.classList.add('active');
            document.body.style.overflow = 'hidden';
        }
        function closeModal() { document.getElementById('modal').classList.remove('active'); document.body.style.overflow = ''; }
        document.getElementById('modal').addEventListener('click', function(e) { if (e.target === this) closeModal(); });

        // صفحات
        function showWriterPage() { document.getElementById('mainPage').style.display='none'; document.getElementById('writerPage').style.display='block'; window.scrollTo({top:0,behavior:'smooth'}); }
        function showMainPage() { document.getElementById('writerPage').style.display='none'; document.getElementById('mainPage').style.display='block'; window.scrollTo({top:0,behavior:'smooth'}); }

        let userWorks = [];
        function addWork() {
            const name = document.getElementById('wName').value.trim();
            const type = document.getElementById('wType').value;
            const genre = document.getElementById('wGenre').value;
            const title = document.getElementById('wTitle').value.trim();
            const image = document.getElementById('wImage').value.trim();
            const chapters = document.getElementById('wChapters').value.trim();
            const status = document.getElementById('wStatus').value;
            const desc = document.getElementById('wDesc').value.trim();
            if (!name || !title || !desc) { alert('املأ الحقول المطلوبة'); return; }
            const w = { id:'u_'+Date.now(), title, author:name, type:type.includes('مانهاوا')?'manhwa':type.includes('مانهوا')?'manhua':type.includes('مانغا')?'manga':'novel', flag:'👤', label:type, image:image||'https://images.unsplash.com/photo-1543002588-bfa74002ed7e?w=400', chapters:parseInt(chapters)||0, status, rating:'5.0', genre, desc };
            userWorks.unshift(w);
            allWorks.unshift(w);
            document.getElementById('successMsg').style.display='block';
            setTimeout(()=>document.getElementById('successMsg').style.display='none',3000);
            ['wName','wTitle','wImage','wChapters','wDesc'].forEach(id=>document.getElementById(id).value='');
            renderUserWorks();
            renderWorks();
            renderTrending();
        }
        function renderUserWorks() {
            const grid = document.getElementById('userWorksGrid');
            grid.innerHTML = userWorks.map(w => `
                <div class="book-card" onclick="openModal('${w.id}')">
                    <div class="book-cover"><img src="${w.image}" alt="${w.title}" onerror="this.style.display='none';this.parentElement.style.background='linear-gradient(135deg,#4C1D95,#7C3AED)';"><span class="book-badge badge-popular">${w.status==='complete'?'مكتمل':'مستمر'}</span></div>
                    <div class="book-info"><div class="book-title">👤 ${w.title}</div><div class="book-meta">⭐${w.rating} · ${w.chapters} فصل</div><div class="book-meta">${w.genre} · ${w.label}</div></div>
                </div>
            `).join('');
        }

        // سكرول
        window.addEventListener('scroll', () => {
            const btn = document.getElementById('scrollTop');
            if (window.scrollY > 500) btn.classList.add('visible'); else btn.classList.remove('visible');
        });
        document.getElementById('scrollTop').addEventListener('click', () => { window.scrollTo({top:0,behavior:'smooth'}); });

        // بدء
        renderWorks();
        renderTrending();
    </script>
</body>
</html>            align-items: center;
            justify-content: center;
            z-index: 9999;
            transition: opacity 0.5s, visibility 0.5s;
        }
        .loader.hidden {
            opacity: 0;
            visibility: hidden;
        }
        .loader-content {
            text-align: center;
        }
        .loader-book {
            font-size: 60px;
            animation: float 2s ease-in-out infinite;
        }
        .loader-logo {
            font-size: 2rem;
            font-weight: 900;
            background: var(--gradient-1);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-top: 10px;
        }
        .loader-bar {
            width: 200px;
            height: 4px;
            background: var(--border);
            border-radius: 4px;
            margin: 20px auto;
            overflow: hidden;
        }
        .loader-bar-fill {
            height: 100%;
            background: var(--gradient-1);
            border-radius: 4px;
            animation: loadBar 1.5s ease-in-out infinite;
        }
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
        }
        @keyframes loadBar {
            0% { width: 0; transform: translateX(0); }
            50% { width: 100%; transform: translateX(0); }
            100% { width: 0; transform: translateX(200px); }
        }

        /* ===== خلفية النجوم ===== */
        .stars-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 0;
        }
        .star {
            position: absolute;
            background: white;
            border-radius: 50%;
            animation: twinkle var(--duration) ease-in-out infinite;
            opacity: 0;
        }
        @keyframes twinkle {
            0%, 100% { opacity: 0.2; transform: scale(1); }
            50% { opacity: 0.8; transform: scale(1.5); }
        }

        /* ===== إعلان الشريط العلوي ===== */
        .top-ad-bar {
            background: var(--ad-bg);
            border-bottom: 1px solid var(--ad-border);
            text-align: center;
            padding: 8px;
            position: relative;
            z-index: 1001;
            color: var(--text-muted);
            font-size: 0.8rem;
        }
        .top-ad-bar .ad-content {
            background: var(--bg-card);
            border: 1px dashed var(--ad-border);
            border-radius: 8px;
            padding: 6px 20px;
            display: inline-block;
            max-width: 728px;
            width: 100%;
        }

        /* ===== الهيدر ===== */
        .header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            background: var(--glass-bg);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            border-bottom: 1px solid var(--border);
            transition: var(--transition);
        }
        .header.scrolled {
            box-shadow: 0 4px 30px rgba(123, 47, 190, 0.2);
        }
        .header-inner {
            max-width: 1300px;
            margin: 0 auto;
            padding: 12px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            gap: 20px;
        }
        .logo {
            display: flex;
            align-items: center;
            gap: 8px;
            text-decoration: none;
            color: var(--text);
            font-size: 1.8rem;
            font-weight: 900;
            white-space: nowrap;
        }
        .logo-icon {
            font-size: 2rem;
            animation: float 3s ease-in-out infinite;
        }
        .logo-gradient {
            background: var(--gradient-1);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        .search-container {
            flex: 1;
            max-width: 400px;
            position: relative;
        }
        .search-input {
            width: 100%;
            padding: 12px 45px 12px 20px;
            border-radius: 50px;
            border: 2px solid var(--border);
            background: rgba(255, 255, 255, 0.05);
            color: var(--text);
            font-size: 0.95rem;
            transition: var(--transition);
            outline: none;
            font-family: inherit;
        }
        .search-input:focus {
            border-color: var(--primary-light);
            box-shadow: var(--shadow-neon);
            background: rgba(255, 255, 255, 0.08);
        }
        .search-input::placeholder { color: var(--text-muted); }
        .search-btn {
            position: absolute;
            left: 8px;
            top: 50%;
            transform: translateY(-50%);
            background: var(--gradient-1);
            border: none;
            color: white;
            width: 35px;
            height: 35px;
            border-radius: 50%;
            cursor: pointer;
            font-size: 1rem;
            transition: var(--transition);
        }
        .search-btn:hover { box-shadow: var(--shadow-neon); transform: translateY(-50%) scale(1.05); }
        .user-btn {
            background: var(--gradient-1);
            border: none;
            color: white;
            padding: 10px 24px;
            border-radius: 50px;
            cursor: pointer;
            font-weight: 600;
            font-size: 0.9rem;
            transition: var(--transition);
            white-space: nowrap;
            font-family: inherit;
        }
        .user-btn:hover { box-shadow: var(--shadow-neon); transform: translateY(-2px); }
        .nav-links {
            display: flex;
            gap: 5px;
            flex-wrap: wrap;
            justify-content: center;
        }
        .nav-links a {
            color: var(--text-muted);
            text-decoration: none;
            padding: 8px 16px;
            border-radius: 50px;
            transition: var(--transition);
            font-size: 0.9rem;
            font-weight: 500;
        }
        .nav-links a:hover,
        .nav-links a.active {
            color: var(--text);
            background: rgba(168, 85, 247, 0.15);
        }
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            color: var(--text);
            font-size: 1.8rem;
            cursor: pointer;
        }

        /* ===== المحتوى الرئيسي ===== */
        .main-content {
            position: relative;
            z-index: 1;
            margin-top: 165px;
            max-width: 1300px;
            margin-left: auto;
            margin-right: auto;
            padding: 0 20px 60px;
        }

        /* ===== الإعلانات ===== */
        .ad-banner {
            background: var(--ad-bg);
            border: 1px dashed var(--ad-border);
            border-radius: var(--radius);
            padding: 20px;
            text-align: center;
            margin-bottom: 30px;
            color: var(--text-muted);
            font-size: 0.85rem;
            min-height: 90px;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: var(--transition);
        }
        .ad-banner:hover {
            border-color: var(--primary-light);
            background: rgba(168, 85, 247, 0.03);
        }
        .ad-label {
            display: inline-block;
            background: rgba(168, 85, 247, 0.15);
            color: var(--neon);
            padding: 3px 10px;
            border-radius: 4px;
            font-size: 0.7rem;
            margin-bottom: 8px;
            letter-spacing: 1px;
        }
        .ad-banner-large {
            min-height: 250px;
        }
        .ad-sidebar {
            position: fixed;
            top: 180px;
            width: 160px;
            min-height: 600px;
            background: var(--ad-bg);
            border: 1px dashed var(--ad-border);
            border-radius: var(--radius);
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--text-muted);
            font-size: 0.8rem;
            text-align: center;
            padding: 20px;
            z-index: 2;
            transition: var(--transition);
        }
        .ad-sidebar.left { left: 10px; }
        .ad-sidebar.right { right: 10px; }
        .ad-sidebar:hover { border-color: var(--primary-light); }

        /* ===== الهيرو ===== */
        .hero {
            position: relative;
            border-radius: var(--radius);
            overflow: hidden;
            margin-bottom: 30px;
            height: 380px;
            display: flex;
            align-items: center;
            background: var(--gradient-2);
        }
        .hero-slider {
            display: flex;
            width: 400%;
            height: 100%;
            transition: transform 0.6s ease;
        }
        .hero-slide {
            width: 25%;
            height: 100%;
            display: flex;
            align-items: center;
            padding: 40px 50px;
            position: relative;
            flex-shrink: 0;
        }
        .hero-slide:nth-child(1) { background: linear-gradient(135deg, #1A0A2E 0%, #3B1F6E 100%); }
        .hero-slide:nth-child(2) { background: linear-gradient(135deg, #1A0A2E 0%, #5B2D8E 100%); }
        .hero-slide:nth-child(3) { background: linear-gradient(135deg, #1A0A2E 0%, #2D1B5E 100%); }
        .hero-slide:nth-child(4) { background: linear-gradient(135deg, #1A0A2E 0%, #4A2578 100%); }
        .hero-content { max-width: 500px; }
        .hero-badge {
            display: inline-block;
            background: rgba(168, 85, 247, 0.2);
            color: var(--neon);
            padding: 6px 16px;
            border-radius: 50px;
            font-size: 0.85rem;
            margin-bottom: 16px;
            font-weight: 600;
        }
        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 12px;
            line-height: 1.3;
        }
        .hero p {
            color: var(--text-muted);
            margin-bottom: 24px;
            font-size: 1.1rem;
        }
        .hero-btn {
            display: inline-block;
            background: var(--gradient-1);
            color: white;
            padding: 14px 32px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 700;
            font-size: 1rem;
            transition: var(--transition);
            border: none;
            cursor: pointer;
        }
        .hero-btn:hover { box-shadow: var(--shadow-neon); transform: translateY(-2px); }
        .hero-dots {
            position: absolute;
            bottom: 20px;
            left: 50%;
            transform: translateX(-50%);
            display: flex;
            gap: 10px;
            z-index: 2;
        }
        .hero-dot {
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.3);
            cursor: pointer;
            transition: var(--transition);
            border: none;
        }
        .hero-dot.active { background: var(--neon); box-shadow: 0 0 10px var(--neon); }

        /* ===== وصف الموقع ===== */
        .site-description {
            text-align: center;
            margin-bottom: 40px;
            padding: 30px;
            background: var(--bg-card);
            border: 1px solid var(--border);
            border-radius: var(--radius);
        }
        .site-description h2 {
            font-size: 1.4rem;
            background: var(--gradient-1);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 10px;
        }
        .site-description p {
            color: var(--text-muted);
            max-width: 800px;
            margin: 0 auto;
            font-size: 1rem;
            line-height: 1.8;
        }
        .site-tags {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
            justify-content: center;
            margin-top: 16px;
        }
        .site-tag {
            background: rgba(168, 85, 247, 0.1);
            color: var(--neon);
            padding: 6px 16px;
            border-radius: 50px;
            font-size: 0.85rem;
            border: 1px solid var(--ad-border);
        }

        /* ===== الإحصائيات ===== */
        .stats-bar {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 20px;
            margin-bottom: 30px;
        }
        .stat-card {
            background: var(--bg-card);
            border: 1px solid var(--border);
            border-radius: var(--radius);
            padding: 24px;
            text-align: center;
            transition: var(--transition);
        }
        .stat-card:hover { border-color: var(--primary-light); box-shadow: var(--shadow-neon); transform: translateY(-4px); }
        .stat-icon { font-size: 2.2rem; margin-bottom: 8px; }
        .stat-number {
            font-size: 2rem;
            font-weight: 800;
            background: var(--gradient-1);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        .stat-label { color: var(--text-muted); font-size: 0.9rem; }

        /* ===== الأقسام ===== */
        .section { margin-bottom: 45px; }
        .section-header {
            display: flex;
            align-items: center;
            justify-content: space-between;
            margin-bottom: 20px;
        }
        .section-title {
            font-size: 1.5rem;
            font-weight: 700;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        .section-title-icon { font-size: 1.6rem; }
        .section-link {
            color: var(--primary-light);
            text-decoration: none;
            font-weight: 600;
            font-size: 0.9rem;
            transition: var(--transition);
        }
        .section-link:hover { color: var(--neon); }

        /* ===== كروت الكتب ===== */
        .books-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
            gap: 20px;
        }
        .book-card {
            background: var(--bg-card);
            border: 1px solid var(--border);
            border-radius: var(--radius);
            overflow: hidden;
            transition: var(--transition);
            cursor: pointer;
            position: relative;
        }
        .book-card:hover {
            border-color: var(--primary-light);
            box-shadow: var(--shadow-card);
            transform: translateY(-6px);
        }
        .book-cover {
            width: 100%;
            aspect-ratio: 3/4;
            background: var(--gradient-2);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 3.5rem;
            position: relative;
            overflow: hidden;
        }
        .book-cover.cover-1 { background: linear-gradient(135deg, #4C1D95, #7C3AED); }
        .book-cover.cover-2 { background: linear-gradient(135deg, #5B21B6, #8B5CF6); }
        .book-cover.cover-3 { background: linear-gradient(135deg, #3B0764, #6D28D9); }
        .book-cover.cover-4 { background: linear-gradient(135deg, #2E1065, #7E22CE); }
        .book-cover.cover-5 { background: linear-gradient(135deg, #4A1D96, #9333EA); }
        .book-cover.cover-6 { background: linear-gradient(135deg, #1E0B4A, #5B21B6); }
        .book-cover.cover-7 { background: linear-gradient(135deg, #312E81, #6366F1); }
        .book-cover.cover-8 { background: linear-gradient(135deg, #3730A3, #818CF8); }
        .book-badge {
            position: absolute;
            top: 10px;
            right: 10px;
            padding: 4px 10px;
            border-radius: 50px;
            font-size: 0.7rem;
            font-weight: 700;
            z-index: 2;
        }
        .badge-new { background: #F59E0B; color: #1A0A2E; }
        .badge-complete { background: #10B981; color: white; }
        .badge-hot { background: #EF4444; color: white; }
        .badge-featured { background: #8B5CF6; color: white; }
        .book-info { padding: 14px; }
        .book-title {
            font-weight: 700;
            font-size: 0.95rem;
            margin-bottom: 4px;
            white-space: nowrap;
            overflow: hidden;
            text-overflow: ellipsis;
        }
        .book-author {
            font-size: 0.75rem;
            color: var(--text-muted);
            margin-bottom: 4px;
            white-space: nowrap;
            overflow: hidden;
            text-overflow: ellipsis;
        }
        .book-meta {
            display: flex;
            align-items: center;
            gap: 8px;
            font-size: 0.78rem;
            color: var(--text-muted);
        }
        .book-rating { color: var(--gold); font-weight: 600; }
        .book-chapters { color: var(--neon); }

        /* ===== تصنيفات ===== */
        .categories-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(140px, 1fr));
            gap: 16px;
        }
        .category-card {
            background: var(--bg-card);
            border: 1px solid var(--border);
            border-radius: var(--radius);
            padding: 22px 16px;
            text-align: center;
            cursor: pointer;
            transition: var(--transition);
            text-decoration: none;
            color: var(--text);
        }
        .category-card:hover {
            border-color: var(--primary-light);
            box-shadow: var(--shadow-neon);
            transform: translateY(-4px);
        }
        .category-icon { font-size: 2.5rem; margin-bottom: 10px; }
        .category-name { font-weight: 700; font-size: 0.95rem; }

        /* ===== الأكثر قراءة ===== */
        .trending-list { display: flex; flex-direction: column; gap: 14px; }
        .trending-item {
            display: flex;
            align-items: center;
            gap: 16px;
            background: var(--bg-card);
            border: 1px solid var(--border);
            border-radius: var(--radius);
            padding: 16px;
            transition: var(--transition);
            cursor: pointer;
        }
        .trending-item:hover { border-color: var(--primary-light); box-shadow: var(--shadow-card); }
        .trending-rank {
            font-size: 1.8rem;
            font-weight: 900;
            min-width: 45px;
            text-align: center;
        }
        .trending-rank.r1 { color: #FFD700; }
        .trending-rank.r2 { color: #C0C0C0; }
        .trending-rank.r3 { color: #CD7F32; }
        .trending-rank.r4,
        .trending-rank.r5 { color: var(--text-muted); }
        .trending-cover {
            width: 55px;
            height: 75px;
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.8rem;
            flex-shrink: 0;
        }
        .trending-info { flex: 1; }
        .trending-title { font-weight: 700; margin-bottom: 4px; }
        .trending-meta { font-size: 0.8rem; color: var(--text-muted); }
        .trending-btn {
            background: var(--gradient-1);
            color: white;
            border: none;
            padding: 8px 18px;
            border-radius: 50px;
            cursor: pointer;
            font-weight: 600;
            font-size: 0.82rem;
            transition: var(--transition);
            white-space: nowrap;
            font-family: inherit;
        }
        .trending-btn:hover { box-shadow: var(--shadow-neon); }

        /* ===== مودال ===== */
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.85);
            z-index: 9999;
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
        }
        .modal-overlay.active {
            opacity: 1;
            visibility: visible;
        }
        .modal {
            background: var(--bg-card);
            border: 1px solid var(--border);
            border-radius: var(--radius);
            padding: 30px;
            max-width: 550px;
            width: 90%;
            max-height: 80vh;
            overflow-y: auto;
            position: relative;
        }
        .modal-close {
            position: absolute;
            top: 12px;
            left: 16px;
            background: none;
            border: none;
            color: var(--text);
            font-size: 1.8rem;
            cursor: pointer;
        }
        .modal-cover {
            width: 120px;
            height: 160px;
            border-radius: 12px;
            margin: 0 auto 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 4rem;
        }
        .modal h2 { text-align: center; margin-bottom: 8px; }
        .modal .modal-author { text-align: center; color: var(--text-muted); margin-bottom: 16px; }
        .modal .modal-meta {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 16px;
            flex-wrap: wrap;
        }
        .modal .modal-meta span {
            background: rgba(168,85,247,0.15);
            padding: 6px 14px;
            border-radius: 50px;
            font-size: 0.85rem;
        }
        .modal .modal-desc {
            color: var(--text-muted);
            font-size: 0.9rem;
            margin-bottom: 20px;
            line-height: 1.8;
        }
        .modal .modal-btn {
            display: block;
            width: 100%;
            background: var(--gradient-1);
            color: white;
            border: none;
            padding: 14px;
            border-radius: 50px;
            font-weight: 700;
            font-size: 1rem;
            cursor: pointer;
            transition: var(--transition);
            text-align: center;
            font-family: inherit;
        }
        .modal .modal-btn:hover { box-shadow: var(--shadow-neon); }

        /* ===== الفوتر ===== */
        .footer {
            position: relative;
            z-index: 1;
            background: var(--bg-card);
            border-top: 1px solid var(--border);
            padding: 50px 20px 30px;
            text-align: center;
        }
        .footer-logo {
            font-size: 2rem;
            font-weight: 900;
            margin-bottom: 8px;
        }
        .footer-tagline { color: var(--text-muted); margin-bottom: 24px; font-size: 1rem; }
        .footer-links {
            display: flex;
            gap: 24px;
            justify-content: center;
            flex-wrap: wrap;
            margin-bottom: 24px;
        }
        .footer-links a {
            color: var(--text-muted);
            text-decoration: none;
            transition: var(--transition);
        }
        .footer-links a:hover { color: var(--neon); }
        .footer-social { display: flex; gap: 16px; justify-content: center; margin-bottom: 20px; }
        .social-icon {
            width: 42px;
            height: 42px;
            border-radius: 50%;
            background: var(--border);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            cursor: pointer;
            transition: var(--transition);
        }
        .social-icon:hover { background: var(--gradient-1); box-shadow: var(--shadow-neon); }
        .footer-copy { color: var(--text-muted); font-size: 0.85rem; }

        /* ===== زر العودة للأعلى ===== */
        .scroll-top {
            position: fixed;
            bottom: 30px;
            left: 30px;
            width: 48px;
            height: 48px;
            border-radius: 50%;
            background: var(--gradient-1);
            color: white;
            border: none;
            cursor: pointer;
            font-size: 1.3rem;
            z-index: 999;
            box-shadow: var(--shadow-neon);
            transition: var(--transition);
            opacity: 0;
            visibility: hidden;
            transform: translateY(20px);
        }
        .scroll-top.visible {
            opacity: 1;
            visibility: visible;
            transform: translateY(0);
        }
        .scroll-top:hover { transform: translateY(-4px) scale(1.05); }

        /* ===== تجاوب ===== */
        @media (max-width: 1400px) {
            .ad-sidebar { display: none; }
        }
        @media (max-width: 768px) {
            .header-inner { flex-wrap: wrap; gap: 10px; }
            .search-container { order: 3; max-width: 100%; flex: 100%; }
            .nav-links { display: none; }
            .mobile-menu-btn { display: block; }
            .hero { height: 300px; }
            .hero-slide { padding: 24px; }
            .hero h1 { font-size: 1.6rem; }
            .hero p { font-size: 0.9rem; }
            .stats-bar { grid-template-columns: repeat(2, 1fr); }
            .books-grid { grid-template-columns: repeat(auto-fill, minmax(140px, 1fr)); }
            .categories-grid { grid-template-columns: repeat(auto-fill, minmax(100px, 1fr)); }
            .trending-item { flex-wrap: wrap; }
            .trending-btn { width: 100%; text-align: center; }
            .main-content { margin-top: 190px; }
            .ad-banner-large { min-height: 150px; }
        }
    </style>
</head>
<body>

    <!-- شاشة التحميل -->
    <div class="loader" id="loader">
        <div class="loader-content">
            <div class="loader-book">📜</div>
            <div class="loader-logo">كايدن</div>
            <div class="loader-bar"><div class="loader-bar-fill"></div></div>
            <p style="color:var(--text-muted)">جاري تحميل عوالم الخيال...</p>
        </div>
    </div>

    <!-- خلفية النجوم -->
    <div class="stars-container" id="stars"></div>

    <!-- إعلانات جانبية -->
    <div class="ad-sidebar left" id="adLeft">
        <div>
            <div class="ad-label">إعلان</div>
            <p>مساحة<br>إعلانية<br>160×600</p>
        </div>
    </div>
    <div class="ad-sidebar right" id="adRight">
        <div>
            <div class="ad-label">إعلان</div>
            <p>مساحة<br>إعلانية<br>160×600</p>
        </div>
    </div>

    <!-- المودال -->
    <div class="modal-overlay" id="modalOverlay">
        <div class="modal" id="modalContent"></div>
    </div>

    <!-- إعلان أعلى الصفحة -->
    <div class="top-ad-bar">
        <div class="ad-content">
            <span class="ad-label">إعلان</span> 📢 مساحة إعلانية - 728×90 - للإعلان: ads@kaiden.com
        </div>
    </div>

    <!-- الهيدر -->
    <header class="header" id="header" style="top: 36px;">
        <div class="header-inner">
            <a href="#" class="logo">
                <span class="logo-icon">⚡</span>
                <span class="logo-gradient">كايدن</span>
            </a>
            <div class="search-container">
                <input type="text" class="search-input" placeholder="🔍 ابحث عن رواية، مانغا، مانهاوا، مانهوا...">
                <button class="search-btn">🔍</button>
            </div>
            <button class="mobile-menu-btn">☰</button>
            <button class="user-btn">👤 دخول / تسجيل</button>
        </div>
        <nav class="nav-links" style="padding:8px 20px 12px">
            <a href="#" class="active">الرئيسية</a>
            <a href="#">📚 روايات</a>
            <a href="#">🎭 مانغا</a>
            <a href="#">🌏 مانهاوا</a>
            <a href="#">🀄 مانهوا</a>
            <a href="#">📂 التصنيفات</a>
            <a href="#">🆕 أحدث الفصول</a>
        </nav>
    </header>

    <!-- المحتوى الرئيسي -->
    <main class="main-content">

        <!-- وصف الموقع -->
        <section class="site-description">
            <h2>⚡ كايدن - وجهتك الأولى لعوالم الخيال</h2>
            <p>موقع <strong>كايدن</strong> هو منصتك المتكاملة لقراءة <strong>الروايات العربية</strong>، <strong>المانغا اليابانية</strong>، <strong>المانهاوا الكورية</strong>، و<strong>المانهوا الصينية</strong> المترجمة. نقدم لك آلاف الأعمال المكتملة والمستمرة بجودة عالية وتحديثات يومية.</p>
            <div class="site-tags">
                <span class="site-tag">📚 روايات عربية</span>
                <span class="site-tag">🎭 مانغا يابانية</span>
                <span class="site-tag">🌏 مانهاوا كورية</span>
                <span class="site-tag">🀄 مانهوا صينية</span>
                <span class="site-tag">✅ مكتملة</span>
                <span class="site-tag">🔄 تحديث يومي</span>
                <span class="site-tag">💯 مجانية</span>
            </div>
        </section>

        <!-- إعلان بعد الوصف -->
        <div class="ad-banner">
            <div>
                <span class="ad-label">إعلان</span>
                <p>📢 مساحة إعلانية 970×90 - ضع إعلانك هنا ليصل لآلاف القراء يومياً</p>
            </div>
        </div>

        <!-- الهيرو سلايدر -->
        <section class="hero" id="hero">
            <div class="hero-slider" id="heroSlider">
                <div class="hero-slide">
                    <div class="hero-content">
                        <span class="hero-badge">🔥 جديد على كايدن</span>
                        <h1>اكتشف عوالم من الخيال</h1>
                        <p>روايات ومانغا ومانهاوا مترجمة بجودة عالية وتحديث يومي</p>
                        <a href="#" class="hero-btn">تصفح الآن 💜</a>
                    </div>
                </div>
                <div class="hero-slide">
                    <div class="hero-content">
                        <span class="hero-badge">⭐ الأكثر قراءة</span>
                        <h1>أفضل المانهاوا المترجمة</h1>
                        <p>مجموعة ضخمة من أحدث إصدارات المانهاوا الكورية والمانهوا الصينية</p>
                        <a href="#" class="hero-btn">استكشف 🎭</a>
                    </div>
                </div>
                <div class="hero-slide">
                    <div class="hero-content">
                        <span class="hero-badge">🆕 تحديث يومي</span>
                        <h1>فصول جديدة كل يوم</h1>
                        <p>لا تفوت أي تحديث، فصول جديدة تضاف يومياً على كايدن</p>
                        <a href="#" class="hero-btn">آخر التحديثات 📖</a>
                    </div>
                </div>
                <div class="hero-slide">
                    <div class="hero-content">
                        <span class="hero-badge">📚 مكتملة</span>
                        <h1>آلاف الأعمال المكتملة</h1>
                        <p>مجموعة ضخمة من الروايات والمانغا المكتملة مترجمة للعربية</p>
                        <a href="#" class="hero-btn">تصفح المكتبة 💜</a>
                    </div>
                </div>
            </div>
            <div class="hero-dots">
                <button class="hero-dot active" data-slide="0"></button>
                <button class="hero-dot" data-slide="1"></button>
                <button class="hero-dot" data-slide="2"></button>
                <button class="hero-dot" data-slide="3"></button>
            </div>
        </section>

        <!-- شريط الإحصائيات -->
        <div class="stats-bar">
            <div class="stat-card">
                <div class="stat-icon">📚</div>
                <div class="stat-number">+500</div>
                <div class="stat-label">رواية</div>
            </div>
            <div class="stat-card">
                <div class="stat-icon">🎭</div>
                <div class="stat-number">+800</div>
                <div class="stat-label">مانغا</div>
            </div>
            <div class="stat-card">
                <div class="stat-icon">🌏🀄</div>
                <div class="stat-number">+700</div>
                <div class="stat-label">مانهاوا ومانهوا</div>
            </div>
            <div class="stat-card">
                <div class="stat-icon">👥</div>
                <div class="stat-number">+50K</div>
                <div class="stat-label">قارئ</div>
            </div>
        </div>

        <!-- ✨ روايات مشهورة ومكتملة -->
        <section class="section">
            <div class="section-header">
                <h2 class="section-title"><span class="section-title-icon">📚</span> روايات مشهورة ومكتملة</h2>
                <a href="#" class="section-link">عرض الكل →</a>
            </div>
            <div class="books-grid">
                <div class="book-card" onclick="openModal('zicola')">
                    <div class="book-cover cover-1">🌍<span class="book-badge badge-complete">مكتملة</span></div>
                    <div class="book-info">
                        <div class="book-title">أرض زيكولا</div>
                        <div class="book-author">✍️ عمرو عبد الحميد</div>
                        <div class="book-meta"><span class="book-rating">⭐ 4.8</span><span class="book-chapters">📖 3 أجزاء</span></div>
                    </div>
                </div>
                <div class="book-card" onclick="openModal('jareteen')">
                    <div class="book-cover cover-2">🏰<span class="book-badge badge-complete">مكتملة</span></div>
                    <div class="book-info">
                        <div class="book-title">قواعد جارتين</div>
                        <div class="book-author">✍️ عمرو عبد الحميد</div>
                        <div class="book-meta"><span class="book-rating">⭐ 4.7</span><span class="book-chapters">📖 3 أجزاء</span></div>
                    </div>
                </div>
                <div class="book-card" onclick="openModal('daqeeqa')">
                    <div class="book-cover cover-3">⏱️<span class="book-badge badge-complete">مكتملة</span></div>
                    <div class="book-info">
                        <div class="book-title">دقيقة واحدة</div>
                        <div class="book-author">✍️ أحمد الشايب</div>
                        <div class="book-meta"><span class="book-rating">⭐ 4.5</span><span class="book-chapters">📖 جزء واحد</span></div>
                    </div>
                </div>
                <div class="book-card" onclick="openModal('antali')">
                    <div class="book-cover cover-4">💕<span class="book-badge badge-complete">مكتملة</span></div>
                    <div class="book-info">
                        <div class="book-title">أنت لي</div>
                        <div class="book-author">✍️ منى المرشود</div>
                        <div class="book-meta"><span class="book-rating">⭐ 4.6</span><span class="book-chapters">📖 جزء واحد</span></div>
                    </div>
                </div>
                <div class="book-card" onclick="openModal('tharthara')">
                    <div class="book-cover cover-5">🌊<span class="book-badge badge-featured">كلاسيكية</span></div>
                    <div class="book-info">
                        <div class="book-title">ثرثرة فوق النيل</div>
                        <div class="book-author">✍️ نجيب محفوظ</div>
                        <div class="book-meta"><span class="book-rating">⭐ 4.4</span><span class="book-chapters">📖 جزء واحد</span></div>
                    </div>
                </div>
                <div class="book-card" onclick="openModal('alkhemiai')">
                    <div class="book-cover cover-6">🔮<span class="book-badge badge-complete">مكتملة</span></div>
                    <div class="book-info">
                        <div class="book-title">الخيميائي</div>
                        <div class="book-author">✍️ باولو كويلو</div>
                        <div class="book-meta"><span class="book-rating">⭐ 4.9</span><span class="book-chapters">📖 جزء واحد</span></div>
                    </div>
                </div>
            </div>
        </section>

        <!-- إعلان بين الأقسام -->
        <div class="ad-banner">
            <div>
                <span class="ad-label">إعلان</span>
                <p>📢 مساحة إعلانية 970×90 - احجز مكانك الآن!</p>
            </div>
        </div>

        <!-- ✨ مانهوا مشهورة ومكتملة -->
        <section class="section">
            <div class="section-header">
                <h2 class="section-title"><span class="section-title-icon">🌏</span> مانهاوا كورية مشهورة</h2>
                <a href="#" class="section-link">عرض الكل →</a>
            </div>
            <div class="books-grid">
                <div class="book-card" onclick="openModal('sololeveling')">
                    <div class="book-cover cover-1">🗡️<span class="book-badge badge-complete">مكتملة</span></div>
                    <div class="book-info">
                        <div class="book-title">Solo Leveling</div>
                        <div class="book-author">✍️ Chugong</div>
                        <div class="book-meta"><span class="book-rating">⭐ 4.9</span><span class="book-chapters">🌏 200 فصل</span></div>
                    </div>
                </div>
                <div class="book-card" onclick="openModal('tbate')">
                    <div class="book-cover cover-2">🐉<span class="book-badge badge-hot">رائجة</span></div>
                    <div class="book-info">
                        <div class="book-title">The Beginning After The End</div>
                        <div class="book-author">✍️ TurtleMe</div>
                        <div class="book-meta"><span class="book-rating">⭐ 4.8</span><span class="book-chapters">🌏 175+ فصل</span></div>
                    </div>
                </div>
                <div class="book-card" onclick="openModal('noblesse')">
                    <div class="book-cover cover-4">🧛<span class="book-badge badge-complete">مكتملة</span></div>
                    <div class="book-info">
                        <div class="book-title">Noblesse</div>
                        <div class="book-author">✍️ Son Jeho</div>
                        <div class="book-meta"><span class="book-rating">⭐ 4.8</span><span class="book-chapters">🌏 544 فصل</span></div>
                    </div>
                </div>
                <div class="book-card" onclick="openModal('sweethome')">
                    <div class="book-cover cover-6">👹<span class="book-badge badge-complete">مكتملة</span></div>
                    <div class="book-info">
                        <div class="book-title">Sweet Home</div>
                        <div class="book-author">✍️ Kim Carnby</div>
                        <div class="book-meta"><span class="book-rating">⭐ 4.7</span><span class="book-chapters">🌏 141 فصل</span></div>
                    </div>
                </div>
            </div>
        </section>

        <!-- ✨ مانهوا صينية -->
        <section class="section">
            <div class="section-header">
                <h2 class="section-title"><span class="section-title-icon">🀄</span> مانهوا وروايات ويب صينية</h2>
                <a href="#" class="section-link">عرض الكل →</a>
            </div>
            <div class="books-grid">
                <div class="book-card" onclick="openModal('againstthegods')">
                    <div class="book-cover cover-5">⚔️<span class="book-badge badge-hot">رائجة</span></div>
                    <div class="book-info">
                        <div class="book-title">Against the Gods</div>
                        <div class="book-author">✍️ Mars Gravity</div>
                        <div class="book-meta"><span class="book-rating">⭐ 4.6</span><span class="book-chapters">🀄 2000+ فصل</span></div>
                    </div>
                </div>
                <div class="book-card" onclick="openModal('tdg')">
                    <div class="book-cover cover-3">👹<span class="book-badge badge-featured">مشهورة</span></div>
                    <div class="book-info">
                        <div class="book-title">Tales of Demons and Gods</div>
                        <div class="book-author">✍️ Mad Snail</div>
                        <div class="book-meta"><span class="book-rating">⭐ 4.5</span><span class="book-chapters">🀄 496 فصل</span></div>
                    </div>
                </div>
                <div class="book-card" onclick="openModal('issth')">
                    <div class="book-cover cover-1">🔖<span class="book-badge badge-complete">مكتملة</span></div>
                    <div class="book-info">
                        <div class="book-title">I Shall Seal the Heavens</div>
                        <div class="book-author">✍️ Er Gen</div>
                        <div class="book-meta"><span class="book-rating">⭐ 4.8</span><span class="book-chapters">🀄 1614 فصل</span></div>
                    </div>
                </div>
                <div class="book-card" onclick="openModal('coilingdragon')">
                    <div class="book-cover cover-2">🐉<span class="book-badge badge-complete">مكتملة</span></div>
                    <div class="book-info">
                        <div class="book-title">Coiling Dragon</div>
                        <div class="book-author">✍️ I Eat Tomatoes</div>
                        <div class="book-meta"><span class="book-rating">⭐ 4.7</span><span class="book-chapters">🀄 806 فصل</span></div>
                    </div>
                </div>
            </div>
        </section>

        <!-- إعلان كبير -->
        <div class="ad-banner ad-banner-large">
            <div>
                <span class="ad-label">إعلان</span>
                <p>📢 مساحة إعلانية كبيرة 970×250<br>مثالية للعروض والإعلانات البارزة</p>
            </div>
        </div>

        <!-- التصنيفات -->
        <section class="section">
            <div class="section-header">
                <h2 class="section-title"><span class="section-title-icon">📂</span> تصفح حسب التصنيف</h2>
            </div>
            <div class="categories-grid">
                <a href="#" class="category-card"><div class="category-icon">🗡️</div><div class="category-name">أكشن</div></a>
                <a href="#" class="category-card"><div class="category-icon">💕</div><div class="category-name">رومانسي</div></a>
                <a href="#" class="category-card"><div class="category-icon">🌍</div><div class="category-name">إيسيكاي</div></a>
                <a href="#" class="category-card"><div class="category-icon">👻</div><div class="category-name">رعب</div></a>
                <a href="#" class="category-card"><div class="category-icon">🧙</div><div class="category-name">فانتازيا</div></a>
                <a href="#" class="category-card"><div class="category-icon">🏫</div><div class="category-name">مدرسي</div></a>
                <a href="#" class="category-card"><div class="category-icon">⚔️</div><div class="category-name">شونين</div></a>
                <a href="#" class="category-card"><div class="category-icon">🤣</div><div class="category-name">كوميدي</div></a>
            </div>
        </section>

        <!-- الأكثر قراءة -->
        <section class="section">
            <div class="section-header">
                <h2 class="section-title"><span class="section-title-icon">📈</span> الأكثر رواجاً هذا الأسبوع</h2>
                <a href="#" class="section-link">عرض الكل →</a>
            </div>
            <div class="trending-list">
                <div class="trending-item" onclick="openModal('sololeveling')">
                    <span class="trending-rank r1">#1</span>
                    <div class="trending-cover cover-1">🗡️</div>
                    <div class="trending-info">
                        <div class="trending-title">Solo Leveling</div>
                        <div class="trending-meta">⭐ 4.9 · 200 فصل · مانهاوا كورية · مكتملة</div>
                    </div>
                    <button class="trending-btn">اقرأ الآن 💜</button>
                </div>
                <div class="trending-item" onclick="openModal('zicola')">
                    <span class="trending-rank r2">#2</span>
                    <div class="trending-cover cover-5">🌍</div>
                    <div class="trending-info">
                        <div class="trending-title">أرض زيكولا</div>
                        <div class="trending-meta">⭐ 4.8 · 3 أجزاء · رواية عربية · مكتملة</div>
                    </div>
                    <button class="trending-btn">اقرأ الآن 💜</button>
                </div>
                <div class="trending-item" onclick="openModal('tbate')">
                    <span class="trending-rank r3">#3</span>
                    <div class="trending-cover cover-2">🐉</div>
                    <div class="trending-info">
                        <div class="trending-title">The Beginning After The End</div>
                        <div class="trending-meta">⭐ 4.8 · 175+ فصل · مانهاوا · مستمرة</div>
                    </div>
                    <button class="trending-btn">تصفح 💜</button>
                </div>
                <div class="trending-item" onclick="openModal('noblesse')">
                    <span class="trending-rank r4">#4</span>
                    <div class="trending-cover cover-4">🧛</div>
                    <div class="trending-info">
                        <div class="trending-title">Noblesse</div>
                        <div class="trending-meta">⭐ 4.8 · 544 فصل · مانهاوا · مكتملة</div>
                    </div>
                    <button class="trending-btn">اقرأ 💜</button>
                </div>
                <div class="trending-item" onclick="openModal('jareteen')">
                    <span class="trending-rank r5">#5</span>
                    <div class="trending-cover cover-6">🏰</div>
                    <div class="trending-info">
                        <div class="trending-title">قواعد جارتين</div>
                        <div class="trending-meta">⭐ 4.7 · 3 أجزاء · رواية عربية · مكتملة</div>
                    </div>
                    <button class="trending-btn">تصفح 💜</button>
                </div>
            </div>
        </section>

        <!-- إعلان أسفل الصفحة -->
        <div class="ad-banner">
            <div>
                <span class="ad-label">إعلان</span>
                <p>📢 مساحة إعلانية 970×90 - أعلن معنا على كايدن</p>
            </div>
        </div>

    </main>

    <!-- الفوتر -->
    <footer class="footer">
        <div class="footer-logo">
            <span style="background:var(--gradient-1);-webkit-background-clip:text;-webkit-text-fill-color:transparent;">⚡ كايدن</span>
        </div>
        <p class="footer-tagline">وجهتك الأولى للروايات العربية، المانغا اليابانية، المانهاوا الكورية، والمانهوا الصينية المترجمة</p>
        <div class="footer-links">
            <a href="#">عن كايدن</a>
            <a href="#">اتصل بنا</a>
            <a href="#">سياسة الخصوصية</a>
            <a href="#">أعلن معنا</a>
            <a href="#">انضم ككاتب</a>
            <a href="#">انضم كمترجم</a>
        </div>
        <div class="footer-social">
            <div class="social-icon">📱</div>
            <div class="social-icon">🐦</div>
            <div class="social-icon">🎮</div>
            <div class="social-icon">📸</div>
        </div>
        <p class="footer-copy">© 2025 كايدن - Kaiden. كل الحقوق محفوظة</p>
    </footer>

    <!-- زر العودة للأعلى -->
    <button class="scroll-top" id="scrollTop">↑</button>

    <script>
        // ========== بيانات الأعمال ==========
        const worksData = {
            zicola: {
                title: 'أرض زيكولا',
                author: 'عمرو عبد الحميد',
                coverClass: 'cover-1',
                coverEmoji: '🌍',
                badges: '<span class="book-badge badge-complete">مكتملة
