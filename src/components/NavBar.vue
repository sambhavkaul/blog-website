<template>
  <div id="navigation">
    <ul>
      <li>Home</li>
      <li>Articles</li>
      <li>Magazines</li>
      <li>Editors</li>
      <li>Readers</li>
    </ul>
    <div class="search">
      <input type="text" placeholder="Search for articles" />
      <i class="fas fa-search"></i>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavBar"
};
</script>

<style lang="scss" scoped>
#navigation {
  display: flex;
  width: 100%;
  margin-bottom: 50px;

  ul {
    display: flex;
    list-style: none;
    padding: 0;
    margin: 0 20px 0 0;
    li {
      font-size: 2rem;
      padding: 2px 10px;
      cursor: pointer;
    }
  }
  .search {
    position: relative;
    width: 100%;
    max-width: 400px;
    input {
      border: none;
      outline: none;
      width: calc(100% - 80px);
      padding: 15px 60px 15px 20px;
      margin: 0;
      border-radius: 20px;
      font-family: "Segoe UI", Tahoma;
      font-size: 1rem;
      float: right;
    }
    i {
      position: absolute;
      right: 20px;
      top: 15px;
      font-size: 1.6rem;
      cursor: pointer;
    }
  }
}
</style>