---
title: Hamburger
date: 2018-12-08
layout: post
---

<style>
  .hamburger .hamburger__line{
      width: 20px;
      height: 2px;
      background-color: black;
      display: block;
      margin: 4px auto;
      -webkit-transition: all 0.3s ease-in-out;
      -o-transition: all 0.3s ease-in-out;
      transition: all 0.3s ease-in-out;
  }

  .hamburger:hover{
      cursor: pointer;
  }

  .hamburger.hamburger-active .hamburger__line:nth-child(2){
      opacity: 0;
  }

  .hamburger.hamburger-active .hamburger__line:nth-child(1){
      -webkit-transform: translateY(6px) rotate(45deg);
      -ms-transform: translateY(6px) rotate(45deg);
      -o-transform: translateY(6px) rotate(45deg);
      transform: translateY(6px) rotate(45deg);
  }

  .hamburger.hamburger-active .hamburger__line:nth-child(3){
      -webkit-transform: translateY(-6px) rotate(-45deg);
      -ms-transform: translateY(-6px) rotate(-45deg);
      -o-transform: translateY(-6px) rotate(-45deg);
      transform: translateY(-6px) rotate(-45deg);
  }
</style>

<div class="hamburger">
  <span class="hamburger__line"></span>
  <span class="hamburger__line"></span>
  <span class="hamburger__line"></span>
</div>

<script>
  $(document).ready(function(){
    $(".hamburger").click(function(){
      $(this).toggleClass("hamburger-active");
    });
  });
</script>

html
``` 
<div class="hamburger">
  <span class="hamburger__line"></span>
  <span class="hamburger__line"></span>
  <span class="hamburger__line"></span>
</div>
```
css
```
.hamburger .hamburger__line{
    width: 20px;
    height: 2px;
    background-color: black;
    display: block;
    margin: 4px auto;
    -webkit-transition: all 0.3s ease-in-out;
    -o-transition: all 0.3s ease-in-out;
    transition: all 0.3s ease-in-out;
}

.hamburger:hover{
    cursor: pointer;
}

.hamburger.hamburger-active .hamburger__line:nth-child(2){
    opacity: 0;
}

.hamburger.hamburger-active .hamburger__line:nth-child(1){
    -webkit-transform: translateY(6px) rotate(45deg);
    -ms-transform: translateY(6px) rotate(45deg);
    -o-transform: translateY(6px) rotate(45deg);
    transform: translateY(6px) rotate(45deg);
}

.hamburger.hamburger-active .hamburger__line:nth-child(3){
    -webkit-transform: translateY(-6px) rotate(-45deg);
    -ms-transform: translateY(-6px) rotate(-45deg);
    -o-transform: translateY(-6px) rotate(-45deg);
    transform: translateY(-6px) rotate(-45deg);
}
```
js
```
$(document).ready(function(){
  $(".hamburger").click(function(){
    $(this).toggleClass("hamburger-active");
  });
});
```

