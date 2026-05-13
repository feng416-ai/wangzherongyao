<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>王者荣耀攻略站 - 英雄详情下钻版</title>
    <style>
        :root { --bg: #0b101b; --card: #161c2e; --gold: #c9a063; --text: #a0a8b9; }
        body { font-family: "Microsoft YaHei"; background: var(--bg); color: white; margin: 0; padding: 20px; }
        .hero-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px; }
        .hero-card { background: var(--card); border: 1px solid #2d364d; border-radius: 8px; display: flex; overflow: hidden; position: relative; }
        /* 修复图片显示 */
        .hero-img { width: 120px; height: 160px; object-fit: cover; background: #222; }
        .hero-info { padding: 15px; flex: 1; }
        .hero-info h3 { margin: 0 0 10px 0; color: var(--gold); }
        .tag { background: rgba(201,160,99,0.2); color: var(--gold); padding: 2px 6px; border-radius: 4px; font-size: 12px; }
        /* 下钻按钮样式 */
        .btn-detail { 
            display: inline-block; margin-top: 10px; padding: 5px 15px; 
            background: var(--gold); color: black; text-decoration: none; 
            border-radius: 4px; font-weight: bold; font-size: 13px;
        }
        .btn-detail:hover { background: #e0b370; }
    </style>
</head>
<body>

<h2 style="border-left: 5px solid var(--gold); padding-left: 15px;">英雄攻略精选 (点击按钮查看详情)</h2>

<div class="hero-grid">
    <!-- 李白卡片 -->
    <div class="hero-card">
        <img src="https://game.gtimg.cn/images/yxzj/img201605/heroimg/131/131.jpg" class="hero-img" alt="李白">
        <div class="hero-info">
            <h3>李白 <span class="tag">刺客</span></h3>
            <p style="font-size: 13px; color: var(--text);">核心技巧：1技能起手，利用野怪刷大...</p>
            <!-- 下钻链接：指向 libai.html -->
            <a href="libai.html" class="btn-detail">查看完整攻略</a>
        </div>
    </div>

    <!-- 后羿卡片 -->
    <div class="hero-card">
        <img src="https://game.gtimg.cn/images/yxzj/img201605/heroimg/169/169.jpg" class="hero-img" alt="后羿">
        <div class="hero-info">
            <h3>后羿 <span class="tag">射手</span></h3>
            <p style="font-size: 13px; color: var(--text);">核心技巧：注意走位，大招全图支援...</p>
            <!-- 下钻链接：指向 houyi.html -->
            <a href="houyi.html" class="btn-detail">查看完整攻略</a>
        </div>
    </div>
</div>

</body>
</html>
