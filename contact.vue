<template>
  <body bgcolor="#CC9900">
    <table width="1238" height="530" border="0">
      <tr>
        <td width="23" rowspan="2">&nbsp;</td>
        <td height="119" colspan="2" bgcolor="#006600">
          <h1>
            <center>
              <font color="#FFFFFF">พรชัยอพาร์ตเมนต์</font>
            </center>
          </h1>
          <Date />
        </td>
        <td width="43" rowspan="2">&nbsp;</td>
      </tr>
      <tr>
        <td width="1007" bgcolor="#FFFFFF">
          <img src="images/map.gif">
        </td>
        <td width="190" bgcolor="#FFFF66">
          <ul>
            <li><a href="/home">หน้าแรก</a></li>
            <li><a href="/room">ห้องพัก&ราคา</a></li>
            <li><a herf="/guest">สมุดเยี่ยม</a></li>
            <li><a href="/contact">ติดต่อ</a></li>
          </ul>
          <div>
            <LoginForm />
          </div>
        </td>
      </tr>
    </table>
  </body>
</template>

<script setup>
import LoginForm from '/components/LoginForm.vue';
import Date from '/components/Date.vue';
</script>