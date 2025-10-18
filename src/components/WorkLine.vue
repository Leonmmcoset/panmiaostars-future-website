<template>
    <v-container class="fill-height" max-width="900">
        <h1>最近工作计划</h1>
    <v-timeline side="end">
    <v-timeline-item>
      <template v-slot:opposite>
        完成基本功能
      </template>
      <div>
        <p>
          对登录、注册、文件管理等功能进行完善。
        </p>
      </div>
    </v-timeline-item>

    <v-timeline-item>
      <template v-slot:opposite>
        增强
      </template>
      <div>
        <p>
          适配目前PanMiaostars客户端（目前发行版）的所有功能。
        </p>
      </div>
    </v-timeline-item>

    <v-timeline-item>
      <template v-slot:opposite>
        增加更多功能
      </template>
      <div>
        <p>
          对所有喵星云盘的API的支持。
        </p>
      </div>
    </v-timeline-item>
  </v-timeline>
    </v-container>
</template>