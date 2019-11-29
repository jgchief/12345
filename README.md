<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title></title>
    <style>
      .slide {
        width:210px;
        border:2px solid #333;
        box-shadow:2px 2px 3px #000;
        float:left;
        margin-top:30;
        margin-right:20px;
      }
    </style>
    <script src="http://code.jquery.com/jquery-3.3.1.js"></script>
  </head>
  <body>
    <script>

      $(document).ready(function(){
        $("#sup").click(function(){
          $(".slide").slideUp(3000);
        });

        $("#sdown").click(function(){
          $(".slide").slideDown(3000);
        });

        $("#stoggle").click(function(){
          $(".slide").slideToggle(3000);
        });
      });

    </script>
    <form>
      <input type="button" id="sup" value="slideup">
      <input type="button" id="sdown" value="slidedown">
      <input type="button" id="stoggle" value="slidetoggle">
    </form>
    <div class="slide">
      <img src="dog2.jpg" width="200">
    </div>
    <div class="slide">
      <img src="dog3.jpg" width="200">
    </div>
    <div class="slide">
      <p width=200 height=140>겨울입니다</p>
    </div>


  </body>
</html>
