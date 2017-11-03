<!DOCTYPE html>
<html>

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="device-width, initial-scale=1, maximum-scale=1,minimum-scale,user-scalable=no">
  <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
  <meta name="robots" content="all" />
  <meta name="robots" content="index,follow" />
  <link rel="stylesheet" href="https://cdn.bootcss.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u"
    crossorigin="anonymous">
  <title>VIP视频分享</title>
</head>

<body>
  <div class="container">
    <h1>Vip视频解析</h1>
    <div class="row">
      <div class="col-md-4">
        <div class="form-group">
          <div class="input-group">
            <span class="input-group-addon">接口</span>
            <select id="selectId" class="form-control">
              <option value="http://api.baiyug.cn/vip/index.php?url=" selected>超清</option>
              <option value="http://www.vipjiexi.com/yun.php?url=">接口1</option>
              <option value="http://api.1008net.com/v.php?url=">接口2</option>
              <option value="http://api.nepian.com/ckparse/?url=">接口3</option>
              <option value="http://player.jidiaose.com/supapi/iframe.php?v=">接口4</option>
              <option value="http://api.pucms.com/index.php?url=">接口5</option>
              <option value="http://api.wlzhan.com/sudu/?url=">接口6</option>
              <option value="http://www.0335haibo.com/yun.php?url=">接口7</option>
              <option value="http://yun.mt2t.com/yun?url=">接口8</option>
              <option value="http://y.mt2t.com/lines?url=">接口9</option>
              <option value="http://www.0335haibo.com/yun.php?url=">接口10</option>
              <option value="http://www.sfsft.com/video.php?url=">接口11</option>
              <option value="http://www.82190555.com/video.php?url=">接口12</option>
              <option value=" http://2.jx.72du.com/video.php?url=">接口13</option>
              <option value="http://www.97panda.com/kkflv/index.php?url=">接口14</option>
              <option value="http://jx.vgoodapi.com/jx.php?url=">接口15</option>
              <option value="http://www.dgua.xyz/webcloud/?url=">接口16</option>
              <option value="http://api.91exp.com/svip/?url=">接口17</option>
              <option value="http://vip.jlsprh.com/index.php?url=">接口18</option>
              <option value="http://api.xfsub.com/index.php?url=">接口19</option>
              <option value="http://jiexi.071811.cc/jx.php?url=">接口20</option>
              <option value="http://jiexi.92fz.cn/player/vip.php?url=">接口21</option>
              <option value="http://api.baiyug.cn/vip/index.php?url=">接口22</option>
              <option value="http://api.662820.com/xnflv/index.php?url=">接口23</option>
              <option value="http://www.82190555.com/index/qqvod.php?url=">接口24</option>
              <option value="http://yyygwz.com/index.php?url=">接口25</option>
              <option value="http://www.97panda.com/kkflv/index.php?url=">接口26</option>
              <option value="http://jx.api.163ren.com/vod.php?url=">接口27</option>
              <option value="http://lookxw.com/yingzi/?url=">接口28</option>
              <option value="http://www.0335haibo.com/tong.php?url=">接口29</option>
              <option value="http://www.wmxz.wang/video.php?url=">接口30</option>
              <option value="http://api.97kn.com/?url=">接口31</option>
              <option value="https://aikanapi.duapp.com/odflv105/index.php?url=">接口32</option>
              <option value="http://v.buy360.vip/wwcx/index.php?url=">接口33</option>
              <option value="http://api.lequgirl.com/?url">接口34</option>
              <option value="https://jxapi.nepian.com/ckparse/?url=">接口35</option>
              <option value="http://91k.co/play.php?url=">接口36</option>
              <option value="http://www.52jiexi.com/yun.php?url=">接口37</option>
              <option value="http://mt2t.com/yun?url=">接口38</option>
              <option value="http://000o.cc/jx/ty.php?url=">接口39</option>
              <option value="http://yyygwz.com/index.php?url=">接口40</option>
              <option value="http://vipjiexi.com/vip.php?url=">接口41</option>
              <option value="http://www.wmxz.wang/video.php?url=">接口42</option>
              <option value="http://jx.ck921.com/?url=">接口43</option>
              <option value="http://s1y2.com/?url=">接口44</option>
              <option value="http://www.ou522.cn/t2/1.php?url=">接口45</option>
              <option value="http://jx.xuanpianwang.com/parse?url=">接口46</option>
              <option value="https://apiv.ga/magnet/">接口47</option>
              <option value="http://jiexi.92fz.cn/player/vip.php?url=">接口48</option>
            </select>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="form-group">
          <input type="text" class="form-control" id="addressUrl" placeholder="播放地址">
        </div>
      </div>
      <div class="col-md-2">
        <div class="form-group">
          <div class="btn-group" role="group" aria-label="...">
            <button type="button" class="btn btn-success" id="played">播放</button>
          </div>
        </div>
      </div>
    </div>
    <div class="row" style="border:1px solid #eee;border-radius:5px;background-color:#eee">
      <div class="col-md-12">
        <iframe width="100%" height="540px" scrolling=no id="player" frameborder="0" allowtransparency="true" allowFullScreen="true">
        </iframe>
      </div>
    </div>
  </div>
  <div class="container" style="text-align:center;margin-top:25px;">
    <span class="copyright">Copyright © 2017 DSSSC VIP视频解析 powered
      <a href="https://dsssc.top" title="DSSSC的博客" target="_blank">DSSSC的博客</a>
    </span>
  </div>
  <script>
    window.onload = function () {
      var obj = document.getElementById("selectId");
      var url = document.getElementById("addressUrl");
      var videoObj = document.getElementById("player");
      document.getElementById('played').onclick = function () {
        if (obj.value && url.value) {
          videoObj.src = obj.value + url.value
        }
      }
    }
  </script>
</body>

</html>
