<template>
  <div>
    <p>Clicked {{ count }} times! Count is {{ parity }}.</p>
  </div>
</template>

<script>
export default {
  name: "Counter",
  data: function() {
    return {
      count: 0
    };
  },
  computed: {
    parity: function() {
      return this.count % 2 === 0 ? "even" : "odd";
    }
  }
};
</script>