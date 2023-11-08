<template>
    <div class="flex items-center justify-center">
      <div class="p-10 overflow-hidden bg-white shadow-sm sm:rounded-lg">
        <div id="card-header" class="px-4 py-3">
          <slot name="header"></slot>
        </div>
        <div id="card-footer">
          <slot name="footer"></slot>
        </div>
      </div>
    </div>


</template>
