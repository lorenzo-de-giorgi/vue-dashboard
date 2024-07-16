<template>
    <div class="sidebar">
        <h3 class="text-white"><strong>- Dashbool -</strong></h3>
        <div class="d-flex">
            <div class="img">
                <img src="https://www.w3schools.com/howto/img_avatar.png" alt="" class="ldg-img">
            </div>
            <div class="ms-4 text-white">
                <p>Welcome</p>
                <p id="ldg-name-sidebar"><strong>Mario Rossi</strong></p>
            </div>
        </div>
        <ul class="sidebar-menu">
            <li class="sidebar-item" v-for="item in menuItems" :key="item.id">
                <a :href="item.link">{{ item.name }}</a>
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: 'SidebarComponent',
        data() {
            return {
                menuItems: [
                    { id: 1, name: 'Home', link: '/' },
                    { id: 2, name: 'About', link: '/about' },
                    { id: 3, name: 'Services', link: '/services' },
                    { id: 4, name: 'Contact', link: '/contact' }
                ]
            }
        },
    }
</script>

<style lang="scss" scoped>
.sidebar {
  width: 250px;
  height: 100vh;
  background-color: #2c3e50;
  padding: 20px;
  box-shadow: 2px 0 5px rgba(0, 0, 0, 0.1);

  .sidebar-menu {
    list-style: none;
    padding: 0;

    .sidebar-item {
      margin: 15px 0;

      a {
        color: #ecf0f1;
        text-decoration: none;
        font-size: 18px;
        transition: color 0.3s;

        &:hover {
          color: #3498db;
        }
      }
    }
  }
}

.ldg-img{
    width: 55px;
    border-radius: 50%;
    border: 1.5px solid white;
}

#ldg-name-sidebar{
    margin-top: -15px;
}
</style>