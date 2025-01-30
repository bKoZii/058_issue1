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
            <template v-for="link in navLinks" :key="link.name">
              <li>
                <a :href="link.url">{{ link.name }}</a>
              </li>
            </template>
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

const navLinks = [{
  name: 'หน้าแรก',
  url: '/home'
}, {
  name: 'ห้องพัก&ราคา',
  url: '/room'
}, {
  name: 'สมุดเยี่ยม',
  url: '/guest'
}, {
  name: 'ติดต่อ',
  url: '/contact'
}]
</script>