<script setup lang="ts">
/**
 * Camada decorativa de bolinhas roxas para fundos claros.
 * Fica atrás do conteúdo e não captura cliques.
 *
 * variant:
 *  - 'a' (padrão): bokeh nos cantos opostos + pontos espalhados + anéis
 *  - 'b': manchas nas laterais, pontos maiores e mais anéis (visual mais aberto)
 */
withDefaults(
  defineProps<{ variant?: 'a' | 'b' }>(),
  { variant: 'a' },
)
</script>

<template>
  <div class="academe-dots absolute inset-0 overflow-hidden pointer-events-none">
    <!-- ============ Variante A ============ -->
    <template v-if="variant === 'a'">
      <div class="dot" style="width:340px;height:340px;top:-90px;left:-80px;background:#892cdd;opacity:.16;filter:blur(10px)"></div>
      <div class="dot" style="width:420px;height:420px;bottom:-140px;right:-120px;background:#a855f7;opacity:.14;filter:blur(14px)"></div>
      <div class="dot" style="width:180px;height:180px;top:60px;right:120px;background:#6b1fb8;opacity:.12;filter:blur(6px)"></div>

      <div class="dot" style="width:26px;height:26px;top:120px;left:180px;background:#892cdd;opacity:.7"></div>
      <div class="dot" style="width:14px;height:14px;top:200px;left:120px;background:#a855f7;opacity:.6"></div>
      <div class="dot" style="width:18px;height:18px;bottom:150px;left:90px;background:#892cdd;opacity:.5"></div>
      <div class="dot" style="width:12px;height:12px;bottom:90px;right:220px;background:#a855f7;opacity:.6"></div>
      <div class="dot" style="width:22px;height:22px;top:90px;right:80px;background:#892cdd;opacity:.55"></div>
      <div class="dot" style="width:10px;height:10px;bottom:200px;right:120px;background:#6b1fb8;opacity:.5"></div>

      <div class="dot ring" style="width:40px;height:40px;top:70px;left:260px;border-color:#892cdd;opacity:.5"></div>
      <div class="dot ring" style="width:28px;height:28px;bottom:120px;right:300px;border-color:#a855f7;opacity:.5"></div>
    </template>

    <!-- ============ Variante B ============ -->
    <template v-else>
      <!-- Manchas centradas nas laterais (esquerda/direita) -->
      <div class="dot" style="width:380px;height:380px;top:50%;left:-160px;transform:translateY(-50%);background:#a855f7;opacity:.13;filter:blur(16px)"></div>
      <div class="dot" style="width:300px;height:300px;top:50%;right:-130px;transform:translateY(-50%);background:#892cdd;opacity:.14;filter:blur(12px)"></div>
      <div class="dot" style="width:150px;height:150px;top:-50px;left:45%;background:#6b1fb8;opacity:.10;filter:blur(8px)"></div>

      <!-- Anéis maiores e mais presentes -->
      <div class="dot ring" style="width:70px;height:70px;top:80px;left:120px;border-color:#892cdd;opacity:.45;border-width:4px"></div>
      <div class="dot ring" style="width:48px;height:48px;bottom:110px;left:220px;border-color:#a855f7;opacity:.5"></div>
      <div class="dot ring" style="width:60px;height:60px;top:140px;right:150px;border-color:#6b1fb8;opacity:.4;border-width:4px"></div>
      <div class="dot ring" style="width:34px;height:34px;bottom:90px;right:110px;border-color:#892cdd;opacity:.5"></div>

      <!-- Poucos pontos sólidos maiores -->
      <div class="dot" style="width:30px;height:30px;bottom:150px;left:110px;background:#a855f7;opacity:.55"></div>
      <div class="dot" style="width:20px;height:20px;top:110px;right:260px;background:#892cdd;opacity:.55"></div>
    </template>
  </div>
</template>

<style scoped>
.dot {
  position: absolute;
  border-radius: 9999px;
}
.dot.ring {
  background: transparent !important;
  border: 3px solid;
}
</style>
