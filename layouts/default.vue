<template>
  <div>
    <nav class=" p-4 border-b">
      <div class="max-w-7xl mx-auto ">
        <div class="flex items-center justify-between h-6 lg:space-x-6'">
          <div class="flex">
            <Button @click="router.push('/')" variant="ghost">
              <IconsDashboard class="w-4 h-4 mr-2" /> Dashboard
            </Button>
            <Button @click="router.push('/pedidos')" variant="ghost">
              <IconsPedidos class="w-4 h-4 mr-2" /> Pedidos
            </Button>
            <Button @click="router.push('/caixa')" variant="ghost">
              <IconsCaixa class="w-4 h-4 mr-2" /> Caixa
            </Button>
          </div>
        </div>
      </div>
    </nav>
    <slot />
  </div>
</template>

<script lang="ts" setup>
const router = useRouter()
</script>

<style></style>