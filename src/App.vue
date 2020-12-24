<template>
  <div id="app">
    <div id="bg">
      <img src="https://i.ibb.co/fDTcBnG/20171225193112-2144.jpg" alt="20171225193112-2144" border="0">
    </div>
    <div id="a">
      <img src="https://i.ibb.co/Fh8m87t/image-1.png" alt="image-1" border="0">
    </div>
    <div id="bg2">
      <img src="https://i.ibb.co/3s7Znh2/20171225193112-2145.jpg" alt="20171225193112-2145" border="0">
    </div>
    <router-view/>
    <ul class="drop-down-menu">
        <li><a href="#">。最新消息</a>
        </li>
        <li><a href="#">。招生</a>
          <ul>
            <li><a href="#">春之清華卓越獎學金</a>
            </li>
            <li><a href="#">招生Q&A</a>
            </li>
            <li><a href="#">招生資料</a>
            <ul>
              <li><a href="#">2020</a>
              <ul>
                <li><a href="#">錄取名單</a>
                </li>
                <li><a href="#">招生簡章</a>
                </li>
                <li><a href="#">報名資料繳交</a>
                </li>
                <li><a href="#">第二階段注意事項</a>
                </li>
              </ul>
              </li>
              <li><a href="#">2019</a>
              <ul>
                <li><a href="#">錄取名單</a>
                </li>
                <li><a href="#">招生簡章</a>
                </li>
                <li><a href="#">報名資料繳交</a>
                </li>
                <li><a href="#">第二階段注意事項</a>
                </li>
              </ul>
              </li>
              <li><a href="#">2018</a>
              <ul>
                <li><a href="#">錄取名單</a>
                </li>
                <li><a href="#">招生簡章</a>
                </li>
                <li><a href="#">報名資料繳交</a>
                </li>
                <li><a href="#">第二階段注意事項</a>
                </li>
              </ul>
              </li>
            </ul>
            </li>
          </ul>
        </li>
        <li><a href="#">。學士班</a>
        <ul>
          <li><a href="#">學士班FB粉絲專頁</a>
          </li>
          <li><a href="#">學士班簡介</a>
          </li>
          <li><a href="#">學士班課程</a>
          </li>
          <li><a href="#">國際交換</a>
          </li>
          <li><a href="#">藝術學院大樓</a>
          </li>
        </ul>
        </li>
        <li><a href="#">。師資</a>
        </li>
        <li><a href="#">。科藝賞析</a>
        <ul>
          <li><a href="#">數位文創作品</a>
          </li>
          <li><a href="#">互動藝術作品</a>
          </li>
          <li><a href="#">動力藝術作品</a>
          </li>
          <li><a href="#">聲音藝術作品</a>
          </li>
          <li><a href="#">科技表演藝術</a>
          </li>
        </ul>
        </li>
        <li><a href="#">。聯絡</a>
        </li>
    </ul>
  </div>
</template>

<style>
ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  ul.drop-down-menu {
    position: fixed;
    left: 532px;
    top: 117px;
    color: #1B263B;
    font-family: 'ABeeZee';
    font-size: 24px;
    z-index: 999;
  }

#bg {
  position: fixed;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  z-index: -999;
}

#bg img{
  min-height: 100%;
  width: 100%;
  opacity: 100%;
}

#a{
  position: fixed;
  top: 108px;
  left: 380px;
  z-index: 999;
}

#a img{
  width: 81px;
  height: 86px;
}

#bg2{
  position: fixed;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}

#bg2 img{
  height: 260px;
  width: 100%;
  opacity: 100%;
}

#b{
  position: fixed;
  top: 119px;
  left: 482px;
  z-index: 999;
}

#b img{
  width: 1128px;
  height: 61px;
}

#app {
  position: absolute;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

ul {
  margin: 1px;
  padding: 0;
  list-style: none;
  }

  ul.drop-down-menu {
    border: rgba(204, 204, 204, 0) 1px solid;
    display: inline-block;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 24px;
  }

    ul.drop-down-menu li {
        position: relative;
        white-space: nowrap;
        border-right: rgba(204, 204, 204, 0) 1px solid;
    }

    ul.drop-down-menu > li:last-child {
        border-right: none;
    }

    ul.drop-down-menu > li {
        float: left; /* 只有第一層是靠左對齊*/
    }

    ul.drop-down-menu a {
        background-color: #e0e1dde0;
        color: #1B263B;
        display: block;
        padding: 8px 40px;
        text-decoration: none;
        line-height: 40px;
    }

    ul.drop-down-menu a:hover { /* 滑鼠滑入按鈕變色*/
        background-color: #1b263bd5;
        color: #fff;
    }

    ul.drop-down-menu li:hover > a { /* 滑鼠移入次選單上層按鈕保持變色*/
        background-color: #1b263bd5;
        color: #fff;
    }

    ul.drop-down-menu ul {
        border: #ccc 1px solid;
        position: absolute;
        z-index: 99;
        left: -1px;
        top: 100%;
        min-width: 180px;
    }

    ul.drop-down-menu ul li {
        border-bottom: #ccc 1px solid;
    }

    ul.drop-down-menu ul li:last-child {
        border-bottom: none;
    }

    ul.drop-down-menu ul ul { /*第三層以後的選單出現位置與第二層不同*/
        z-index: 999;
        top: 0px;
        left: 100%;
    }

      ul.drop-down-menu ul { /*隱藏次選單*/
        display: none;
    }

    ul.drop-down-menu li:hover > ul { /* 滑鼠滑入展開次選單*/
        display: block;
    }
</style>
