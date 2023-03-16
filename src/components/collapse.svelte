<!-- <script>
  /**
   * @type {any}
   */
  export let description;
  /**
   * @type {any}
   */
  export let caption;
</script>

<button class="collapsible">{caption}</button>
<div class="content">
  <p>
    {description}
  </p>
</div>

<style>
  .collapsible {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding: 40px 0px;
    gap: 32px;

    width: 536px;
    height: 109px;

    border-bottom: 1px solid rgba(30, 21, 21, 0.2);

    /* Inside auto layout */

    flex: none;
    order: 1;
    align-self: stretch;
    flex-grow: 0;
  }

  .active,
  .collapsible:hover {
    background-color: rgb(237, 237, 237);
  }

  .collapsible:after {
    content: "\2B9f";
    color: white;
    font-weight: bold;
    float: right;
    margin-left: 5px;
  }

  .active:after {
    content: "\2b9d";
  }

  .content {
    padding: 0 18px;
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.2s ease-out;
    background-color: #f1f1f1;
  }
</style> -->
