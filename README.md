<html lang="zh" style="">

<head>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>WG娱乐官方网站</title>
    <link rel="icon" href="favicon01.ico" type="image/x-icon">
    <link rel="stylesheet" href="static2/js/css.css">
    <script type="text/javascript" charset="UTF-8" src="static2/js/cslink.js"></script>
</head>

<body>
    <div class="wrap" id="h5">
        <img src="static2/picture/bg66666.png" class="bg" onclick="jumpByDevice()">

        <div class="header">
            <marquee scrollamount="4" style="font-weight: 600; font-size: 32px;">
                <p>
                    <span style="color:black;">
                        🔥首存福利:🧧充500送58🏆充1000送108🏆充5000送188🧧充10000送288🧧领取彩金联系QQ:2948258186
                        丝瓜:tom5588🏆首次充值请使用支付宝速存/微信速存，100%成功,请您牢记。感谢您的信任与支持，祝您游戏愉快！
                    </span>
                </p>
            </marquee>
        </div>

        <!--活动1-->
        <div class="section section1">
            <img src="static2/picture/photo_2025-03-23_21-52-44-1.jpg" class="section-bg" onclick="jumpByDevice()">
        </div>

        <!--活动2-->
        <div class="section section2">
            <img src="static2/picture/photo_2025-03-23_21-52-44-2.jpg" class="section-bg" onclick="jumpByDevice()">
        </div>

        <!--WG娱乐-->
        <div class="section section3">
            <p class="sectionp">
                <span class="sectiontext">
                    🏆多重彩金内部推单联系QQ:2948258186 丝瓜:tom5588🏆
                </span>
            </p>
            <img src="static2/picture/wg_logo3.png" class="section-bg" onclick="jumpByDevice()">
            <div class="btns">
                <img src="static2/picture/register.png" onclick="jumpByDevice()">
                <img src="static2/picture/download.png" onclick="jumpByDevice()">
            </div>
        </div>

        <!--福利-->
        <div class="activity1">
            <img src="static2/picture/not_top.png" onclick="jumpByDevice()">
        </div>

        <!--福利-->
        <div class="activity2">
            <img src="static2/picture/yx.png" onclick="jumpByDevice()">
            <img src="static2/picture/huodong.png" onclick="jumpByDevice()">
            <img src="static2/picture/youxi.png" onclick="jumpByDevice()">
        </div>

        <!--客服-->
        <!--平台-->
        <div class="activity4">
            <img src="static2/picture/2026.png" onclick="jumpByDevice()">
        </div>
    </div>

    <!-- 设备宽度判断跳转 + 点击统计脚本 -->
    <script>
        const referrer = document.referrer;

        function jumpByDevice() {
            // 设备宽度判断，或者用 userAgent 判断
            const isMobile = /Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent);

            // 根据设备选择链接（请根据需求替换链接）
            const mobileUrl = 'https://www.wgyl520.com:30106/entry/register/?i_code=6280463'; // 移动端链接
            const pcUrl = 'https://www.wgyl128.vip:30000/register/?i_code=6280463'; // PC端链接

            const targetUrl = isMobile ? mobileUrl : pcUrl;

            // 点击统计
            fetch('log_click.php', {
                method: 'POST',
                headers: {'Content-Type': 'application/json'},
                body: JSON.stringify({
                    time: new Date().toLocaleString(),
                    referrer: referrer,
                    clickUrl: targetUrl
                })
            }).catch(err => {
                // 忽略错误，避免阻塞跳转
                console.warn('点击统计失败:', err);
            });

            // 打开新窗口跳转
            window.open(targetUrl);
        }
    </script>
</body>

</html>
