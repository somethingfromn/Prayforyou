# Daily Check List

## 2020.05.05. 화

-Some Menus added.    
-Version 5.4 cant get along to comment adding functions 
-By this, all the files are out of controll.
-So I deleted everything and installed them again.

-(소스수정)  
  1) ~/skin/good.head.skin 추가 
~~~
 <?php
    $ss_name = 'ss_view_'.$bo_table.'_'.$wr_id;
    set_session($ss_name, true);
    $board['bo_use_good'] = true;
 ?>
~~~
  2) ~/board/basic/view_comment.skin.php의 69번째 라인 수정
~~~  
   <!--2020.05.05 댓글 비추천 추천 추가 { -->
            <div style="height:5px"></div>
            <ul class="bo_vc_act">
                <li>
                    <a class="btn_b03" href="<?php echo G5_BBS_URL.'/good_comment.php?bo_table='.$bo_table.'&wr_id='.$list[$i]['wr_id'].'&good=good';?>">
                    <i class="fa fa-thumbs-up"> </i><strong style="margin-left:10px"><?php echo number_format($list[$i]['wr_good']) ?> </strong>
                    <b id="bo_v_act_good" class="bo_v_act_good"></b>
                    </a>
                </li>
                <li>
                    <a class="btn_b03" href="<?php echo G5_BBS_URL.'/good_comment.php?bo_table='.$bo_table.'&wr_id='.$list[$i]['wr_id'].'&good=nogood';?>">
                    <i class="fa fa-thumbs-down"> </i><strong style="margin-left:10px"><?php echo number_format($list[$i]['wr_nogood']) ?> </strong>
                    <b id="bo_v_act_nogood" class="bo_v_act_nogood"></b>
                    </a>
                </li>
            </ul>
            <!--댓글 비추천 추가 끝 } -->
  ~~~

## 2020.05.06. 수

-5.4 Version of the Theme is not matched with these kind of websites.  
-Generally, 5.3 version of Gnuboard is perfect with comment recommnedation functions on the Q&A section on the Gnu.  
-I changed the 5.4 to 5.3 version! and added "good_comment.php" which is same as good.php into bbs with changing below codes.  

~~~
  //2020.05.05 아래 코드 생략.
   // $ss_name = 'ss_view_'.$bo_table.'_'.$wr_id;
    //if (!get_session($ss_name))
     //   alert('해당 게시물에서만 추천 또는 비추천 하실 수 있습니다.');
~~~


## 2020.05.07.목
### -What changed?   

(in Basic Setting on the websites)
 1. Added "Privay" and "Provision Policy" on the website.  
 2. "Website Subject" name changed. 
 3. "Getting Points" setting changed.  
 4. "The time for checking the number of Accessors" is changed.  
 5. "Prohibitive words for sing up" added some words on it.  
 6. "Privay for signu up" added. 
 7. "Mailing Service for sign up to Admin and User" added.
 
(in Soruce Files in the folder)  
 1. I finally figured where these "www/index.php, /tail.php, /head.php .." come from. The steps are like the same files in the "Theme" folder wirte same codes on same files in the "www" folder. so if you wanna change something, you gotta go to Theme folder and do something, and then the files you just modified write codes on the files in the "www" folder. and then, you could see the modification on the website as soon as you click the Refresh button.    
   
   1) /www/Theme/basic/tail.php
  ~~~
    <div id="ft_wr">
        <div id="ft_link">
            <a href="<?php echo G5_BBS_URL; ?>/content.php?co_id=company">회사소개</a>
            <a href="<?php echo G5_BBS_URL; ?>/content.php?co_id=privacy">개인정보처리방침</a>
            <a href="<?php echo G5_BBS_URL; ?>/content.php?co_id=provision">서비스이용약관</a>
            <a href="<?php echo get_device_change_url(); ?>">모바일버전</a>
        </div>
        <div id="ft_catch"><img src="<?php echo G5_IMG_URL; ?>/ft_logo.png" alt="<?php echo G5_VERSION ?>"></div>
	    <!-- 2020.05.07: "소유하신 도메인" -> "2020.05 Covid-19 in Korea." -->
        <div id="ft_copy">Copyright &copy; <b2020.05 Covid-19 in Korea.</b> All rights reserved.</div>
    </div>
   ~~~
    
  2. Need the size of logo image smaller!  
  
    1) /www/logo.png --> made the size of image smaller than now.  
    
## 2020.05.08.금
### -What changed?   
  

(in Basic Setting on the websites)
  1. 
  
(in Soruce Files in the folder) 
  1. also I changed mobile one in the mobile folder
    
    1)/www/Theme/basic/mobile/tail.php
    
    ~~~
    <div id="ft_copy">
        <div id="ft_company">
            <a href="<?php echo G5_BBS_URL; ?>/content.php?co_id=company">회사소개</a>
            <a href="<?php echo G5_BBS_URL; ?>/content.php?co_id=privacy">개인정보처리방침</a>
            <a href="<?php echo G5_BBS_URL; ?>/content.php?co_id=provision">서비스이용약관</a>
        </div>
	<!-- 2020.05.07: "소유하신 도메인" -> "2020.05 Covid-19 in Korea." -->
        Copyright &copy; <b>2020.05 Covid-19 in Korea.</b> All rights reserved.<br>
    </div>
    ~~~
    
    2. 
    
    
    
  

