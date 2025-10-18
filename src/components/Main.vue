<template>
  <v-container class="fill-height" max-width="900">
    <div>
      <v-img
        class="mb-4"
        height="150"
        src="@/assets/logo.png"
      />

      <div class="mb-8 text-center">
        <div class="text-body-2 font-weight-light mb-n1">欢迎来到</div>
        <h1 class="text-h2 font-weight-bold">PanMiaostars Future官网</h1>
      </div>

      <v-row>
        <v-col cols="12">
          <!-- <v-card
            class="py-4"
            color="surface-variant"
            image="https://cdn.vuetifyjs.com/docs/images/one/create/feature.png"
            prepend-icon="mdi-rocket-launch-outline"
            rounded="lg"
            variant="tonal"
          >
            <template #image>
              <v-img position="top right" />
            </template>

            <template #title>
              <h2 class="text-h5 font-weight-bold">
                Get started
              </h2>
            </template>

            <template #subtitle>
              <div class="text-subtitle-1">
                Change this page by updating <v-kbd>{{ `<HelloWorld />` }}</v-kbd> in <v-kbd>components/HelloWorld.vue</v-kbd>.
              </div>
            </template>
          </v-card> -->
        </v-col>

        <v-col v-for="link in links" :key="link.href" cols="6">
          <v-card
            append-icon="mdi-open-in-new"
            class="py-4"
            color="surface-variant"
            :href="link.href"
            :prepend-icon="link.icon"
            rel="noopener noreferrer"
            rounded="lg"
            :subtitle="link.subtitle"
            target="_blank"
            :title="link.title"
            variant="tonal"
          />
        </v-col>
      </v-row>

      <br/>
      <h1>贡献者</h1> 
        <v-card
    class="mx-auto"
    append-avatar="https://avatars.githubusercontent.com/u/152147508?v=4"
    width="400"
  >
    <template v-slot:title>
      <span class="font-weight-black">LeonMMcoset</span>
    </template>

    <v-card-text class="bg-surface-light pt-4">
      程序主要负责人
    </v-card-text>
  </v-card>
    </div>
  </v-container>
</template>

<script setup>
  const links = [
    {
      href: 'work',
      icon: 'mdi-text-box-outline',
      subtitle: '查看最近工作计划',
      title: '最近工作计划',
    },
    {
      href: 'https://pan.miaostars.com/',
      icon: 'mdi-text-box-outline',
      subtitle: '访问喵星云盘',
      title: '喵星云盘',
    },
  ]
</script>