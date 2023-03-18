<script>
  export let title_color = "";

  export let title1 = "title1";
  export let title2 = "%";
  export let content = "content";

</script>

<div class="card">
  <div class="title" style="color: {title_color};">
    <span class="title1">{title1}</span>
    <span class="title2">{title2}</span>
  </div>
  <span class="content">
    {content}
  </span>
</div>

<style lang="scss">
  .card {
    /* Auto layout */

    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 48px 30px;
    gap: 48px;

    width: 312px;
    height: 312px;

    background: #FFFFFF;
    /* Blur 80 | 10% */

    box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);
    border-radius: 20px;

    /* Inside auto layout */

    flex: none;
    order: 1;
    flex-grow: 0;

    .title {
      /* Auto layout */

      display: flex;
      flex-direction: row;
      justify-content: flex-end;
      align-items: flex-start;
      padding: 0px;

      width: 169px;
      height: 80px;


      /* Inside auto layout */

      flex: none;
      order: 0;
      flex-grow: 0;

      .title1 {
        width: 131px;
        height: 80px;

        font-family: 'Suisse Intl';
        font-style: normal;
        font-weight: 500;
        font-size: 80px;
        line-height: 100%;
        /* identical to box height, or 80px */

        letter-spacing: -0.02em;

        /* Brandcolors/Purple */


        /* Inside auto layout */

        flex: none;
        order: 0;
        flex-grow: 0;
      }

      .title2 {
        width: 38px;
        height: 43px;

        font-family: 'Suisse Intl';
        font-style: normal;
        font-weight: 500;
        font-size: 36px;
        line-height: 120%;
        /* or 43px */


        /* Brandcolors/Purple */

        /* Inside auto layout */

        flex: none;
        order: 1;
        flex-grow: 0;
      }
    }

    .content {
      width: 248px;
      height: 66px;

      /* Desktop/Body 2 Desktop | 16 */

      font-family: 'Suisse Intl';
      font-style: normal;
      font-weight: 400;
      font-size: 16px;
      line-height: 140%;
      /* or 22px */

      text-align: center;

      color: rgba(15, 17, 33, 0.6);


      /* Inside auto layout */

      flex: none;
      order: 1;
      flex-grow: 0;
    }
  }
</style>