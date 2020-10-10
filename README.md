# 1821051031
1821051031 Lý Thị Hiền - Bài thu hoạch Thiết kế Website

![alt text](screenshots/img1.png "Title")

*Cách để tạo 1 slide ảnh chạy sau mỗi 3s*
*Bạn có thể tham khảo javascript sau*

```javascipt
// Automatic Slideshow - change image every 3 seconds
        var myIndex = 0;
        carousel();
        
        function carousel() {
          var i;
          var x = document.getElementsByClassName("mySlides");
          for (i = 0; i < x.length; i++) {
             x[i].style.display = "none";
          }
          myIndex++;
          if (myIndex > x.length) {myIndex = 1}
          x[myIndex-1].style.display = "block";
          setTimeout(carousel, 3000);
        }