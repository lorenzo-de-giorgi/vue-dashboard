<template>
    <div class="sidebar">
        <h3>Dashbool</h3>
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
</style>