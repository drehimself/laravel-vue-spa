<template>
  <div>
    Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptas, consequatur, itaque. Aut tempora delectus reiciendis et, quidem esse est deserunt quia unde quaerat eius amet, nisi illum quibusdam asperiores ab aliquid odio quas, alias nulla ipsum! Tempora id dolorum, explicabo nulla, totam in est molestiae ipsam. Odio laudantium nesciunt, quos libero quasi, iusto dolorum harum provident vero, quod voluptatum eveniet aspernatur quia. Facere, numquam quae. Aperiam eveniet obcaecati culpa pariatur ipsam alias qui, ea reiciendis excepturi. Omnis rem culpa excepturi autem earum tempora aperiam at itaque vero pariatur officia obcaecati repudiandae ipsam vitae provident, neque unde optio facilis totam. Amet velit beatae suscipit ea, fugit perspiciatis similique dolores ut. Eligendi facilis odit recusandae adipisci repellendus consequatur vero soluta pariatur, sed animi quasi facere nisi tempora quod, atque eum voluptatem dolorem ad, temporibus, iste rem non exercitationem. Laudantium molestias, nostrum corporis fuga, similique vitae nihil quas adipisci at asperiores sapiente expedita aliquid. Impedit, eius, id! Aliquid aperiam numquam, tenetur officiis, natus praesentium animi. Quod dolorum aliquam dolores iste voluptatum unde dolore error ducimus, voluptas sed voluptatem mollitia quos, totam nesciunt. Voluptate dolorem nemo eveniet corrupti voluptates itaque neque expedita minus a aperiam blanditiis sapiente facere numquam quae placeat aspernatur fugit sint, error impedit harum possimus ipsum, beatae libero ab sunt. Dolore soluta ratione, dignissimos enim atque nulla eum. Dolorem autem optio porro maiores sed laudantium sapiente enim! Voluptatum blanditiis saepe, vitae laborum. Ullam et, quaerat quia dicta repudiandae est quibusdam! Accusantium explicabo id iusto expedita corrupti neque harum totam obcaecati placeat, perferendis exercitationem nulla possimus tenetur consequatur, voluptates libero dolorem ab blanditiis error illo ipsum ipsam? Explicabo, impedit consequatur nihil modi consequuntur deserunt culpa, necessitatibus aspernatur placeat eius dolore, sed doloremque! Earum perspiciatis, aliquam tenetur quod, reprehenderit sunt minus nihil nulla ipsa ullam, totam. Vitae iusto maxime in error, quibusdam. Voluptate tempora quaerat accusantium fuga! In, dicta, atque ipsam vero eaque omnis optio! Cum non perferendis veritatis consequatur enim corporis excepturi atque quia debitis, eaque consectetur molestias praesentium odit quo animi ipsa quos inventore voluptates, nisi nesciunt eius ipsum reiciendis ullam distinctio beatae! Ex at perspiciatis quam eos corporis aut incidunt ut nisi, recusandae et libero accusamus, deserunt error, quod omnis similique? Sapiente expedita soluta quam, minima tempore maiores corporis. Minima, doloremque natus ab soluta aut quidem dolor aliquid, dolores eos itaque iste a sit ea incidunt excepturi. Hic cum a aliquid harum quaerat nulla voluptatum temporibus, maiores quod soluta, optio.

    <button v-tooltip="'You have ' + 3 + ' new messages.'">Count</button>
  </div>

</template>

<style>
  .tooltip {
  display: block !important;
  z-index: 10000;
}

.tooltip .tooltip-inner {
  background: black;
  color: white;
  border-radius: 16px;
  padding: 5px 10px 4px;
}

.tooltip .tooltip-arrow {
  width: 0;
  height: 0;
  border-style: solid;
  position: absolute;
  margin: 5px;
  border-color: black;
  z-index: 1;
}

.tooltip[x-placement^="top"] {
  margin-bottom: 5px;
}

.tooltip[x-placement^="top"] .tooltip-arrow {
  border-width: 5px 5px 0 5px;
  border-left-color: transparent !important;
  border-right-color: transparent !important;
  border-bottom-color: transparent !important;
  bottom: -5px;
  left: calc(50% - 5px);
  margin-top: 0;
  margin-bottom: 0;
}

.tooltip[x-placement^="bottom"] {
  margin-top: 5px;
}

.tooltip[x-placement^="bottom"] .tooltip-arrow {
  border-width: 0 5px 5px 5px;
  border-left-color: transparent !important;
  border-right-color: transparent !important;
  border-top-color: transparent !important;
  top: -5px;
  left: calc(50% - 5px);
  margin-top: 0;
  margin-bottom: 0;
}

.tooltip[x-placement^="right"] {
  margin-left: 5px;
}

.tooltip[x-placement^="right"] .tooltip-arrow {
  border-width: 5px 5px 5px 0;
  border-left-color: transparent !important;
  border-top-color: transparent !important;
  border-bottom-color: transparent !important;
  left: -5px;
  top: calc(50% - 5px);
  margin-left: 0;
  margin-right: 0;
}

.tooltip[x-placement^="left"] {
  margin-right: 5px;
}

.tooltip[x-placement^="left"] .tooltip-arrow {
  border-width: 5px 0 5px 5px;
  border-top-color: transparent !important;
  border-right-color: transparent !important;
  border-bottom-color: transparent !important;
  right: -5px;
  top: calc(50% - 5px);
  margin-left: 0;
  margin-right: 0;
}

.tooltip.popover .popover-inner {
  background: #f9f9f9;
  color: black;
  padding: 24px;
  border-radius: 5px;
  box-shadow: 0 5px 30px rgba(black, .1);
}

.tooltip.popover .popover-arrow {
  border-color: #f9f9f9;
}

.tooltip[aria-hidden='true'] {
  visibility: hidden;
  opacity: 0;
  transition: opacity .15s, visibility .15s;
}

.tooltip[aria-hidden='false'] {
  visibility: visible;
  opacity: 1;
  transition: opacity .15s;
}
</style>
