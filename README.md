# bfunday.github.io
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes">
    <title>经济法实境案例库 · 案例20</title>
    <!-- Font Awesome 图标库 (可选) -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', 'Noto Sans', sans-serif;
        }
        body {
            background-color: #f5f7fa;
            padding: 20px 16px 40px;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        .case-container {
            max-width: 720px;
            width: 100%;
            background-color: #ffffff;
            border-radius: 28px;
            box-shadow: 0 12px 30px rgba(0, 20, 50, 0.08);
            overflow: hidden;
            padding: 24px 20px 32px;
            margin-bottom: 24px;
        }
        /* 头部标识 */
        .case-header {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            border-bottom: 2px solid #eef2f6;
            padding-bottom: 16px;
        }
        .case-meta {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            align-items: center;
        }
        .module-badge {
            background-color: #2A5CAA;
            color: white;
            font-size: 0.75rem;
            font-weight: 600;
            padding: 4px 12px;
            border-radius: 50px;
            letter-spacing: 0.5px;
            display: inline-block;
        }
        .case-number {
            background-color: #e9ecf3;
            color: #1e3a6b;
            font-size: 0.75rem;
            font-weight: 600;
            padding: 4px 12px;
            border-radius: 50px;
        }
        .qr-placeholder {
            width: 60px;
            height: 60px;
            background: linear-gradient(145deg, #f0f3f8, #ffffff);
            border: 1px dashed #a0b8d4;
            border-radius: 12px;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            font-size: 0.6rem;
            color: #4a6a9e;
            box-shadow: 0 2px 6px rgba(0,0,0,0.02);
        }
        .qr-placeholder i {
            font-size: 1.5rem;
            margin-bottom: 2px;
            color: #2A5CAA;
        }
        .qr-placeholder span {
            background: #eef2f6;
            padding: 2px 6px;
            border-radius: 20px;
            font-weight: 500;
        }
        h1 {
            font-size: 1.7rem;
            font-weight: 700;
            line-height: 1.3;
            margin: 16px 0 8px;
            color: #0B1C3A;
        }
        .subtitle {
            font-size: 0.95rem;
            color: #4a5b79;
            background-color: #f0f4fc;
            padding: 8px 14px;
            border-radius: 30px;
            display: inline-block;
            margin-bottom: 20px;
        }
        .section-title {
            font-size: 1.2rem;
            font-weight: 650;
            color: #1e3a6b;
            margin: 28px 0 16px 0;
            display: flex;
            align-items: center;
            gap: 10px;
            border-left: 5px solid #2A5CAA;
            padding-left: 15px;
        }
        .section-title i {
            color: #2A5CAA;
            font-size: 1.3rem;
        }
        .card {
            background-color: #f9fbfe;
            border-radius: 20px;
            padding: 18px 20px;
            margin-bottom: 20px;
            box-shadow: 0 2px 8px rgba(0,20,40,0.02);
            border: 1px solid #e6ecf5;
        }
        .card p {
            color: #1e2f4a;
            line-height: 1.6;
            font-size: 1rem;
        }
        .law-list, .think-list {
            list-style: none;
        }
        .law-list li, .think-list li {
            margin-bottom: 14px;
            padding-left: 28px;
            position: relative;
            line-height: 1.5;
        }
        .law-list li i, .think-list li i {
            position: absolute;
            left: 0;
            top: 2px;
            color: #2A5CAA;
            font-size: 1.1rem;
        }
        .tag-group {
            display: flex;
            flex-wrap: wrap;
            gap: 8px 12px;
            margin: 16px 0 8px;
        }
        .tag {
            background-color: #e0e8f5;
            color: #1e3a6b;
            font-size: 0.8rem;
            padding: 4px 12px;
            border-radius: 30px;
            font-weight: 500;
        }
        .param-table {
            width: 100%;
            border-collapse: collapse;
            font-size: 0.95rem;
        }
        .param-table th {
            text-align: left;
            background-color: #d9e4f5;
            color: #0d2b55;
            font-weight: 600;
            padding: 10px 12px;
            border-radius: 16px 16px 0 0;
        }
        .param-table td {
            padding: 12px;
            border-bottom: 1px solid #dde3ed;
        }
        .param-table tr:last-child td {
            border-bottom: none;
        }
        .param-table td:first-child {
            font-weight: 600;
            width: 35%;
            color: #1e3a6b;
        }
        .button-outline {
            display: inline-block;
            background-color: transparent;
            border: 1.5px solid #2A5CAA;
            color: #2A5CAA;
            padding: 10px 22px;
            border-radius: 50px;
            font-weight: 600;
            font-size: 0.95rem;
            text-decoration: none;
            transition: all 0.2s;
            margin-top: 10px;
        }
        .button-outline i {
            margin-right: 6px;
        }
        .button-outline:hover {
            background-color: #eef3ff;
        }
        .footer-links {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-top: 30px;
            padding-top: 16px;
            border-top: 1px solid #dce3ef;
            font-size: 0.9rem;
        }
        .footer-links a {
            color: #2A5CAA;
            text-decoration: none;
            font-weight: 500;
        }
        .footer-links a:hover {
            text-decoration: underline;
        }
        .disclaimer {
            font-size: 0.75rem;
            color: #7a89a6;
            text-align: center;
            margin-top: 12px;
        }
        .emph-blue {
            color: #2A5CAA;
            font-weight: 600;
        }
    </style>
</head>
<body>
    <div class="case-container">
        <!-- 头部：模块标识 + 二维码占位 -->
        <div class="case-header">
            <div class="case-meta">
                <span class="module-badge">模块四 · 新兴风险治理</span>
                <span class="case-number">案例 20</span>
            </div>
            <div class="qr-placeholder" title="部署后生成实际二维码">
                <i class="fas fa-qrcode"></i>
                <span>扫码看案例</span>
            </div>
        </div>

        <!-- 案例标题 -->
        <h1>平台“算法合谋”反垄断调查案</h1>
        <div class="subtitle">
            <i class="fas fa-map-pin" style="margin-right: 6px;"></i>深圳 · 人工智能企业 · 2024
        </div>

        <!-- 案例情境卡片 -->
        <div class="section-title">
            <i class="fas fa-briefcase"></i> 案例情境
        </div>
        <div class="card">
            <p>某头部电商平台（“智购科技”）利用其定价算法实时抓取竞争对手价格，并通过机器学习自动调整自身售价。在长达8个月的时间内，该平台与另外两家主要竞争者的价格始终保持高度同步，且均高于完全竞争市场的预期水平。深圳市市场监督管理局接到举报后启动调查，初步发现三家企业虽无书面或口头协议，但其算法在相似定价策略驱动下形成了“默示共谋”，涉嫌违反《反垄断法》关于垄断协议的规定。该案成为国内首例聚焦算法合谋的反垄断调查，引发对数字经济时代竞争规制工具创新的广泛讨论。</p>
            <div class="tag-group">
                <span class="tag"><i class="fas-regular fa-hashtag" style="margin-right: 4px;"></i>算法合谋</span>
                <span class="tag"><i class="fas-regular fa-hashtag" style="margin-right: 4px;"></i>默示共谋</span>
                <span class="tag"><i class="fas-regular fa-hashtag" style="margin-right: 4px;"></i>平台经济</span>
                <span class="tag"><i class="fas-regular fa-hashtag" style="margin-right: 4px;"></i>价格平行行为</span>
            </div>
        </div>

        <!-- 经济法问题聚焦 -->
        <div class="section-title">
            <i class="fas fa-gavel"></i> 经济法问题聚焦
        </div>
        <div class="card">
            <ul class="law-list">
                <li><i class="fas fa-check-circle"></i> <span class="emph-blue">垄断协议认定边界：</span>算法驱动的平行定价行为是否构成《反垄断法》第十六条禁止的“其他协同行为”？如何证明“意思联络”要件？</li>
                <li><i class="fas fa-check-circle"></i> <span class="emph-blue">滥用市场支配地位：</span>若平台利用算法实施掠夺性定价或差别待遇，是否同时触犯《反垄断法》第二十二条？</li>
                <li><i class="fas fa-check-circle"></i> <span class="emph-blue">规制工具创新：</span>现行反垄断规则能否有效应对“算法黑箱”带来的取证挑战？是否需要引入算法审计、透明度义务等新型监管工具？</li>
            </ul>
            <p style="margin-top: 12px; background-color: #e9effa; padding: 10px; border-radius: 12px;"><i class="fas fa-book-open" style="margin-right: 6px;"></i><strong>关联法条：</strong>《反垄断法》第16、17、19条；《平台经济领域反垄断指南》第6条（协同行为）、第8条（算法共谋）。</p>
        </div>

        <!-- 经济学分析工具 -->
        <div class="section-title">
            <i class="fas fa-chart-line"></i> 经济学分析工具
        </div>
        <div class="card">
            <ul class="law-list">
                <li><i class="fas fa-calculator"></i> <span class="emph-blue">超级博弈论：</span>在无限次重复博弈中，算法可自动触发“以牙还牙”策略，导致隐性合谋成为均衡结果。学生可调整贴现因子模拟合谋稳定性。</li>
                <li><i class="fas fa-calculator"></i> <span class="emph-blue">价格平行行为检测：</span>通过计算企业间价格变动的相关系数、方差比等指标，识别非正常的同步定价模式。</li>
                <li><i class="fas fa-calculator"></i> <span class="emph-blue">机器学习可解释性分析：</span>运用LIME或SHAP方法解析算法定价的主要特征，判断是否存在刻意匹配竞争对手的行为。</li>
            </ul>
            <div style="background: #eef2f6; border-radius: 16px; padding: 15px; margin-top: 15px; text-align: center;">
                <i class="fas fa-sliders-h" style="color: #2A5CAA; margin-right: 6px;"></i>
                <strong>互动计算器（模拟）：</strong> 输入市场企业数量、折扣因子、价格监测频率 → 测算合谋稳定性指数 
                <div style="background: white; border-radius: 40px; padding: 10px 20px; margin-top: 12px; font-size: 0.9rem; color: #666;">
                    [此处嵌入动态参数输入，实际部署时可使用JavaScript实现]
                </div>
            </div>
        </div>

        <!-- 监管工具箱 -->
        <div class="section-title">
            <i class="fas fa-shield-alt"></i> 监管工具箱
        </div>
        <div class="card">
            <p><i class="fas fa-globe" style="color: #2A5CAA; width: 24px;"></i> <strong>国内实践：</strong> 深圳市监局已委托第三方机构对涉案算法进行技术审计，探索“算法透明度报告”制度，拟要求平台披露定价逻辑的主要特征。</p>
            <p style="margin-top: 12px;"><i class="fas fa-university" style="color: #2A5CAA;"></i> <strong>国际比较：</strong> 欧盟《数字市场法案》将“算法合谋”列入黑名单，监管机构可推定具有市场支配地位的守门人企业承担举证责任；美国FTC发布《算法共谋指南》，强调对信号行为的审查。</p>
        </div>

        <!-- 沙盘推演参数 -->
        <div class="section-title">
            <i class="fas fa-dice-d6"></i> 沙盘推演参数（供双通路暗线任务使用）
        </div>
        <div class="card" style="padding: 0; overflow: hidden;">
            <table class="param-table">
                <tr><th colspan="2" style="background: #d9e4f5;">初始市场条件</th></tr>
                <tr><td>企业数量</td><td>3 家 (A: 智购科技, B: 万川电商, C: 云商)</td></tr>
                <tr><td>边际成本</td><td>A: 12元, B: 13元, C: 12.5元</td></tr>
                <tr><td>初始价格</td><td>全部 24元</td></tr>
                <tr><td>需求弹性</td><td>-1.8</td></tr>
                <tr><th colspan="2">算法设定</th></tr>
                <tr><td>定价频率</td><td>每15分钟一次</td></tr>
                <tr><td>监测对手窗口</td><td>过去2小时价格</td></tr>
                <tr><td>触发策略</td><td>若对手降价超过2%，则在下一周期跟进降价1.5%</td></tr>
                <tr><th colspan="2">监管干预选项</th></tr>
                <tr><td>突击算法审计</td><td>可开启（发现违规概率40%）</td></tr>
                <tr><td>宽大制度适用</td><td>第一家主动报告企业豁免全部罚款</td></tr>
            </table>
        </div>
        <p style="font-size: 0.85rem; color: #5d6f8c; margin-top: 4px;"><i class="fas fa-info-circle"></i> 上述参数可导入沙盘模型进行分组博弈，记录各小组决策路径与市场结果。</p>

        <!-- 思政讨论题 -->
        <div class="section-title">
            <i class="fas fa-heart"></i> 思政思辨题
        </div>
        <div class="card">
            <ul class="think-list">
                <li><i class="fas fa-comment-dots"></i> 算法合谋通常缺乏“白纸黑字”的协议，但其市场效果与垄断协议无异。在“技术中立”与“企业责任”之间，你认为平台应承担怎样的伦理责任？</li>
                <li><i class="fas fa-comment-dots"></i> 如果你是被调查企业的合规官，面对业绩压力与法律风险，你会如何向董事会解释“坚持算法透明”的价值？</li>
                <li><i class="fas fa-comment-dots"></i> 粤港澳大湾区正在建设“数字湾区”，你认为如何在促进人工智能产业发展的同时，守住公平竞争、科技向善的底线？</li>
            </ul>
        </div>

        <!-- 延伸阅读 -->
        <div class="section-title">
            <i class="fas fa-file-alt"></i> 延伸阅读
        </div>
        <div class="card" style="padding: 16px;">
            <p><i class="fas fa-file-pdf" style="color: #d14d42; margin-right: 10px;"></i> 市场监管总局《关于平台经济领域的反垄断指南》2024年修订草案 (扫码下载)</p>
            <p><i class="fas fa-file-pdf" style="color: #d14d42; margin-right: 10px;"></i> Ezrachi & Stucke, “算法合谋：数字时代的新挑战” 《哈佛商业评论》中文版 2023.08</p>
            <p><i class="fas fa-external-link-alt" style="color: #2A5CAA;"></i> <a href="#" style="text-decoration: none; border-bottom: 1px dashed;">广东省市场监管局：人工智能产业竞争合规指引（征求意见稿）</a></p>
        </div>

        <!-- 底部链接 -->
        <div class="footer-links">
            <a href="#"><i class="fas fa-arrow-left"></i> 返回案例库首页</a>
            <a href="#">下一案例 <i class="fas fa-arrow-right"></i></a>
        </div>
        <div class="disclaimer">
            * 本案例库为教学用途，基于公开资料改编。实际监管以官方文书为准。
        </div>
    </div>

    <!-- 附加说明：如何生成二维码（仅供理解） -->
    <div style="max-width:720px; width:100%; font-size:0.8rem; color:#7c8aa5; background:#eef3fc; border-radius:40px; padding:14px 20px; text-align:center;">
        <i class="fas fa-code"></i> 部署提示：将本HTML上传至服务器或GitHub Pages，使用二维码生成器（如草料二维码）将页面URL转换为二维码，印制于教材/PPT即可。
    </div>
</body>
</html>
