<template>
    <div class="message">
      <svg class="icon">
        <use :xlink:href="`#icon-${typeName}`"></use>
      </svg>
      <slot></slot>
    </div>
</template>

<script>
export default {
  props: {
    autoCloseDelay: {
      type: Number,
      default: 2
    },
    typeName: {
      type: String
    } 
  },
  mounted() {
    setTimeout(() => {
      this.close()
    }, this.autoCloseDelay * 1000)  
  },
  methods: {  
    close() {
      this.$el.remove()
      this.$destroy()
    }
  }
}
</script>
<style lang="scss" scoped>
  .message {
    border: 1px solid#ebedf0;
    border-radius: 8px;
    position: fixed;
    top: 5%;
    left: 50%;
    transform: translateX(-50%);
    padding: 8px 18px;    
    box-shadow: 0px 2px 8px rgba(0,0,0,0.3);
    text-align: center;
    display: flex;
    align-items: center;
    animation: slide-message 0.4s;
    background: #fff;
    z-index: 100;
    .icon {
      width: 18px;
      height: 18px;
      fill: #47b8e0;
      margin-right: 10px;
    }
  }

  @keyframes slide-message {
    0% {
      transform: translate(-50%,-50%);
      opacity: 0;
    }
    100% {
      transform: translate(-50%);
      opacity: 1;
    }
  }
 
</style>