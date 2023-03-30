<script>
  export let title_color = "";

  export let title1 = "";
  export let title2 = "";
  export let content = "";
</script>

<div class="card1">
  <h1 class="title" style="color: {title_color};">
    {title1}<sup>{title2}</sup>
  </h1>
  <p class="content">
    {content}
  </p>
</div>

<style lang="scss">
  .card1 {
    /* Auto layout */
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 312px;
    height: 312px;
    padding: 48px 30px;
    background: #ffffff;
    /* Blur 80 | 10% */
    box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);
    border-radius: 20px;
    /* Inside auto layout */
    text-align: center;
    gap: 48px;

    .title {
      font-family: "Suisse Intl Medium";
      font-style: normal;
      font-weight: 500;
      font-size: 80px;
      line-height: 100%;
      margin: 0%;
    }

    .content {

      /* Desktop/Body 2 Desktop | 16 */

      font-family: "Suisse Intl";
      font-style: normal;
      font-weight: 400;
      font-size: 16px;
      line-height: 140%;
      /* or 22px */

      color: rgba(15, 17, 33, 0.6);
    }
  }
</style>
