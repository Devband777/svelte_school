<script>
  import Button from "../+button.svelte";

  export let card_width = "";
  export let card_height = "";
  export let card_left = "";
  export let card_top = "";

  export let img_url = "";
  export let title = "title";
  export let content = "content";

  export let btn_bk_color = "";
  export let btn_text_color = "";
  export let btn_caption = "";

</script>

<div class="card" style="
  width: {card_width};
  height: {card_height};
  left: {card_left};
  top: {card_top};
">
  <img src={img_url} class="img" />
  <div class="heading-subtitle">
    <span class="title">{title}</span>
    <span class="content">
      {content}
    </span>
  </div>
  <div class="button">
    <Button
      bk_color={btn_bk_color}
      text_color={btn_text_color}
      caption={btn_caption}
    />
  </div>
</div>

<style lang="scss">
  .card {
    /* Auto layout */
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 48px 32px 72px;
    gap: 48px;
    isolation: isolate;

    position: absolute;

    /* Basic & Secondary/White */

    background: #FFFFFF;
    /* Blur 80 | 10% */

    box-shadow: 0px 4px 80px rgba(68, 40, 14, 0.1);
    border-radius: 24px;

    .img {
      width: 97px;
      height: 82px;


      /* Inside auto layout */

      flex: none;
      order: 0;
      flex-grow: 0;
      z-index: 0;
    }

    .heading-subtitle {
      /* Auto layout */

      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      padding: 0px;
      gap: 16px;

      width: 248px;
      height: 110px;


      /* Inside auto layout */

      flex: none;
      order: 1;
      flex-grow: 0;
      z-index: 1;

      .title {
        width: 248px;
        height: 28px;

        /* Desktop/Body Medium Desktop | 20 */

        font-family: 'Suisse Intl';
        font-style: normal;
        font-weight: 500;
        font-size: 20px;
        line-height: 140%;
        /* identical to box height, or 28px */

        text-align: center;

        /* Basic & Secondary/Black */

        color: #1E1515;


        /* Inside auto layout */

        flex: none;
        order: 0;
        flex-grow: 0;
      }

      .content {
        width: 246px;
        height: 66px;

        /* Desktop/Body 2 Desktop | 16 */

        font-family: 'Suisse Intl';
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 140%;
        /* or 22px */

        text-align: center;

        /* Basic & Secondary/Black */

        color: #1E1515;

        opacity: 0.6;

        /* Inside auto layout */

        flex: none;
        order: 1;
        flex-grow: 0;
      }
    }

    .button {
      position: absolute;
      width: 160px;
      height: 48px;
      left: calc(50% - 160px/2);
      top: 93%;
    }
  }
</style>