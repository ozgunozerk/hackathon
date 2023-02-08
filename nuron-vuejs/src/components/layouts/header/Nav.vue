<template>
  <ul class="mainmenu">
    <li
      v-for="(item, index) in navItems"
      :class="[
        item.hasDropdown ? 'has-droupdown has-menu-child-item' : '',
        item.megamenu ? 'with-megamenu' : '',
      ]"
      :key="`nav-item-${index}`"
    >
      <router-link :to="item.link" class="nav-link its_new">
        {{ item.title }}
      </router-link>
      <ul v-if="item.hasDropdown" class="submenu">
        <li
          v-for="(subMenuItem, subMenuIndex) in item.dropdownItems"
          :key="`sub-menu-item-${subMenuIndex}`"
        >
          <router-link :to="subMenuItem.link" :class="subMenuItem.class">
            {{ subMenuItem.title }}
            <i
              v-if="subMenuItem.class !== 'live-expo'"
              :class="`feather-${subMenuItem.icon}`"
            />
          </router-link>
        </li>
      </ul>
      <div v-if="item.megamenu" class="rn-megamenu">
        <div class="wrapper">
          <div class="row row--0">
            <div
              v-for="(megamenuItem, megamenuIndex) in item.megaMenuItems"
              :key="`mega-menu-item-${megamenuIndex}`"
              class="col-lg-3 single-mega-item"
            >
              <ul class="mega-menu-item">
                <li
                  v-for="(
                    megamenuSubItem, megamenuSubIndex
                  ) in megamenuItem.items"
                  :key="`mega-submenu-item-${megamenuSubIndex}`"
                >
                  <router-link :to="megamenuSubItem.link">
                    {{ megamenuSubItem.title }}
                    <i :class="`feather-${megamenuSubItem.icon}`" />
                  </router-link>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </li>
  </ul>
</template>

<script>
export default {
  name: 'Nav',
  data() {
    return {
      navItems: [
        {
          link: '/',
          title: 'Home',
          hasDropdown: false,
          megamenu: false,
        },
        {
          link: '/about',
          title: 'About',
          hasDropdown: false,
          megamenu: false,
        },
        {
          link: '/blog-col-two',
          title: 'Blog',
          hasDropdown: false,
          megamenu: false,
        },
        {
          link: '/contact',
          title: 'Contact',
          hasDropdown: false,
          megamenu: false,
        }
      ]
    }
  }
}
</script>
