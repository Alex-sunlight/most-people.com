<template>
  <div class="mp-header">
    <div class="left">
      <router-link to="/" class="active">
        <span>{{ $t('Survey') }}</span>
      </router-link>
      <router-link to="/notes">
        <span>{{ $t('Notes') }}</span>
      </router-link>
    </div>

    <div class="right">
      <router-link to="/people" :style="{ maxWidth: '118px' }">
        <span>{{ $t('ServePeople') }}</span>
      </router-link>
      <router-link to="/me" class="avatar">
        <img src="/avatar.jpeg" alt="avatar" />
      </router-link>
    </div>
  </div>
  <router-view class="mp-page" />
</template>

<script setup lang="ts">
const { availableLocales: locales, locale } = useI18n()

const toggleLocales = () => {
  locale.value = locales[(locales.indexOf(locale.value) + 1) % locales.length]
}
</script>

<style lang="scss">
#app {
  padding: 0 16px;

  > .mp-header {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;

    .left,
    .right {
      display: flex;
      align-items: center;
      a {
        cursor: pointer;
        padding: 20px 16px;
        height: 100%;
        display: flex;
        align-items: center;
        span {
          border-bottom: 2px dashed transparent;
        }

        &.router-link-active {
          span {
            color: var(--red);
            font-weight: bold;
            border-bottom-color: var(--red);
          }
        }
      }
    }

    .right {
      .avatar {
        display: flex;
        align-items: center;
        padding: 20px 16px;
        cursor: pointer;
        line-height: 32px;
        opacity: 0.9;
        img {
          width: 32px;
          height: 32px;
          box-shadow: 0px 0px 2px 0px rgba(0, 0, 0, 0.4);
          border-radius: 50%;
        }
        &:hover {
          opacity: 1;
        }
      }
    }
  }

  > .mp-page {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
}
</style>
