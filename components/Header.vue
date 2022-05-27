<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="danger">
      <b-navbar-brand to="/">남건의 뷰 게시판</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item to="/">home</b-nav-item>
          <b-nav-item to="/gallery">갤러리</b-nav-item>
          <b-nav-item to="/boardlist">리스트</b-nav-item>
          <b-nav-item to="/calvue">캘린더</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  nama: "Header",
  data() {
    return {

    }
  }
};
</script>
