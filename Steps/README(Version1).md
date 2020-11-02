# Daily Check List

## 2020.10.29. 목


-Title&Sub is edited.
  1) /www/thema/Basic/head.php 
~~~
			<div class="header-logo">
				<a href="<?php echo $at_href['home'];?>">
					Home
				</a>
				<span class="header-desc">
					하나님이 날 사랑하시네
				</span>
			</div>
~~~

## 2020.11.02. 월

-Title's anme colors(hover) are changed

  1)/www/thema/Basic/colorset/Basic/colorset.css
  
~~~

/* 20.11.02 화면 메인 로고--> color: #000 --> #A8F552 으로 변경함 */
.pc-header .header-logo a:hover { color:#A8F552; }


~~~

-Menus names are changed to '찬양' , '감사', '회개', '기도', '간증', '질문' 등

-Some of the main page are changed. (갤러리, 웹진, 이미지 배너 are commented)
  1)/www/thema/Basic/main/basic-main.php

~~~

			 <!-- 갤러리 시작 --> <!-- 갤러리 생략
			<div class="div-title-underbar">
				<a href="<?php echo G5_BBS_URL;?>/board.php?bo_table=basic">
					<span class="pull-right lightgray <?php echo $font;?>">+</span>
					<span class="div-title-underbar-bold border-<?php echo $line;?> <?php echo $font;?>">
						<b>Gallery</b>
					</span>
				</a>
			</div>
			<div class="widget-box">
				<?php echo apms_widget('basic-post-gallery', $wid.'-wm3', 'center=1'); ?>
			</div>-->
			<!-- 갤러리 끝 -->	

			<!-- 웹진 시작 --> <!-- 웹진 생략
			<div class="div-title-underbar">
				<a href="<?php echo G5_BBS_URL;?>/board.php?bo_table=basic">
					<span class="pull-right lightgray <?php echo $font;?>">+</span>
					<span class="div-title-underbar-bold border-<?php echo $line;?> <?php echo $font;?>">
						<b>Webzine</b>
					</span>
				</a>
			</div>
			<div class="widget-box">
				<?php echo apms_widget('basic-post-webzine', $wid.'-wm4', 'bold=1 date=1'); ?>
			</div> -->
			<!-- 웹진 끝 -->	

			<!-- 이미지 배너 시작 --> <!-- 이미지배너 생략
			<div class="widget-box widget-img">
				<a href="#배너이동주소">
					<img src="<?php echo THEMA_URL;?>/assets/img/banner.jpg">
				</a>
			</div> -->
			<!-- 이미지 배너 끝 --> 

~~~


