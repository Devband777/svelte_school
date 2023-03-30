<script>
  export let bk_color = "red";
  export let bk_color_hover = "blue";
  export let text_color = "yellow";

  /**
   * @type {any}
   */
  export let caption = "test";
</script>

<button
  class="btn_component"
  style="--bk_color: {bk_color}; --text_color: {text_color}; --bk_color_hover: {bk_color_hover}"
  >{caption}
  <spain class="btn-icon">&#x2B95</spain>
</button>

<style lang="scss">
  .btn_component {
    background-color: var(--bk_color);
    border-radius: 24px;
    padding: 10px 20px;
    gap: 12px;
    border: none;

    display: flex;
    justify-content: center;
    align-items: center;
    /* Desktop/btn1 Desktop | 16 */

    font-family: "Suisse Intl";
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 100%;

    color: var(--text_color);
    width: auto;

    .btn-icon {
      width: 28px;
      height: 28px;
      background-color: var(--text_color);
      color: var(--bk_color);
      border-radius: 50%;

      display: flex;
      justify-content: center;
      align-items: center;
      float: right;
    }
  }
  .btn_component:hover {
    background-color: var(bk_color_hover);
  }
</style>
