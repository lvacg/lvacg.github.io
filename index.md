<html>
<head>
    <!--作者：小猫咪，背景js是从网上扒的，剩下的都是自己的，源码已开源禁止用于商业用途倒卖源码-->
    <!--小猫咪QQ：3503473416-->
    <!--头像替换在index.html第11行代码中的"3503473416"替换成你的qq号即可-->
	<title>小猫咪导航页</title>
	<link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
	<img src="https://q2.qlogo.cn/headimg_dl?dst_uin=3503473416&spec=100" class="logo">
    <p>小猫咪导航页</p>
    <HR style="border: 0.5px solid #888888" width="40%" size=1>
		<div class="sx"></div>
        <!--网站简介-->
        <p1>有钱终成眷属&nbsp;&nbsp;没钱亲眼目睹</p1>
        <!--菜单栏-->
	<a href="#" style="--clr:#1e9bff"><span>首页</span><i></i></a>
	<a href="#" style="--clr:#ff1867"><span>工具箱</span><i></i></a>
	<a href="#" style="--clr:#6eff3e"><span>敬请期待</span><i></i></a>
    <a href="#" style="--clr:#ff5511"><span>敬请期待</span><i></i></a>
    <a href="#" style="--clr:#ff00ff"><span>敬请期待</span><i></i></a>
	<script src="js/jquery-2.1.1.min.js" type="text/javascript"></script>
	<HR style="border: 0.5px solid #888888" width="30%" size=1>
	<a2 href="https://beian.miit.gov.cn/#/Integrated/index">冀ICP备:xxxxxx</a2>
    <a1>Copyright&nbsp;&nbsp;2021 - 2022&nbsp;&nbsp;小猫咪工作室版权所有</a1>
</body>
<script>
    ! function() {
        function n(n, e, t) {
            return n.getAttribute(e) || t
        }
 
        function e(n) {
            return document.getElementsByTagName(n)
        }
 
        function t() {
            var t = e("script"),
                o = t.length,
                i = t[o - 1];
            return {
                l: o,
                z: n(i, "zIndex", -1),
                o: n(i, "opacity", 1),
                c: n(i, "color", "220,220,220"),//控制线条的颜色的地方
                n: n(i, "count", 180)
            }
        }
 
        function o() {
            a = m.width = window.innerWidth || document.documentElement.clientWidth || document.body.clientWidth, c = m.height = window.innerHeight || document.documentElement.clientHeight || document.body.clientHeight
        }
 
        function i() {
            r.clearRect(0, 0, a, c);
            var n, e, t, o, m, l;
            s.forEach(function(i, x) {
                for(i.x += i.xa, i.y += i.ya, i.xa *= i.x > a || i.x < 0 ? -1 : 1, i.ya *= i.y > c || i.y < 0 ? -1 : 1, r.fillRect(i.x - .5, i.y - .5, 1, 1), e = x + 1; e < u.length; e++) n = u[e], null !== n.x && null !== n.y && (o = i.x - n.x, m = i.y - n.y, l = o * o + m * m, l < n.max && (n === y && l >= n.max / 2 && (i.x -= .03 * o, i.y -= .03 * m), t = (n.max - l) / n.max, r.beginPath(), r.lineWidth = t / 2, r.strokeStyle = "rgba(" + d.c + "," + (t + .2) + ")", r.moveTo(i.x, i.y), r.lineTo(n.x, n.y), r.stroke()))
            }), x(i)
        }
        var a, c, u, m = document.createElement("canvas"),
            d = t(),
            l = "c_n" + d.l,
            r = m.getContext("2d"),
            x = window.requestAnimationFrame || window.webkitRequestAnimationFrame || window.mozRequestAnimationFrame || window.oRequestAnimationFrame || window.msRequestAnimationFrame || function(n) {
                window.setTimeout(n, 1e3 / 45)
            },
            w = Math.random,
            y = {
                x: null,
                y: null,
                max: 2e4
            };
        m.id = l, m.style.cssText = "position:fixed;top:0;left:0;z-index:" + d.z + ";opacity:" + d.o, e("body")[0].appendChild(m), o(), window.onresize = o, window.onmousemove = function(n) {
            n = n || window.event, y.x = n.clientX, y.y = n.clientY
        }, window.onmouseout = function() {
            y.x = null, y.y = null
        };
        for(var s = [], f = 0; d.n > f; f++) {
            var h = w() * a,
                g = w() * c,
                v = 2 * w() - 1,
                p = 2 * w() - 1;
            s.push({
                x: h,
                y: g,
                xa: v,
                ya: p,
                max: 6e3
            })
        }
        u = s.concat([y]), setTimeout(function() {
            i()
        }, 100)
    }();
</script>
</html>
