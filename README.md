<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NIGEL PARRY 尼格博瑞 - 高端男装品牌</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', 'Microsoft YaHei', sans-serif;
        }
        
        body {
            background-color: #0a0a0a;
            color: #e6e6e6;
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* 头部样式 */
        header {
            background-color: rgba(10, 10, 10, 0.95);
            padding: 20px 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            border-bottom: 1px solid #333;
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 28px;
            font-weight: 300;
            letter-spacing: 3px;
            color: #d4af37;
            text-decoration: none;
        }
        
        .logo span {
            font-weight: 600;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav li {
            margin-left: 40px;
        }
        
        nav a {
            color: #e6e6e6;
            text-decoration: none;
            font-weight: 300;
            font-size: 16px;
            letter-spacing: 1px;
            transition: color 0.3s;
            position: relative;
        }
        
        nav a:hover {
            color: #d4af37;
        }
        
        nav a::after {
            content: '';
            position: absolute;
            width: 0;
            height: 1px;
            background: #d4af37;
            bottom: -5px;
            left: 0;
            transition: width 0.3s;
        }
        
        nav a:hover::after {
            width: 100%;
        }
        
        .mobile-menu-btn {
            display: none;
            font-size: 24px;
            cursor: pointer;
        }
        
        /* 英雄区域 */
        .hero {
            height: 100vh;
            background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url('https://images.unsplash.com/photo-1594938374186-90f5d75cf0a5?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2070&q=80');
            background-size: cover;
            background-position: center;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding-top: 80px;
        }
        
        .hero-content {
            max-width: 800px;
            padding: 0 20px;
        }
        
        .hero h1 {
            font-size: 4.5rem;
            font-weight: 300;
            margin-bottom: 20px;
            letter-spacing: 5px;
            color: #fff;
        }
        
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 40px;
            font-weight: 300;
            letter-spacing: 1px;
            line-height: 1.8;
        }
        
        .cta-button {
            display: inline-block;
            padding: 15px 40px;
            background-color: transparent;
            color: #d4af37;
            border: 1px solid #d4af37;
            text-decoration: none;
            font-size: 16px;
            letter-spacing: 2px;
            transition: all 0.3s;
            margin-top: 20px;
        }
        
        .cta-button:hover {
            background-color: #d4af37;
            color: #0a0a0a;
        }
        
        /* 内容区域 */
        section {
            padding: 100px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 60px;
            position: relative;
        }
        
        .section-title h2 {
            font-size: 2.5rem;
            font-weight: 300;
            letter-spacing: 3px;
            color: #d4af37;
            display: inline-block;
            padding-bottom: 15px;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            width: 100px;
            height: 1px;
            background: #d4af37;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
        }
        
        .content-block {
            margin-bottom: 60px;
        }
        
        .content-block h3 {
            font-size: 1.8rem;
            margin-bottom: 20px;
            color: #d4af37;
            font-weight: 400;
            letter-spacing: 1px;
        }
        
        .content-block p {
            font-size: 1.1rem;
            line-height: 1.8;
            margin-bottom: 20px;
            font-weight: 300;
            color: #ccc;
        }
        
        .highlight {
            color: #d4af37;
            font-weight: 400;
        }
        
        /* 品牌特色区域 */
        .features {
            background-color: #111;
        }
        
        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
        }
        
        .feature-item {
            text-align: center;
            padding: 40px 30px;
            border: 1px solid #333;
            transition: all 0.3s;
        }
        
        .feature-item:hover {
            border-color: #d4af37;
            transform: translateY(-10px);
        }
        
        .feature-icon {
            font-size: 3rem;
            color: #d4af37;
            margin-bottom: 25px;
        }
        
        .feature-item h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
            letter-spacing: 1px;
        }
        
        .feature-item p {
            font-size: 1rem;
            color: #aaa;
        }
        
        /* 图库区域 */
        .gallery {
            background-color: #0a0a0a;
        }
        
        .gallery-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .gallery-item {
            height: 300px;
            overflow: hidden;
            position: relative;
        }
        
        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s;
        }
        
        .gallery-item:hover img {
            transform: scale(1.05);
        }
        
        .gallery-overlay {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(transparent, rgba(0, 0, 0, 0.8));
            color: #fff;
            padding: 20px;
            transform: translateY(100%);
            transition: transform 0.3s;
        }
        
        .gallery-item:hover .gallery-overlay {
            transform: translateY(0);
        }
        
        /* 页脚 */
        footer {
            background-color: #080808;
            padding: 60px 0 30px;
            border-top: 1px solid #333;
        }
        
        .footer-content {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            margin-bottom: 40px;
        }
        
        .footer-column {
            flex: 1;
            min-width: 250px;
            margin-bottom: 30px;
        }
        
        .footer-column h3 {
            font-size: 1.3rem;
            margin-bottom: 25px;
            color: #d4af37;
            letter-spacing: 1px;
        }
        
        .footer-column p, .footer-column a {
            color: #aaa;
            margin-bottom: 10px;
            display: block;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-column a:hover {
            color: #d4af37;
        }
        
        .social-icons {
            display: flex;
            gap: 20px;
            margin-top: 20px;
        }
        
        .social-icons a {
            font-size: 1.2rem;
            color: #aaa;
            transition: color 0.3s;
        }
        
        .social-icons a:hover {
            color: #d4af37;
        }
        
        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid #333;
            color: #777;
            font-size: 0.9rem;
        }
        
        /* 响应式设计 */
        @media (max-width: 992px) {
            .hero h1 {
                font-size: 3.5rem;
            }
            
            .features-grid {
                grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            }
        }
        
        @media (max-width: 768px) {
            .mobile-menu-btn {
                display: block;
            }
            
            nav ul {
                position: fixed;
                top: 80px;
                left: -100%;
                width: 100%;
                height: calc(100vh - 80px);
                background-color: rgba(10, 10, 10, 0.98);
                flex-direction: column;
                align-items: center;
                justify-content: flex-start;
                padding-top: 50px;
                transition: left 0.3s;
            }
            
            nav.active ul {
                left: 0;
            }
            
            nav li {
                margin: 0 0 30px 0;
            }
            
            .hero h1 {
                font-size: 2.8rem;
            }
            
            .section-title h2 {
                font-size: 2rem;
            }
        }
        
        @media (max-width: 576px) {
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .hero p {
                font-size: 1rem;
            }
            
            .cta-button {
                padding: 12px 30px;
            }
        }
    .gallery-item1 {            height: 300px;
            overflow: hidden;
            position: relative;
}
    </style>
</head>
<body>
    <!-- 头部导航 -->
    <header>
        <div class="container header-container">
            <a href="#" class="logo"> <span>NIGEL PARRY</span></a>
            <nav id="mainNav">
                <ul>
                    <li><a href="#home">首页</a></li>
                    <li><a href="#about">品牌故事</a></li>
                    <li><a href="#philosophy">品牌理念</a></li>
                    <li><a href="#features">品牌特色</a></li>
                    <li><a href="#gallery">视觉呈现</a></li>
                </ul>
            </nav>
            <div class="mobile-menu-btn" id="mobileMenuBtn">
                <i class="fas fa-bars"></i>
            </div>
        </div>
    </header>

    <!-- 英雄区域 -->
    <section class="hero" id="home">
        <div class="hero-content">
          <h1><strong>NIGEL PARRY</strong></h1>
          <p>英格兰人物摄影师，以独特的视角展现人物风格的瞬间。随着快门的开启，时间被凝固下来，作为"此时此刻"的记录是不可重复的，也就成为永远。</p>
            <a href="#about" class="cta-button">探索品牌故事</a>
      </div>
    </section>

    <!-- 品牌故事 -->
    <section id="about">
        <div class="container">
            <div class="section-title">
                <h2>品牌故事</h2>
            </div>
          <div class="content-block">
            <h3>NIGEL PARRY - 尼格博瑞</h3>
            <p><strong>NIGEL PARRY</strong>品牌倡导的是人性化的生活理念，讲究传统与创新的结合，注重生活质量，享受休闲的生活方式。<strong>NIGEL PARRY</strong>的男人总是喜欢搭配服装，每时每刻生活在优雅之中。</p>
            <p><strong>NIGEL PARRY</strong>生产的不仅是产品也是艺术品，让着装成为享受，视觉的享受和心灵的享受。他们用这种美学原理提高着产品的附加值，给消费者全新的生活体验。无时无刻不让消费者在体验美的感觉与生活，品味到美的存在。</p>
          </div>
        </div>
    </section>

    <!-- 品牌理念 -->
    <section id="philosophy" class="features">
        <div class="container">
            <div class="section-title">
                <h2>品牌理念</h2>
            </div>
          <div class="content-block">
            <p><strong>NIGEL</strong> <strong>PARRY</strong>品牌选用与国际流行同步的面料，时尚简约的设计风格，展现服装外观的细致，挺括，内敛，使穿着者穿着舒适和随意，塑造出现代都市成功男士突破自我，修身时尚，优雅绅士的浪漫形象，体现出都市生活中男性所追求的与众不同全新形象，使自己最经典的瞬间成为生活品味的永恒。</p>
            <p><strong>NIGEL</strong> <strong>PARRY</strong>尼格博瑞品牌的网点建设充分考虑高端消费者的购物需求，在店面设置、店面装修、产品陈列、人员服务等方面体现顾客的尊贵身份，让顾客在购物的过程之中获得一种全新的购物体验。</p>
          </div>
        </div>
    </section>

    <!-- 品牌特色 -->
    <section id="features">
        <div class="container">
            <div class="section-title">
                <h2>品牌特色</h2>
            </div>
            <div class="features-grid">
                <div class="feature-item">
                    <div class="feature-icon">
                        <i class="fas fa-camera-retro"></i>
                    </div>
                    <h3>摄影美学</h3>
                    <p>源自英格兰人物摄影师的独特视角，将瞬间的优雅凝固为永恒的艺术，融入服装设计之中。</p>
                </div>
                <div class="feature-item">
                    <div class="feature-icon">
                        <i class="fas fa-cut"></i>
                    </div>
                    <h3>精湛工艺</h3>
                    <p>选用国际同步流行的高品质面料，结合时尚简约的设计，展现服装的细致、挺括与内敛。</p>
                </div>
                <div class="feature-item">
                    <div class="feature-icon">
                        <i class="fas fa-crown"></i>
                    </div>
                    <h3>绅士风范</h3>
                    <p>塑造现代都市成功男士突破自我、修身时尚、优雅绅士的浪漫形象，彰显独特品味。</p>
                </div>
            </div>
        </div>
    </section>

    <!-- 视觉呈现 -->
    <section id="gallery" class="gallery">
        <div class="container">
            <div class="section-title">
                <h2>视觉呈现</h2>
            </div>
            <div class="gallery-grid">
                <div class="gallery-item">
                  <img src="https://images.unsplash.com/photo-1591047139829-d91aecb6caea?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Nigel Parry 男装展示">
                    <div class="gallery-overlay">
                        <h3>优雅绅士系列</h3>
                    </div>
                </div>
                <div class="gallery-item">
                  <img src="https://images.unsplash.com/photo-1602810318383-e386cc2a3ccf?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Nigel Parry 面料细节">
                    <div class="gallery-overlay">
                        <h3>精选面料细节</h3>
                    </div>
                </div>
                <div class="gallery-item">
                    <img src="https://ix-marketing.imgix.net/case-study_tile_ikyu.png?auto=format,compress&w=1946" alt="Nigel Parry 店铺展示">
                    <div class="gallery-overlay">
                      <h3>高端购物体验</h3>
                  </div>
              </div>
            </div>
        </div>
    </section>

    <!-- 页脚 -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3>NIGEL PARRY</h3>
                    <p>源自英格兰的高端男装品牌，将摄影美学与服装设计完美融合，为现代绅士提供独特的着装体验。</p>
                    <div class="social-icons">
                        <a href="#"><i class="fab fa-weibo"></i></a>
                        <a href="#"><i class="fab fa-weixin"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                    </div>
                </div>
                <div class="footer-column">
                    <h3>品牌理念</h3>
                    <p>人性化的生活理念</p>
                    <p>传统与创新的结合</p>
                    <p>注重生活质量</p>
                    <p>享受休闲的生活方式</p>
                </div>
                <div class="footer-column">
                    <h3>联系我们</h3>
                    <p>中国旗舰店：西安市</p>
                  <p>电话：+87194386</p>
                    <p>邮箱：NP@nigelparry.com</p>
                    <p>官网：www.nigelparry.cn</p>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2023 NIGEL PARRY 尼格博瑞. 保留所有权利.</p>
            </div>
        </div>
    </footer>

    <script>
        // 移动端菜单切换
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const mainNav = document.getElementById('mainNav');
        
        mobileMenuBtn.addEventListener('click', () => {
            mainNav.classList.toggle('active');
            mobileMenuBtn.innerHTML = mainNav.classList.contains('active') 
                ? '<i class="fas fa-times"></i>' 
                : '<i class="fas fa-bars"></i>';
        });
        
        // 平滑滚动
        document.querySelectorAll('nav a, .cta-button').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                if(this.getAttribute('href').startsWith('#')) {
                    e.preventDefault();
                    
                    const targetId = this.getAttribute('href');
                    const targetSection = document.querySelector(targetId);
                    
                    if(targetSection) {
                        window.scrollTo({
                            top: targetSection.offsetTop - 80,
                            behavior: 'smooth'
                        });
                        
                        // 关闭移动端菜单
                        if(mainNav.classList.contains('active')) {
                            mainNav.classList.remove('active');
                            mobileMenuBtn.innerHTML = '<i class="fas fa-bars"></i>';
                        }
                    }
                }
            });
        });
        
        // 滚动时改变导航栏透明度
        window.addEventListener('scroll', () => {
            const header = document.querySelector('header');
            if(window.scrollY > 100) {
                header.style.backgroundColor = 'rgba(10, 10, 10, 0.98)';
            } else {
                header.style.backgroundColor = 'rgba(10, 10, 10, 0.95)';
            }
        });
    </script>
</body>
</html>
