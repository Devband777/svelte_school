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
  <div>&#x2B95</div>
</button>

<style lang="scss">
  .btn_component {
    background-color: var(--bk_color);
    border-radius: 24px;
    width: 160px;
    height: 48px;
    display: flex;
    flex-direction: row;
    align-items: center;
    padding: 10px 10px 10px 24px;
    gap: 12px;
    border: none;

    /* Desktop/btn1 Desktop | 16 */

    font-family: "Suisse Intl";
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 100%;

    color: var(--text_color);

    div {
      width: 28px;
      height: 28px;
      background-color: var(--text_color);
      color: var(--bk_color);
      border-radius: 50%;
      
    }
  }
  .btn_component:hover {
    background-color: var(bk_color_hover);
  }
</style>
