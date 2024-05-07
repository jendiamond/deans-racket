<script setup lang="ts">
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <div class="songs">
    <WelcomeItem>
      <template #icon>
        <SupportIcon />
      </template>
      <template #heading>Dean's Fun</template>
      Lyrics & Video
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <SupportIcon />
      </template>
      <template #heading>In Your Body</template>
      Lyrics in collaboration with Carla Denka
      Lyrics & Video
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <SupportIcon />
      </template>
      <template #heading>Exquisite Man</template>
      Lyrics in collaboration with Kevin Hanley
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <SupportIcon />
      </template>
      <template #heading>I Love your Nose</template>
      <p>Lyrics in collaboration with Michael Urban</p>
    </WelcomeItem>

    <WelcomeItem>
      <template #icon>
        <SupportIcon />
      </template>
      <template lass= "heading-item" #heading>Man Among Men</template>

      As an independent project, Vue relies on community backing for its sustainability. You can help
      us by
      <a href="https://vuejs.org/sponsor/" target="_blank" rel="noopener">becoming a sponsor</a>.
    </WelcomeItem>
      <RouterView />
<span class="divider">================</span>
  <nav>
    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/about">About</RouterLink>
  </nav>
  </div>
</template>

<style scoped>
.songs {
  background-color:#d935bb;
}

.heading-item {
  z-index: 20;
  color:rgb(240, 255, 255);
  font-size: 1.5rem;
}

.divider {
  font-size: 12px;
  color: white;
  display: flex;
  place-items: center;
  place-content: center;
  padding-top: 10px;;
}

nav {
  width: 100%;
  font-size: 16px;
  text-align: center;
  margin-top: .5rem;
  padding-bottom: 10px;
  z-index: 30;
}

nav a.router-link-exact-active {
  color: white;
  font-weight: 500;
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
  color: black;
  font-weight: 500;
}

nav a:first-of-type {
  border: 0;
}
</style>
