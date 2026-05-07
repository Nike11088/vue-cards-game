<template>
  <div class="field-container">
    <div
      v-for="(col, colIndex) in field.cols"
      :key="colIndex"
    >
      <div
        v-for="(row, rowIndex) in field.rows"
        :key="rowIndex"
      >
        <div class="cell">
          {{ rowIndex }}
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
type Field = {
  rows: number
  cols: number
}
const field: Field = {
  rows: 8,
  cols: 4
}
</script>

<style scoped>
.field-container {
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 8px;
  box-sizing: border-box;
}
</style>
