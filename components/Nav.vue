<template>
  <nav class="nav">
    <ul class="nav-menu">
      <li class="nav-menu-item">
        <NuxtLink to="/">Hakkımda</NuxtLink>
      </li>
      <li class="nav-menu-item">
        <NuxtLink to="/projects">Projeler</NuxtLink>
      </li>
      <li class="nav-menu-item">
        <NuxtLink to="/articles">Yazılar</NuxtLink>
      </li>
    </ul>
  </nav>
</template>

<style lang="scss">
.nav {
  display: inline-flex;
  align-items: center;
  margin-bottom: 50px;

  &-menu {
    display: inline-flex;
    align-items: center;

    &-item {
      display: inline-flex;
      align-items: center;
      margin-right: 14px;

      a {
        font-size: 14px;
        line-height: 17px;
        color: $base-white;

        &.router-link-active {
          font-weight: 500;
        }
      }

      &:last-child {
        margin-right: 0;
      }
    }
  }
}
</style>