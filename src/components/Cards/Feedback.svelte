<script>
  import ParentAvatar from "$lib/images/parent_avatar.png";
  import PolygonImg from "$lib/images/Polygon.png";

  export let content = "";
  export let name1 = "";
  export let name2 = "";
</script>

<div class="feedback-card">
  <div class="body">
    <div class="text-content">
      {content}
    </div>
    <div class="name">
      <h1 class="parent-name">{name1}</h1>
      <p class="whoose-parent">{name2}</p>
    </div>
  </div>
  <div class="avatar">
    <div class="play-button">&#x2BC8;</div>
    <div class="avatar-img">
      <!-- svelte-ignore a11y-missing-attribute -->
      <img src={ParentAvatar} />
    </div>
  </div>
</div>

<style lang="scss">
  .feedback-card {
    width: 648px;
    height: 338px;
    position: relative;

    /* Blur 80 | 10% */

    filter: drop-shadow(0px 4px 80px rgba(68, 40, 14, 0.1));

    /* Inside auto layout */

    flex: none;
    order: 5;
    flex-grow: 0;

    .body {
      display: flex;
      flex-direction: column;
      align-items: flex-start;
      padding: 48px;

      position: absolute;
      left: 0%;
      right: 0%;
      top: -0.59%;
      bottom: 17.16%;

      background: #ffffff;
      border-radius: 24px;

      .text-content {
        width: 552px;
        height: 84px;

        /* Desktop/Body Medium Desktop | 20 */

        font-family: "Suisse Intl";
        font-style: normal;
        font-weight: 500;
        font-size: 20px;
        line-height: 140%;
        /* or 28px */

        /* Basic & Secondary/Black */

        color: #1e1515;

        /* Inside auto layout */

        flex: none;
        order: 0;
        align-self: stretch;
        flex-grow: 0;
      }

      .name {
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        padding: 0px;

        width: 552px;
        height: 54px;

        /* Inside auto layout */

        flex: none;
        order: 1;
        align-self: stretch;
        flex-grow: 0;
      }
    }

    .avatar {
      position: absolute;
      left: 74.07%;
      right: 7.41%;
      top: 60%;
      bottom: -0.59%;
      .play-button {
        position: absolute;
        left: 67.65%;
        right: 7.41%;
        top: 0;
        bottom: 25.44%;

        background-color: #1e1515;
        border-radius: 50%;
        color: #ffffff;
        width: 32px;
        height: 32px;
        text-align: center;

        display: flex;
        justify-content: center;
        align-items: center;
      }
      .avatar-img {
        background-repeat: no-repeat;
      }
    }
  }
</style>
