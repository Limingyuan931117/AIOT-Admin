<script setup lang="ts">
import { isEqual } from "@pureadmin/utils";
import { useRoute, useRouter } from "vue-router";
import { ref, watch, onMounted, toRaw } from "vue";
import { getParentPaths, findRouteByPath } from "@/router/utils";
import { useMultiTagsStoreHook } from "@/store/modules/multiTags";

const route = useRoute();
const levelList = ref([]);
const router = useRouter();
const routes: any = router.options.routes;
const multiTags: any = useMultiTagsStoreHook().multiTags;

const active = ref(0);

const appList = [
  {
    name: "IOT中台",
    url: "zhogntai",
    icon: "home",
    active_icon: "home_active"
  },
  {
    name: "门店信息",
    url: "zhogntai",
    icon: "home",
    active_icon: "home_active"
  },
  {
    name: "员工中心",
    url: "zhogntai",
    icon: "home",
    active_icon: "home_active"
  },
  {
    name: "系统管理",
    url: "zhogntai",
    icon: "home",
    active_icon: "home_active"
  }
];
</script>

<template>
  <div class="!leading-[50px] select-none">123312</div>
</template>

<style lang="scss" scoped></style>
