<template>
  <div id="social">
    <ul>
      <li>
        <a href="https://github.com/JuliaAstro">
          <fa :icon="['fab', 'github']"/>&nbsp;&nbsp;JuliaAstro
        </a> on GitHub
      </li>
      <li>
        <a href="https://groups.google.com/forum/#!forum/julia-astro">
          <fa icon="envelope"/>&nbsp;&nbsp;julia-astro mailing list
        </a> on Google Groups
      </li>
      <li>
        <a href="https://discourse.julialang.org/c/domain/astro">
          <fa icon="comment"/>&nbsp;&nbsp;Astro/Space topics
        </a>
 on JuliaLang Discourse
      </li>
      <li>
        <a href="https://riot.im/app/#/room/#JuliaAstro:openastronomy.org">
          <fa icon="comment"/>&nbsp;&nbsp;#JuliaAstro:openastronomy.org
        </a> on Matrix
      </li>
      <li>
        <a href="slack://channel?id=CMXU6SD7V&team=T68168MUP">
          <fa icon="comment"/>&nbsp;&nbsp;#astronomy
        </a> on
        <a href="https://slackinvite.julialang.org/">JuliaLang Slack</a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Social"
};
</script>