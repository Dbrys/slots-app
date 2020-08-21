<script>
export default {
  functional: true,
  name: "Loader",
  render(createElement) {
    return createElement("div", {
      attrs: {
        class: "spinner-border",
        role: "status",
      },
    });
  },
};
</script>
