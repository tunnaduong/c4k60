---
layout: default
title: Sinh nhật sắp tới
permalink: /sinhnhat/
tc: active
snst: active
1fname: Dương Huyền Anh
1birthday-month: 08
1birthday-day: 27
2fname: Dương Tùng Anh
2birthday-month: 11
2birthday-day: 21
3fname: Ngô Phương Anh
3birthday-month: 06
3birthday-day: 30
4fname: Nguyễn Đạt Thái Dương
4birthday-month: 12
4birthday-day: 12
5fname: Nguyễn Đặng Hải
5birthday-month: 12
5birthday-day: 10
6fname: Nguyễn Anh Bảo Hân
6birthday-month: 12
6birthday-day: 11
7fname: Bùi Thu Hiền
7birthday-month: 11
7birthday-day: 10
8fname: Nguyễn Thuý Hiền
8birthday-month: 05
8birthday-day: 17
9fname: Phạm Thu Hiền
9birthday-month: 12
9birthday-day: 29
10fname: Hồ Trung Hiếu
10birthday-month: 01
10birthday-day: 21
11fname: Phạm Bảo Sơn Hoa
11birthday-month: 12
11birthday-day: 25
12fname: Dư Thanh Hoài
12birthday-month: 04
12birthday-day: 13
13fname: Lã Kim Huệ
13birthday-month: 12
13birthday-day: 23
14fname: Phạm Thị Thiên Hương
14birthday-month: 11
14birthday-day: 13
15fname: Nguyễn Quang Huy
15birthday-month: 12
15birthday-day: 16
16fname: Trần Thị Diệu Huyền
16birthday-month: 01
16birthday-day: 02
17fname: Nguyễn Minh Khôi
17birthday-month: 05
17birthday-day: 01
18fname: Lê Hoàng Tùng Lâm
18birthday-month: 09
18birthday-day: 02
19fname: Lê Kim Liên
19birthday-month: 05
19birthday-day: 18
20fname: Đinh Thuỳ Linh
20birthday-month: 02
20birthday-day: 25
21fname: Nguyễn Khánh Linh
21birthday-month: 12
21birthday-day: 13
22fname: Bùi Ngọc Lĩnh
22birthday-month: 01
22birthday-day: 19
23fname: Nguyễn Đức Mạnh
23birthday-month: 08
23birthday-day: 09
24fname: Đỗ Thảo Nguyên
24birthday-month: 04
24birthday-day: 13
25fname: Đào Thu Phương
25birthday-month: 08
25birthday-day: 06
26fname: Đỗ Hồng Quân
26birthday-month: 11
26birthday-day: 08
27fname: Vũ Minh Quang
27birthday-month: 04
27birthday-day: 28
28fname: Đan Thị Phương Thảo
28birthday-month: 10
28birthday-day: 07
29fname: Dương Phương Thảo
29birthday-month: 12
29birthday-day: 14
30fname: Nguyễn Minh Thư
30birthday-month: 08
30birthday-day: 19
31fname: Vũ Huyền Trang
31birthday-month: 12
31birthday-day: 21
32fname: Nguyễn Thị Ánh Tuyết
32birthday-month: 04
32birthday-day: 18
33fname: Trần Khánh Vân
33birthday-month: 11
33birthday-day: 25
34fname: Hà Gia Văn
34birthday-month: 11
34birthday-day: 16
---
<style>
.navbar-brand{
font-size: 2rem;
}
</style>
<script>
function daysUntilNext(month, day){
    var tday= new Date(), y= tday.getFullYear(), next= new Date(y, month-1, day);
    tday.setHours(0, 0, 0, 0);
    if(tday>next) next.setFullYear(y+1);
    return Math.round((next-tday)/8.64e7);
}
setTimeout(sortTable, 2); 
function sortTable() {
  var table, rows, switching, i, x, y, shouldSwitch;
  table = document.getElementById("myTable");
  switching = true;
  /*Make a loop that will continue until
  no switching has been done:*/
  while (switching) {
    //start by saying: no switching is done:
    switching = false;
    rows = table.rows;
    /*Loop through all table rows (except the
    first, which contains table headers):*/
    for (i = 0; i < (rows.length - 1); i++) {
      //start by saying there should be no switching:
      shouldSwitch = false;
      /*Get the two elements you want to compare,
      one from current row and one from the next:*/
      x = rows[i].getElementsByTagName("TD")[1];
      y = rows[i + 1].getElementsByTagName("TD")[1];
      //check if the two rows should switch place:
      if (Number(x.innerHTML) > Number(y.innerHTML)) {
        //if so, mark as a switch and break the loop:
        shouldSwitch = true;
        break;
      }
    }
    if (shouldSwitch) {
      /*If a switch has been marked, make the switch
      and mark that a switch has been done:*/
      rows[i].parentNode.insertBefore(rows[i + 1], rows[i]);
      switching = true;
    }
  }
}
//Dương Huyền Anh
var d1= daysUntilNext({{page.1birthday-month}}, {{page.1birthday-day}}); 
if(d1=== 0) {
var today1 = "Hôm nay là sinh nhật của {{page.1fname}} ({{page.1birthday-day}}/{{page.1birthday-month}}/2003)! Hãy gửi lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t1, 1);
}
else {
var dm1 = "Còn "+d1+" ngày nữa là đến sinh nhật của {{page.1fname}}"

}
 function b1() {
  document.getElementById("d1").innerHTML = d1;
}
function t1() {
  document.getElementById("today").innerHTML = today1;
document.getElementById("r1").style.display = "none";
}
setTimeout(b1, 1); 

//Dương Tùng Anh
var d2= daysUntilNext({{page.2birthday-month}}, {{page.2birthday-day}}); 
if(d2=== 0) {
var today2 = "Hôm nay là sinh nhật của {{page.2fname}} ({{page.2birthday-day}}/{{page.2birthday-month}}/2003)! Hãy gửi lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t2, 1);
}
else {
var dm2 = "Còn "+d2+" ngày nữa là đến sinh nhật của {{page.2fname}}"

}
 function b2() {
  document.getElementById("d2").innerHTML = d2;
}
function t2() {
  document.getElementById("today").innerHTML = today2;
document.getElementById("r2").style.display = "none";
}
setTimeout(b2, 1); 

//Ngô Phương Anh
var d3= daysUntilNext({{page.3birthday-month}}, {{page.3birthday-day}}); 
if(d3=== 0) {
var today3 = "Hôm nay là sinh nhật của {{page.3fname}} ({{page.3birthday-day}}/{{page.3birthday-month}}/2003)! Hãy gửi lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t3, 1);
}
else {
var dm3 = "Còn "+d3+" ngày nữa là đến sinh nhật của {{page.3fname}}"

}
 function b3() {
  document.getElementById("d3").innerHTML = d3;
}
function t3() {
  document.getElementById("today").innerHTML = today3;
document.getElementById("r3").style.display = "none";
}
setTimeout(b3, 1); 

//Nguyễn Đạt Thái Dương
var d4= daysUntilNext({{page.4birthday-month}}, {{page.4birthday-day}}); 
if(d4=== 0) {
var today4 = "Hôm nay là sinh nhật của {{page.4fname}} ({{page.4birthday-day}}/{{page.4birthday-month}}/2003)! Hãy gửi lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t4, 1);
}
else {
var dm4 = "Còn "+d4+" ngày nữa là đến sinh nhật của {{page.4fname}}"

}
 function b4() {
  document.getElementById("d4").innerHTML = d4;
}
function t4() {
  document.getElementById("today").innerHTML = today4;
document.getElementById("r4").style.display = "none";
}
setTimeout(b4, 1); 

//Nguyễn Đặng Hải
var d5= daysUntilNext({{page.5birthday-month}}, {{page.5birthday-day}}); 
if(d5=== 0) {
var today5 = "Hôm nay là sinh nhật của {{page.5fname}} ({{page.5birthday-day}}/{{page.5birthday-month}}/2003)! Hãy gửi lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t5, 1);
}
else {
var dm5 = "Còn "+d5+" ngày nữa là đến sinh nhật của {{page.5fname}}"

}
 function b5() {
  document.getElementById("d5").innerHTML = d5;
}
function t5() {
  document.getElementById("today").innerHTML = today5;
document.getElementById("r5").style.display = "none";
}
setTimeout(b5, 1); 

//Dương Huyền Anh
var d6= daysUntilNext({{page.6birthday-month}}, {{page.6birthday-day}}); 
if(d6=== 0) {
var today6 = "Hôm nay là sinh nhật của {{page.6fname}} ({{page.30birthday-day}}/{{page.30birthday-month}}/2003)! Hãy gửi lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t6, 1);
}
else {
var dm6 = "Còn "+d6+" ngày nữa là đến sinh nhật của {{page.6fname}}"

}
 function b6() {
  document.getElementById("d6").innerHTML = d6;
}
function t6() {
  document.getElementById("today").innerHTML = today6;
document.getElementById("r6").style.display = "none";
}
setTimeout(b6, 1); 

//Dương Tùng Anh
var d7= daysUntilNext({{page.7birthday-month}}, {{page.7birthday-day}}); 
if(d7=== 0) {
var today7 = "Hôm nay là sinh nhật của {{page.7fname}} ({{page.7birthday-day}}/{{page.7birthday-month}}/2003)! Hãy gửi lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t7, 1);
}
else {
var dm7 = "Còn "+d7+" ngày nữa là đến sinh nhật của {{page.7fname}}"

}
 function b7() {
  document.getElementById("d7").innerHTML = d7;
}
function t7() {
  document.getElementById("today").innerHTML = today7;
document.getElementById("r7").style.display = "none";
}
setTimeout(b7, 1); 

//Ngô Phương Anh
var d8= daysUntilNext({{page.8birthday-month}}, {{page.8birthday-day}}); 
if(d8=== 0) {
var today8 = "Hôm nay là sinh nhật của {{page.8fname}} ({{page.8birthday-day}}/{{page.8birthday-month}}/2003)! Hãy gửi lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t8, 1);
}
else {
var dm8 = "Còn "+d8+" ngày nữa là đến sinh nhật của {{page.3fname}}"

}
 function b8() {
  document.getElementById("d8").innerHTML = d8;
}
function t8() {
  document.getElementById("today").innerHTML = today8;
document.getElementById("r8").style.display = "none";
}
setTimeout(b8, 1); 

//Nguyễn Đạt Thái Dương
var d9= daysUntilNext({{page.9birthday-month}}, {{page.9birthday-day}}); 
if(d9=== 0) {
var today9 = "Hôm nay là sinh nhật của {{page.9fname}} ({{page.9birthday-day}}/{{page.9birthday-month}}/2003)! Hãy gửi lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t9, 1);
}
else {
var dm9 = "Còn "+d9+" ngày nữa là đến sinh nhật của {{page.9fname}}"

}
 function b9() {
  document.getElementById("d9").innerHTML = d9;
}
function t9() {
  document.getElementById("today").innerHTML = today9;
document.getElementById("r9").style.display = "none";
}
setTimeout(b9, 1); 

//Nguyễn Đặng Hải
var d10= daysUntilNext({{page.10birthday-month}}, {{page.10birthday-day}}); 
if(d10=== 0) {
var today10 = "Hôm nay là sinh nhật của {{page.10fname}} ({{page.10birthday-day}}/{{page.6birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t10, 1);
}
else {
var dm10 = "Còn "+d10+" ngày nữa là đến sinh nhật của {{page.10fname}}"

}
 function b10() {
  document.getElementById("d10").innerHTML = d10;
}
function t10() {
  document.getElementById("today").innerHTML = today10;
document.getElementById("r10").style.display = "none";
}
setTimeout(b10, 1); 

//Nguyễn Anh Bảo Hân
var d11= daysUntilNext({{page.11birthday-month}}, {{page.11birthday-day}}); 
if(d11=== 0) {
var today11 = "Hôm nay là sinh nhật của {{page.11fname}} ({{page.11birthday-day}}/{{page.11birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t11, 1);
}
else {
var dm11 = "Còn "+d11+" ngày nữa là đến sinh nhật của {{page.11fname}}"

}
 function b11() {
  document.getElementById("d11").innerHTML = d11;
}
function t11() {
  document.getElementById("today").innerHTML = today11;
document.getElementById("r11").style.display = "none";
}
setTimeout(b11, 1); 
//Bùi Thu Hiền
var d12= daysUntilNext({{page.12birthday-month}}, {{page.12birthday-day}}); 
if(d12=== 0) {
var today12 = "Hôm nay là sinh nhật của {{page.12fname}} ({{page.12birthday-day}}/{{page.12birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t12, 1);
}
else {
var dm12 = "Còn "+d12+" ngày nữa là đến sinh nhật của {{page.12fname}}"

}
 function b12() {
  document.getElementById("d12").innerHTML = d12;
}
function t12() {
  document.getElementById("today").innerHTML = today12;
document.getElementById("r12").style.display = "none";
}
setTimeout(b12, 1); 
//NguyenThuyHien
var d13= daysUntilNext({{page.13birthday-month}}, {{page.13birthday-day}}); 
if(d13=== 0) {
var today13 = "Hôm nay là sinh nhật của {{page.13fname}} ({{page.13birthday-day}}/{{page.13birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t13, 1);
}
else {
var dm13 = "Còn "+d13+" ngày nữa là đến sinh nhật của {{page.13fname}}"

}
 function b13() {
  document.getElementById("d13").innerHTML = d13;
}
function t13() {
  document.getElementById("today").innerHTML = today13;
document.getElementById("r13").style.display = "none";
}
setTimeout(b13, 1); 
//Nguyễn Đặng Hải
var d14= daysUntilNext({{page.14birthday-month}}, {{page.14birthday-day}}); 
if(d14=== 0) {
var today14 = "Hôm nay là sinh nhật của {{page.14fname}} ({{page.14birthday-day}}/{{page.14birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t14, 1);
}
else {
var dm14 = "Còn "+d14+" ngày nữa là đến sinh nhật của {{page.14fname}}"

}
 function b14() {
  document.getElementById("d14").innerHTML = d14;
}
function t14() {
  document.getElementById("today").innerHTML = today14;
document.getElementById("r14").style.display = "none";
}
setTimeout(b14, 1); 
//Nguyễn Đặng Hải
var d15= daysUntilNext({{page.15birthday-month}}, {{page.15birthday-day}}); 
if(d15=== 0) {
var today15 = "Hôm nay là sinh nhật của {{page.15fname}} ({{page.15birthday-day}}/{{page.15birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t15, 1);
}
else {
var dm15 = "Còn "+d15+" ngày nữa là đến sinh nhật của {{page.15fname}}"

}
 function b15() {
  document.getElementById("d15").innerHTML = d15;
}
function t15() {
  document.getElementById("today").innerHTML = today15;
document.getElementById("r15").style.display = "none";
}
setTimeout(b15, 1); 
//Nguyễn Đặng Hải
var d16= daysUntilNext({{page.16birthday-month}}, {{page.16birthday-day}}); 
if(d16=== 0) {
var today16 = "Hôm nay là sinh nhật của {{page.16fname}} ({{page.16birthday-day}}/{{page.16birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t16, 1);
}
else {
var dm16 = "Còn "+d16+" ngày nữa là đến sinh nhật của {{page.16fname}}"

}
 function b16() {
  document.getElementById("d16").innerHTML = d16;
}
function t16() {
  document.getElementById("today").innerHTML = today16;
document.getElementById("r16").style.display = "none";
}
setTimeout(b16, 1); 
//Nguyễn Đặng Hải
var d17= daysUntilNext({{page.17birthday-month}}, {{page.17birthday-day}}); 
if(d17=== 0) {
var today17 = "Hôm nay là sinh nhật của {{page.17fname}} ({{page.17birthday-day}}/{{page.17birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t17, 1);
}
else {
var dm17 = "Còn "+d17+" ngày nữa là đến sinh nhật của {{page.17fname}}"

}
 function b17() {
  document.getElementById("d17").innerHTML = d17;
}
function t17() {
  document.getElementById("today").innerHTML = today17;
document.getElementById("r17").style.display = "none";
}
setTimeout(b17, 1); 
//Nguyễn Đặng Hải
var d18= daysUntilNext({{page.18birthday-month}}, {{page.18birthday-day}}); 
if(d18=== 0) {
var today18 = "Hôm nay là sinh nhật của {{page.18fname}} ({{page.18birthday-day}}/{{page.18birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t18, 1);
}
else {
var dm18 = "Còn "+d18+" ngày nữa là đến sinh nhật của {{page.18fname}}"

}
 function b18() {
  document.getElementById("d18").innerHTML = d18;
}
function t18() {
  document.getElementById("today").innerHTML = today18;
document.getElementById("r18").style.display = "none";
}
setTimeout(b18, 1); 
//Nguyễn Đặng Hải
var d19= daysUntilNext({{page.19birthday-month}}, {{page.19birthday-day}}); 
if(d19=== 0) {
var today19 = "Hôm nay là sinh nhật của {{page.19fname}} ({{page.19birthday-day}}/{{page.19birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t19, 1);
}
else {
var dm19 = "Còn "+d19+" ngày nữa là đến sinh nhật của {{page.19fname}}"

}
 function b19() {
  document.getElementById("d19").innerHTML = d19;
}
function t19() {
  document.getElementById("today").innerHTML = today19;
document.getElementById("r19").style.display = "none";
}
setTimeout(b19, 1); 
//Nguyễn Đặng Hải
var d20= daysUntilNext({{page.20birthday-month}}, {{page.20birthday-day}}); 
if(d20=== 0) {
var today20 = "Hôm nay là sinh nhật của {{page.20fname}} ({{page.30birthday-day}}/{{page.30birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t20, 1);
}
else {
var dm20 = "Còn "+d20+" ngày nữa là đến sinh nhật của {{page.20fname}}"

}
 function b20() {
  document.getElementById("d20").innerHTML = d20;
}
function t20() {
  document.getElementById("today").innerHTML = today20;
document.getElementById("r20").style.display = "none";
}
setTimeout(b20, 1); 

//Nguyễn Đặng Hải
var d21= daysUntilNext({{page.21birthday-month}}, {{page.21birthday-day}}); 
if(d21=== 0) {
var today21 = "Hôm nay là sinh nhật của {{page.21fname}} ({{page.21birthday-day}}/{{page.21birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t21, 1);
}
else {
var dm21 = "Còn "+d21+" ngày nữa là đến sinh nhật của {{page.21fname}}"

}
 function b21() {
  document.getElementById("d21").innerHTML = d21;
}
function t21() {
  document.getElementById("today").innerHTML = today21;
document.getElementById("r21").style.display = "none";
}
setTimeout(b21, 1); 
//Nguyễn Đặng Hải
var d22= daysUntilNext({{page.22birthday-month}}, {{page.22birthday-day}}); 
if(d22=== 0) {
var today22 = "Hôm nay là sinh nhật của {{page.22fname}} ({{page.22birthday-day}}/{{page.22birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t22, 1);
}
else {
var dm22 = "Còn "+d22+" ngày nữa là đến sinh nhật của {{page.22fname}}"

}
 function b22() {
  document.getElementById("d22").innerHTML = d22;
}
function t22() {
  document.getElementById("today").innerHTML = today22;
document.getElementById("r22").style.display = "none";
}
setTimeout(b22, 1); 
//Nguyễn Đặng Hải
var d23= daysUntilNext({{page.23birthday-month}}, {{page.23birthday-day}}); 
if(d23=== 0) {
var today23 = "Hôm nay là sinh nhật của {{page.23fname}} ({{page.23birthday-day}}/{{page.23birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t23, 1);
}
else {
var dm23 = "Còn "+d23+" ngày nữa là đến sinh nhật của {{page.23fname}}"

}
 function b23() {
  document.getElementById("d23").innerHTML = d23;
}
function t23() {
  document.getElementById("today").innerHTML = today23;
document.getElementById("r23").style.display = "none";
}
setTimeout(b23, 1); 
//Nguyễn Đặng Hải
var d24= daysUntilNext({{page.24birthday-month}}, {{page.24birthday-day}}); 
if(d24=== 0) {
var today24 = "Hôm nay là sinh nhật của {{page.24fname}} ({{page.24birthday-day}}/{{page.24birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t24, 1);
}
else {
var dm24 = "Còn "+d24+" ngày nữa là đến sinh nhật của {{page.24fname}}"

}
 function b24() {
  document.getElementById("d24").innerHTML = d24;
}
function t24() {
  document.getElementById("today").innerHTML = today24;
document.getElementById("r24").style.display = "none";
}
setTimeout(b24, 1); 
//Nguyễn Đặng Hải
var d25= daysUntilNext({{page.25birthday-month}}, {{page.25birthday-day}}); 
if(d25=== 0) {
var today25 = "Hôm nay là sinh nhật của {{page.25fname}} ({{page.25birthday-day}}/{{page.25birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t25, 1);
}
else {
var dm25 = "Còn "+d25+" ngày nữa là đến sinh nhật của {{page.25fname}}"

}
 function b25() {
  document.getElementById("d25").innerHTML = d25;
}
function t25() {
  document.getElementById("today").innerHTML = today25;
document.getElementById("r25").style.display = "none";
}
setTimeout(b25, 1); 
//Nguyễn Đặng Hải
var d26= daysUntilNext({{page.26birthday-month}}, {{page.26birthday-day}}); 
if(d26=== 0) {
var today26 = "Hôm nay là sinh nhật của {{page.26fname}} ({{page.26birthday-day}}/{{page.26birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t26, 1);
}
else {
var dm26 = "Còn "+d26+" ngày nữa là đến sinh nhật của {{page.26fname}}"

}
 function b26() {
  document.getElementById("d26").innerHTML = d26;
}
function t26() {
  document.getElementById("today").innerHTML = today26;
document.getElementById("r26").style.display = "none";
}
setTimeout(b26, 1); 
//Nguyễn Đặng Hải
var d27= daysUntilNext({{page.27birthday-month}}, {{page.27birthday-day}}); 
if(d27=== 0) {
var today27 = "Hôm nay là sinh nhật của {{page.27fname}} ({{page.27birthday-day}}/{{page.27birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t27, 1);
}
else {
var dm27 = "Còn "+d27+" ngày nữa là đến sinh nhật của {{page.27fname}}"

}
 function b27() {
  document.getElementById("d27").innerHTML = d27;
}
function t27() {
  document.getElementById("today").innerHTML = today27;
document.getElementById("r27").style.display = "none";
}
setTimeout(b27, 1); 
//Nguyễn Đặng Hải
var d28= daysUntilNext({{page.28birthday-month}}, {{page.28birthday-day}}); 
if(d28=== 0) {
var today28 = "Hôm nay là sinh nhật của {{page.28fname}} ({{page.28birthday-day}}/{{page.28birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t28, 1);
}
else {
var dm28 = "Còn "+d28+" ngày nữa là đến sinh nhật của {{page.28fname}}"

}
 function b28() {
  document.getElementById("d28").innerHTML = d28;
}
function t28() {
  document.getElementById("today").innerHTML = today28;
document.getElementById("r28").style.display = "none";
}
setTimeout(b28, 1); 
//Nguyễn Đặng Hải
var d29= daysUntilNext({{page.29birthday-month}}, {{page.29birthday-day}}); 
if(d29=== 0) {
var today29 = "Hôm nay là sinh nhật của {{page.29fname}} ({{page.29birthday-day}}/{{page.29birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t29, 1);
}
else {
var dm29 = "Còn "+d29+" ngày nữa là đến sinh nhật của {{page.29fname}}"

}
 function b29() {
  document.getElementById("d29").innerHTML = d29;
}
function t29() {
  document.getElementById("today").innerHTML = today29;
document.getElementById("r29").style.display = "none";
}
setTimeout(b29, 1); 
//Nguyễn Đặng Hải
var d30= daysUntilNext({{page.30birthday-month}}, {{page.30birthday-day}}); 
if(d30=== 0) {
var today30 = "Hôm nay là sinh nhật của {{page.30fname}} ({{page.30birthday-day}}/{{page.30birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t30, 1);
}
else {
var dm30 = "Còn "+d30+" ngày nữa là đến sinh nhật của {{page.30fname}}"

}
 function b30() {
  document.getElementById("d30").innerHTML = d30;
}
function t30() {
  document.getElementById("today").innerHTML = today30;
document.getElementById("r30").style.display = "none";
}
setTimeout(b30, 1); 
//Nguyễn Đặng Hải
var d31= daysUntilNext({{page.31birthday-month}}, {{page.31birthday-day}}); 
if(d31=== 0) {
var today31 = "Hôm nay là sinh nhật của {{page.31fname}} ({{page.31birthday-day}}/{{page.31birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t31, 1);
}
else {
var dm31 = "Còn "+d31+" ngày nữa là đến sinh nhật của {{page.31fname}}"

}
 function b31() {
  document.getElementById("d31").innerHTML = d31;
}
function t31() {
  document.getElementById("today").innerHTML = today31;
document.getElementById("r31").style.display = "none";
}
setTimeout(b31, 1); 
//Nguyễn Đặng Hải
var d32= daysUntilNext({{page.32birthday-month}}, {{page.32birthday-day}}); 
if(d32=== 0) {
var today32 = "Hôm nay là sinh nhật của {{page.32fname}} ({{page.32birthday-day}}/{{page.32birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t32, 1);
}
else {
var dm32 = "Còn "+d32+" ngày nữa là đến sinh nhật của {{page.32fname}}"

}
 function b32() {
  document.getElementById("d32").innerHTML = d32;
}
function t32() {
  document.getElementById("today").innerHTML = today32;
document.getElementById("r32").style.display = "none";
}
setTimeout(b32, 1); 
//Nguyễn Đặng Hải
var d33= daysUntilNext({{page.33birthday-month}}, {{page.33birthday-day}}); 
if(d33=== 0) {
var today33 = "Hôm nay là sinh nhật của {{page.33fname}} ({{page.33birthday-day}}/{{page.33birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t33, 1);
}
else {
var dm33 = "Còn "+d33+" ngày nữa là đến sinh nhật của {{page.33fname}}"

}
 function b33() {
  document.getElementById("d33").innerHTML = d33;
}
function t33() {
  document.getElementById("today").innerHTML = today33;
document.getElementById("r33").style.display = "none";
}
setTimeout(b33, 1); 
//Nguyễn Đặng Hải
var d34= daysUntilNext({{page.34birthday-month}}, {{page.34birthday-day}}); 
if(d34=== 0) {
var today34 = "Hôm nay là sinh nhật của {{page.34fname}} ({{page.34birthday-day}}/{{page.34birthday-month}}/2003)! lời chúc mừng sinh nhật bạn ấy!"
setTimeout(t34, 1);
}
else {
var dm34 = "Còn "+d34+" ngày nữa là đến sinh nhật của {{page.34fname}}"

}
 function b34() {
  document.getElementById("d34").innerHTML = d34;
}
function t34() {
  document.getElementById("today").innerHTML = today34;
document.getElementById("r34").style.display = "none";
}
setTimeout(b34, 1); 
</script>
<h3><i class="fas fa-birthday-cake"></i> Tra cứu sinh nhật</h3>
<h5><strong id="today">Hôm nay không có sinh nhật nào diễn ra...</strong></h5>
<table id="myTable">
  <tr id="r1" style="display: ">
<td>Còn</td>
    <td id="d1">5</td>
    <td>ngày nữa là đến sinh nhật của {{page.1fname}} ({{page.1birthday-day}}/{{page.1birthday-month}}/2003)</td>
  </tr>
  <tr id="r2" style="display: ">
<td>Còn</td>
    <td id="d2">3</td>
    <td>ngày nữa là đến sinh nhật của {{page.2fname}} ({{page.2birthday-day}}/{{page.2birthday-month}}/2003)</td>
  </tr>
 <tr id="r3" style="display: ">
<td>Còn</td>
<td id="d3">6</td>
<td>ngày nữa là đến sinh nhật của {{page.3fname}} ({{page.3birthday-day}}/{{page.3birthday-month}}/2003)</td>
  </tr>
  <tr id="r4" style="display: ">
<td>Còn</td>
<td id="d4">6</td>
<td>ngày nữa là đến sinh nhật của {{page.4fname}} ({{page.4birthday-day}}/{{page.4birthday-month}}/2003)</td>
  </tr>
  <tr id="r5" style="display: ">
<td>Còn</td>
<td id="d5">6</td>
<td>ngày nữa là đến sinh nhật của {{page.5fname}} ({{page.5birthday-day}}/{{page.5birthday-month}}/2003)</td>
  </tr>
  <tr id="r6" style="display: ">
<td>Còn</td>
    <td id="d6">5</td>
    <td>ngày nữa là đến sinh nhật của {{page.6fname}} ({{page.30birthday-day}}/{{page.30birthday-month}}/2003)</td>
  </tr>
  <tr id="r7" style="display: ">
<td>Còn</td>
    <td id="d7">3</td>
    <td>ngày nữa là đến sinh nhật của {{page.7fname}} ({{page.7birthday-day}}/{{page.7birthday-month}}/2003)</td>
  </tr>
 <tr id="r8" style="display: ">
<td>Còn</td>
<td id="d8">6</td>
<td>ngày nữa là đến sinh nhật của {{page.8fname}} ({{page.8birthday-day}}/{{page.8birthday-month}}/2003)</td>
  </tr>
  <tr id="r9" style="display: ">
<td>Còn</td>
<td id="d9">6</td>
<td>ngày nữa là đến sinh nhật của {{page.9fname}} ({{page.9birthday-day}}/{{page.9birthday-month}}/2003)</td>
  </tr>
  <tr id="r10" style="display: ">
<td>Còn</td>
<td id="d10">null</td>
<td>ngày nữa là đến sinh nhật của {{page.10fname}} ({{page.30birthday-day}}/{{page.30birthday-month}}/2003)</td>
  </tr>
  <tr id="r11" style="display: ">
<td>Còn</td>
<td id="d11">null</td>
<td>ngày nữa là đến sinh nhật của {{page.11fname}} ({{page.11birthday-day}}/{{page.11birthday-month}}/2003)</td>
  </tr>
  <tr id="r12" style="display: ">
<td>Còn</td>
<td id="d12">null</td>
<td>ngày nữa là đến sinh nhật của {{page.12fname}} ({{page.12birthday-day}}/{{page.12birthday-month}}/2003)</td>
  </tr>
  <tr id="r13" style="display: ">
<td>Còn</td>
<td id="d13">null</td>
<td>ngày nữa là đến sinh nhật của {{page.13fname}} ({{page.13birthday-day}}/{{page.13birthday-month}}/2003)</td>
  </tr>
  <tr id="r14" style="display: ">
<td>Còn</td>
<td id="d14">null</td>
<td>ngày nữa là đến sinh nhật của {{page.14fname}} ({{page.14birthday-day}}/{{page.14birthday-month}}/2003)</td>
  </tr>
  <tr id="r15" style="display: ">
<td>Còn</td>
<td id="d15">null</td>
<td>ngày nữa là đến sinh nhật của {{page.15fname}} ({{page.15birthday-day}}/{{page.15birthday-month}}/2003)</td>
  </tr>
  <tr id="r16" style="display: ">
<td>Còn</td>
<td id="d16">null</td>
<td>ngày nữa là đến sinh nhật của {{page.16fname}} ({{page.16birthday-day}}/{{page.16birthday-month}}/2003)</td>
  </tr>
  <tr id="r17" style="display: ">
<td>Còn</td>
<td id="d17">null</td>
<td>ngày nữa là đến sinh nhật của {{page.17fname}} ({{page.17birthday-day}}/{{page.17birthday-month}}/2003)</td>
  </tr>
  <tr id="r18" style="display: ">
<td>Còn</td>
<td id="d18">null</td>
<td>ngày nữa là đến sinh nhật của {{page.18fname}} ({{page.18birthday-day}}/{{page.18birthday-month}}/2003)</td>
  </tr>
  <tr id="r19" style="display: ">
<td>Còn</td>
<td id="d19">null</td>
<td>ngày nữa là đến sinh nhật của {{page.19fname}} ({{page.19birthday-day}}/{{page.19birthday-month}}/2003)</td>
  </tr>
  <tr id="r20" style="display: ">
<td>Còn</td>
<td id="d20">null</td>
<td>ngày nữa là đến sinh nhật của {{page.20fname}} ({{page.30birthday-day}}/{{page.30birthday-month}}/2003)</td>
  </tr>
  <tr id="r21" style="display: ">
<td>Còn</td>
<td id="d21">null</td>
<td>ngày nữa là đến sinh nhật của {{page.21fname}} ({{page.21birthday-day}}/{{page.21birthday-month}}/2003)</td>
  </tr>
  <tr id="r22" style="display: ">
<td>Còn</td>
<td id="d22">null</td>
<td>ngày nữa là đến sinh nhật của {{page.22fname}} ({{page.22birthday-day}}/{{page.22birthday-month}}/2003)</td>
  </tr>
  <tr id="r23" style="display: ">
<td>Còn</td>
<td id="d23">null</td>
<td>ngày nữa là đến sinh nhật của {{page.23fname}} ({{page.23birthday-day}}/{{page.23birthday-month}}/2003)</td>
  </tr>
  <tr id="r24" style="display: ">
<td>Còn</td>
<td id="d24">null</td>
<td>ngày nữa là đến sinh nhật của {{page.24fname}} ({{page.24birthday-day}}/{{page.24birthday-month}}/2003)</td>
  </tr>
  <tr id="r25" style="display: ">
<td>Còn</td>
<td id="d25">null</td>
<td>ngày nữa là đến sinh nhật của {{page.25fname}} ({{page.25birthday-day}}/{{page.25birthday-month}}/2003)</td>
  </tr>
  <tr id="r26" style="display: ">
<td>Còn</td>
<td id="d26">null</td>
<td>ngày nữa là đến sinh nhật của {{page.26fname}} ({{page.26birthday-day}}/{{page.26birthday-month}}/2003)</td>
  </tr>
  <tr id="r27" style="display: ">
<td>Còn</td>
<td id="d27">null</td>
<td>ngày nữa là đến sinh nhật của {{page.27fname}} ({{page.27birthday-day}}/{{page.27birthday-month}}/2003)</td>
  </tr>
  <tr id="r28" style="display: ">
<td>Còn</td>
<td id="d28">null</td>
<td>ngày nữa là đến sinh nhật của {{page.28fname}} ({{page.28birthday-day}}/{{page.28birthday-month}}/2003)</td>
  </tr>
  <tr id="r29" style="display: ">
<td>Còn</td>
<td id="d29">null</td>
<td>ngày nữa là đến sinh nhật của {{page.29fname}} ({{page.29birthday-day}}/{{page.29birthday-month}}/2003)</td>
  </tr>
  <tr id="r30" style="display: ">
<td>Còn</td>
<td id="d30">null</td>
<td>ngày nữa là đến sinh nhật của {{page.30fname}} ({{page.30birthday-day}}/{{page.30birthday-month}}/2003)</td>
  </tr>
  <tr id="r31" style="display: ">
<td>Còn</td>
<td id="d31">null</td>
<td>ngày nữa là đến sinh nhật của {{page.31fname}} ({{page.31birthday-day}}/{{page.31birthday-month}}/2003)</td>
  </tr>
  <tr id="r32" style="display: ">
<td>Còn</td>
<td id="d32">null</td>
<td>ngày nữa là đến sinh nhật của {{page.32fname}} ({{page.32birthday-day}}/{{page.32birthday-month}}/2003)</td>
  </tr>
  <tr id="r33" style="display: ">
<td>Còn</td>
<td id="d33">null</td>
<td>ngày nữa là đến sinh nhật của {{page.33fname}} ({{page.33birthday-day}}/{{page.33birthday-month}}/2003)</td>
  </tr>
  <tr id="r34" style="display: ">
<td>Còn</td>
<td id="d34">null</td>
<td>ngày nữa là đến sinh nhật của {{page.34fname}} ({{page.34birthday-day}}/{{page.34birthday-month}}/2003)</td>
  </tr>
</table>
<br>
