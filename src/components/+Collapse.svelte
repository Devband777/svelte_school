<script>
  // @ts-nocheck
  let classNames = "collapsible";

  export let caption = "Collapse Caption";
  export let content =
    "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.";
</script>

<button
  on:click={(e) => {
    e.target.classList.toggle("active");
    if (e.target.nextElementSibling.style.maxHeight) {
      e.target.nextElementSibling.style.maxHeight = null;
    } else {
      e.target.nextElementSibling.style.maxHeight =
        e.target.nextElementSibling.scrollHeight + "px";
    }
  }}
  class="{classNames} ">{caption}</button
>
<div class="content">
  <p>
    {@html content}
  </p>
</div>

<style>
  .collapsible {
    cursor: pointer;
    padding: 18px;
    width: 100%;
    border: none;
    background-color: #fff;
    text-align: left;
    padding: 40px 0px;
    outline: none;
    /* Desktop/H5 Desktop | 24 */

    font-family: "Suisse Intl";
    font-style: normal;
    font-weight: 400;
    font-size: 24px;
    line-height: 120%;

    height: 109px;
    /* identical to box height, or 29px */

    /* Basic & Secondary/Black */

    color: #1e1515;
  }

  .active,
  .collapsible:hover {
    background-color: rgb(255, 255, 255);
  }

  .collapsible:after {
    content: "\002B";
    font-weight: bold;
    float: right;
    margin-left: 5px;
  }

  .active:after {
    content: "\2212";
  }

  .content {
    padding: 0 18px;
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.2s ease-out;
    background-color: #ffffff;
    border-bottom: 1px solid rgba(30, 21, 21, 0.2);

    /* Desktop/Body 2 Desktop | 16 */
  }
</style>
