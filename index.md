---
layout: home
---
<div class="jumbotron jumbotron bg-cover">
        <h1 class="display-3 diemthitext">Welcome to {{ site.title }}</h1>
        <p class="lead diemthitext">{{ site.description }}</p>

  </div>

   <div class="row marketing" style="display:block">
        <div>
          <h4><strong><i class="fas fa-question-circle"></i> Đây là gì?</strong></h4>
          <p>Chào mừng đến với cổng thông tin điện tử dành cho học sinh C4K60! Trang web này là công cụ để tra cứu dễ dàng các thông tin của lớp 11 Nga THPT Chuyên Hà Nam</p>
        </div>
<h4><strong><i class="fas fa-comment-dollar"></i> Nó có miễn phí không?</strong></h4>
<p>Tất nhiên rồi! Miễn phì từ nay và mãi mãi về sau! Tuy nhiên nếu bạn muốn ủng hộ người lập trình, bạn có thể donate một cốc cafe 1$ qua <a href="https://paypal.me/techup">PayPal</a> :)</p>

<!-- Modal -->
<div class="modal fade right" id="ScoreModal6" tabindex="-1" role="dialog" aria-labelledby="exampleModalPreviewLabel" aria-hidden="true">
  <div class="modal-dialog" role="document">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModalPreviewLabel"><i class="fas fa-sign-in-alt"></i> Đăng nhập tài khoản - {{ site.title }}</h5>
        <button type="button" class="close" data-dismiss="modal" aria-label="Đóng">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
      <div class="modal-body">
<div id="okta-login-container"></div>
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-dismiss="modal">Đóng</button>
      </div>
    </div>
  </div>
</div>
<h4><strong><i class="fas fa-bullhorn"></i> Thông báo lớp</strong></h4>
<div class="content list">
{% if site.posts.size == 0 %}
  <h5>Không có bài viết nào:)</h5>
{% else %}
{% for post in site.categories.thongbaolop %}
  <div class="list-item">
    <h2 class="list-post-title">
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
    </h2>
    <div class="list-post-date">
      <time><!-- Whitespace added for readability -->
{% assign m = post.date | date: "%-m" %}
{{ post.date | date: "%-d" }}
{% case m %}
            {% when  '1' %}Tháng Giêng
            {% when  '2' %}Tháng Hai
            {% when  '3' %}Tháng Ba
            {% when  '4' %}Tháng Tư
            {% when  '5' %}Tháng Năm
            {% when  '6' %}Tháng Sáu
            {% when  '7' %}Tháng Bảy
            {% when  '8' %}Tháng Tám
            {% when  '9' %}Tháng Chín
            {% when '10' %}Tháng Mười
            {% when '11' %}Tháng Mười Một
            {% when '12' %}Tháng Mười Hai
{% endcase %}
{{ post.date | date: "%Y" }}
</time>
    </div>
  </div>
{% endfor %}
{% endif %}
</div>
<br>
<!-- START CONTENT -->
<div id="content"><h4><strong><i class="fas fa-clipboard-check"></i> Những thay đổi</strong></h4>

<h5>Phiên bản 3.0</h5>
<p>Ngày phát hành: 21/07/2019</p>

<ul>
  <li>Ra mắt cổng thông tin điện tử 11 Chuyên Nga THPT Chuyên Biên Hoà phiên bản thứ ba trên GitHub.</li>
<li>Phiên bản cải tiến nay sử dụng Jekyll để tiện quản lý và phát triển.</li>
<li>Đã thêm tính năng tra cứu hồ sơ học sinh, bài tập về nhà, thông báo lớp và chat.</li>
<li>Đã thêm tính năng bình luận Facebook ở cuối mỗi bài viết trong mục thông báo lớp.</li>
<li>Đã thêm tính năng liên lạc trợ giúp ở góc dưới bên phải màn hình.</li>
<li>Đã cập nhật giao diện mới cho trang 404.</li>
</ul>

<h5>Phiên bản 2.0</h5>
<p>Ngày phát hành: 23/05/2019</p>

<ul>
  <li>Ra mắt cổng thông tin điện tử 10 Chuyên Nga THPT Chuyên Biên Hoà phiên bản thứ hai trên GitHub.</li>
<li>Phiên bản cải tiến nay đã nhanh hơn và gọn nhẹ hơn.</li>
<li>Đã thêm tính năng tra cứu thời khoá biểu và thư viện ảnh.</li>
</ul>

<h5>Phiên bản 1.0</h5>
<p>Ngày phát hành: 24/03/2019</p>

<ul>
  <li>Ra mắt cổng thông tin điện tử 10 Chuyên Nga THPT Chuyên Biên Hoà phiên bản đầu tiên trên Blogspot.com.</li>
<li>Mục đích ban đầu tạo ra để tra điểm thi học kỳ.</li>
</ul>

</div>
<!-- END CONTENT -->
</div>
<br>