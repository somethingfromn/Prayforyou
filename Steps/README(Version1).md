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
