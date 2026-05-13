<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>王者荣耀攻略站 - 助你轻松上王者</title>
    <style>
        :root {
            --bg-dark: #0b0e18;
            --card-bg: #1a2235;
            --gold: #c9a063;
            --text-gray: #a0a8b9;
            --border: #2d364d;
        }

        body {
            font-family: "PingFang SC", "Microsoft YaHei", sans-serif;
            background-color: var(--bg-dark);
            color: white;
            margin: 0;
            display: flex;
            flex-direction: column;
        }

        /* 导航栏 */
        header {
            background: #161c2e;
            padding: 15px 5%;
            display: flex;
            align-items: center;
            justify-content: space-between;
            border-bottom: 2px solid var(--gold);
            position: sticky;
            top: 0;
            z-index: 100;
        }

        .logo { font-size: 24px; font-weight: bold; color: var(--gold); }
        .search-bar {
            background: #252d3f;
            border: 1px solid var(--border);
            padding: 8px 15px;
            border-radius: 20px;
            width: 300px;
            color: white;
        }

        /* 主体布局 */
        .main-layout {
            display: grid;
            grid-template-columns: 250px 1fr 280px;
            gap: 20px;
            padding: 20px 3%;
        }

        .section-title {
            border-left: 4px solid var(--gold);
            padding-left: 10px;
            margin-bottom: 15px;
            font-size: 18px;
        }

        /* 通用卡片样式 */
        .card {
            background: var(--card-bg);
            border-radius: 8px;
            padding: 15px;
            border: 1px solid var(--border);
        }

        /* 英雄精选列表 */
        .hero-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
        }

        .hero-card {
            display: flex;
            gap: 15px;
        }

        .hero-img {
            width: 100px;
            height: 140px;
            border-radius: 6px;
            object-fit: cover;
            background: #333;
        }

        .hero-info h3 { margin: 0; color: var(--gold); }
        .hero-info p { font-size: 13px; color: var(--text-gray); line-height: 1.6; }
        .tag { background: rgba(201, 160, 99, 0.2); color: var(--gold); padding: 2px 6px; border-radius: 4px; font-size: 11px; }

        /* 大神出装 */
        .build-item {
            display: flex;
            align-items: center;
            justify-content: space-between;
            margin-bottom: 10px;
            background: rgba(255,255,255,0.05);
            padding: 8px;
            border-radius: 4px;
        }
        .item-icons { display: flex; gap: 5px; }
        .item-icon { width: 30px; height: 30px; background: #444; border-radius: 50%; border: 1px solid var(--gold); }

        /* 响应式适配 */
        @media (max-width: 1024px) {
            .main-layout { grid-template-columns: 1fr; }
            .side-panel { display: none; }
        }
    </style>
</head>
<body>

<header>
    <div class="logo">🛡️ 王者荣耀攻略站</div>
    <input type="text" class="search-bar" placeholder="搜索英雄、出装、版本攻略...">
    <div style="color:var(--text-gray)">助你轻松上王者</div>
</header>

<div class="main-layout">
    <!-- 左侧：版本大事记 -->
    <aside class="side-panel">
        <div class="section-title">版本大事件</div>
        <div class="card">
            <ul style="list-style: none; padding: 0; font-size: 14px; line-height: 2.5;">
                <li>🔹 S30赛季段位继承规则发布</li>
                <li>🔹 王者荣耀段位教学：下马英雄...</li>
                <li>🔹 新英雄姬小满强力降临</li>
                <li>🔹 S30赛季巅峰赛挑战赛开启</li>
                <li>🔹 碎片商店更新预览</li>
            </ul>
        </div>
    </aside>

    <!-- 中间：核心攻略区 -->
    <main>
        <div class="section-title">英雄攻略精选</div>
        <div class="hero-grid">
            <!-- 李白 -->
            <div class="card hero-card">
                <img src="https://via.placeholder.com/100x140/c9a063/ffffff?text=Li+Bai" class="hero-img" alt="李白">
                <div class="hero-info">
                    <h3>李白 <span class="tag">刺客</span></h3>
                    <p><strong>技能优先：</strong> 主一副二，有大点大</p>
                    <p><strong>核心技巧：</strong> 利用野怪刷出大招解封，1技能两段位移切入，2技能神速躲避控制。</p>
                </div>
            </div>
            <!-- 后羿 -->
            <div class="card hero-card">
                <img src="https://via.placeholder.com/100x140/c9a063/ffffff?text=Hou+Yi" class="hero-img" alt="后羿">
                <div class="hero-info">
                    <h3>后羿 <span class="tag">射手</span></h3>
                    <p><strong>技能优先：</strong> 主二副一</p>
                    <p><strong>核心技巧：</strong> 注意走位，大招全图支援开启团战，后期配合逐日之弓远程输出。</p>
                </div>
            </div>
        </div>

        <div class="section-title" style="margin-top: 30px;">热门教学视频</div>
        <div class="hero-grid">
            <div class="card" style="text-align: center;">
                <div style="height: 120px; background: #000; display: flex; align-items: center; justify-content: center; border-radius: 5px; margin-bottom: 10px;">▶️</div>
                <div style="font-size: 14px;">全英雄最全连招教学</div>
            </div>
            <div class="card" style="text-align: center;">
                <div style="height: 120px; background: #000; display: flex; align-items: center; justify-content: center; border-radius: 5px; margin-bottom: 10px;">▶️</div>
                <div style="font-size: 14px;">逆风翻盘技巧分享</div>
            </div>
        </div>
    </main>

    <!-- 右侧：出装与论坛 -->
    <aside class="side-panel">
        <div class="section-title">大神出装推荐</div>
        <div class="card">
            <div class="build-item">
                <span>坦克</span>
                <div class="item-icons">
                    <div class="item-icon"></div><div class="item-icon"></div><div class="item-icon"></div>
                </div>
            </div>
            <div class="build-item">
                <span>魔序</span>
                <div class="item-icons">
                    <div class="item-icon"></div><div class="item-icon"></div><div class="item-icon"></div>
                </div>
            </div>
        </div>

        <div class="section-title" style="margin-top: 20px;">玩家讨论区</div>
        <div class="card" style="font-size: 13px; color: var(--text-gray);">
            <p>💬 赵云怎么玩？才玩两把被骂惨了...</p>
            <p>💬 谁是版本最强法师？</p>
            <p>💬 这届玩家不行？遇到挂机怎么办</p>
        </div>
    </aside>
</div>

</body>
</html>
