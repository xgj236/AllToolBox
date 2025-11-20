<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AllToolBox - 小天才工具箱</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', 'Microsoft YaHei', sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            color: #333;
            line-height: 1.6;
            min-height: 100vh;
            padding: 20px;
        }
        
        .container {
            max-width: 1000px;
            margin: 0 auto;
            background-color: white;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            overflow: hidden;
        }
        
        header {
            background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%);
            color: white;
            padding: 40px 30px;
            text-align: center;
            position: relative;
        }
        
        .logo {
            font-size: 3.5rem;
            margin-bottom: 15px;
            color: #FFD700;
        }
        
        h1 {
            font-size: 2.8rem;
            margin-bottom: 15px;
            letter-spacing: 1px;
        }
        
        .tagline {
            font-size: 1.2rem;
            opacity: 0.9;
            max-width: 600px;
            margin: 0 auto;
        }
        
        .content {
            padding: 40px 30px;
        }
        
        .download-section {
            background-color: #f8f9fa;
            border-radius: 15px;
            padding: 30px;
            margin-bottom: 40px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .download-title {
            font-size: 1.8rem;
            margin-bottom: 25px;
            color: #2c3e50;
        }
        
        .download-buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }
        
        .download-btn {
            display: flex;
            align-items: center;
            gap: 10px;
            background: linear-gradient(135deg, #6a11cb 0%, #2575fc 100%);
            color: white;
            padding: 15px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(106, 17, 203, 0.3);
        }
        
        .download-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(106, 17, 203, 0.4);
        }
        
        .download-btn.secondary {
            background: linear-gradient(135deg, #00b09b 0%, #96c93d 100%);
            box-shadow: 0 5px 15px rgba(0, 176, 155, 0.3);
        }
        
        .download-btn.secondary:hover {
            box-shadow: 0 8px 20px rgba(0, 176, 155, 0.4);
        }
        
        .changelog-section {
            margin-top: 40px;
        }
        
        .section-title {
            font-size: 1.8rem;
            margin-bottom: 25px;
            color: #2c3e50;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .section-title i {
            color: #6a11cb;
        }
        
        .changelog-container {
            background-color: #f8f9fa;
            border-radius: 15px;
            padding: 25px;
            max-height: 400px;
            overflow-y: auto;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .changelog-item {
            padding: 20px;
            border-left: 4px solid #6a11cb;
            background-color: white;
            margin-bottom: 20px;
            border-radius: 0 10px 10px 0;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.05);
            transition: transform 0.2s ease;
        }
        
        .changelog-item:hover {
            transform: translateX(5px);
        }
        
        .changelog-item:last-child {
            margin-bottom: 0;
        }
        
        .version {
            font-weight: 700;
            color: #6a11cb;
            font-size: 1.2rem;
            margin-bottom: 5px;
        }
        
        .date {
            color: #7f8c8d;
            font-size: 0.9rem;
            margin-bottom: 10px;
        }
        
        .changes {
            list-style-type: none;
        }
        
        .changes li {
            margin-bottom: 8px;
            padding-left: 20px;
            position: relative;
        }
        
        .changes li:before {
            content: "•";
            color: #6a11cb;
            font-weight: bold;
            position: absolute;
            left: 0;
        }
        
        footer {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 20px;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            .download-buttons {
                flex-direction: column;
                align-items: center;
            }
            
            .download-btn {
                width: 100%;
                max-width: 300px;
                justify-content: center;
            }
            
            h1 {
                font-size: 2.2rem;
            }
            
            .logo {
                font-size: 2.8rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="logo">
                <i class="fas fa-toolbox"></i>
            </div>
            <h1>AllToolBox</h1>
            <p class="tagline">一个专为小天才设计的强大工具箱，包含多种实用工具</p>
        </header>
        
        <div class="content">
            <section class="download-section">
                <h2 class="download-title">立即下载 AllToolBox</h2>
                <div class="download-buttons">
                    <a href="https://atb.xgj.qzz.io/AllToolBox.zip" class="download-btn">
                        <i class="fas fa-download"></i>
                        主下载通道
                    </a>
                    <a href="https://xgj236.github.io/AllToolBox.zip" class="download-btn secondary">
                        <i class="fas fa-rocket"></i>
                        备用下载通道
                    </a>
                </div>
            </section>
            
            <section class="changelog-section">
                <h2 class="section-title">
                    <i class="fas fa-history"></i>
                    更新日志
                </h2>
                <div class="changelog-container">
                </div>
            </section>
        </div>
        
        <footer>
            <p>AllToolBox - 小天才工具箱 | 作者：快乐的小公爵</p>
        </footer>
    </div>

    <script>
        // 添加简单的交互效果
        document.addEventListener('DOMContentLoaded', function() {
            // 为更新日志项添加点击效果
            const changelogItems = document.querySelectorAll('.changelog-item');
            changelogItems.forEach(item => {
                item.addEventListener('click', function() {
                    // 移除其他项目的active类
                    changelogItems.forEach(i => i.classList.remove('active'));
                    // 为当前项目添加active类
                    this.classList.add('active');
                });
            });
            
            // 添加下载按钮点击动画
            const downloadBtns = document.querySelectorAll('.download-btn');
            downloadBtns.forEach(btn => {
                btn.addEventListener('click', function(e) {
                    // 创建点击效果
                    const rect = this.getBoundingClientRect();
                    const x = e.clientX - rect.left;
                    const y = e.clientY - rect.top;
                    
                    const ripple = document.createElement('span');
                    ripple.style.position = 'absolute';
                    ripple.style.borderRadius = '50%';
                    ripple.style.background = 'rgba(255, 255, 255, 0.5)';
                    ripple.style.transform = 'scale(0)';
                    ripple.style.animation = 'ripple 0.6s linear';
                    ripple.style.left = x + 'px';
                    ripple.style.top = y + 'px';
                    
                    this.style.position = 'relative';
                    this.style.overflow = 'hidden';
                    this.appendChild(ripple);
                    
                    setTimeout(() => {
                        ripple.remove();
                    }, 600);
                });
            });
        });
        
        // 添加CSS动画
        const style = document.createElement('style');
        style.textContent = `
            @keyframes ripple {
                to {
                    transform: scale(4);
                    opacity: 0;
                }
            }
            
            .changelog-item.active {
                transform: scale(1.02);
                box-shadow: 0 5px 15px rgba(106, 17, 203, 0.2);
            }
        `;
        document.head.appendChild(style);
    </script>
</body>
</html>
