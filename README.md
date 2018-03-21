<!DOCTYPE html>
<html>
<head><meta charset="utf-8" />
<title>ManipulandoDados</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.0.3/jquery.min.js"></script>

<style type="text/css">
    /*!
*
* Twitter Bootstrap
*
*/
/*!
 * Bootstrap v3.3.7 (http://getbootstrap.com)
 * Copyright 2011-2016 Twitter, Inc.
 * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
 */
/*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */
html {
  font-family: sans-serif;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
}
body {
  margin: 0;
}
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
main,
menu,
nav,
section,
summary {
  display: block;
}
audio,
canvas,
progress,
video {
  display: inline-block;
  vertical-align: baseline;
}
audio:not([controls]) {
  display: none;
  height: 0;
}
[hidden],
template {
  display: none;
}
a {
  background-color: transparent;
}
a:active,
a:hover {
  outline: 0;
}
abbr[title] {
  border-bottom: 1px dotted;
}
b,
strong {
  font-weight: bold;
}
dfn {
  font-style: italic;
}
h1 {
  font-size: 2em;
  margin: 0.67em 0;
}
mark {
  background: #ff0;
  color: #000;
}
small {
  font-size: 80%;
}
sub,
sup {
  font-size: 75%;
  line-height: 0;
  position: relative;
  vertical-align: baseline;
}
sup {
  top: -0.5em;
}
sub {
  bottom: -0.25em;
}
img {
  border: 0;
}
svg:not(:root) {
  overflow: hidden;
}
figure {
  margin: 1em 40px;
}
hr {
  box-sizing: content-box;
  height: 0;
}
pre {
  overflow: auto;
}
code,
kbd,
pre,
samp {
  font-family: monospace, monospace;
  font-size: 1em;
}
button,
input,
optgroup,
select,
textarea {
  color: inherit;
  font: inherit;
  margin: 0;
}
button {
  overflow: visible;
}
button,
select {
  text-transform: none;
}
button,
html input[type="button"],
input[type="reset"],
input[type="submit"] {
  -webkit-appearance: button;
  cursor: pointer;
}
button[disabled],
html input[disabled] {
  cursor: default;
}
button::-moz-focus-inner,
input::-moz-focus-inner {
  border: 0;
  padding: 0;
}
input {
  line-height: normal;
}
input[type="checkbox"],
input[type="radio"] {
  box-sizing: border-box;
  padding: 0;
}
input[type="number"]::-webkit-inner-spin-button,
input[type="number"]::-webkit-outer-spin-button {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: textfield;
  box-sizing: content-box;
}
input[type="search"]::-webkit-search-cancel-button,
input[type="search"]::-webkit-search-decoration {
  -webkit-appearance: none;
}
fieldset {
  border: 1px solid #c0c0c0;
  margin: 0 2px;
  padding: 0.35em 0.625em 0.75em;
}
legend {
  border: 0;
  padding: 0;
}
textarea {
  overflow: auto;
}
optgroup {
  font-weight: bold;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}
td,
th {
  padding: 0;
}
/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */
@media print {
  *,
  *:before,
  *:after {
    background: transparent !important;
    color: #000 !important;
    box-shadow: none !important;
    text-shadow: none !important;
  }
  a,
  a:visited {
    text-decoration: underline;
  }
  a[href]:after {
    content: " (" attr(href) ")";
  }
  abbr[title]:after {
    content: " (" attr(title) ")";
  }
  a[href^="#"]:after,
  a[href^="javascript:"]:after {
    content: "";
  }
  pre,
  blockquote {
    border: 1px solid #999;
    page-break-inside: avoid;
  }
  thead {
    display: table-header-group;
  }
  tr,
  img {
    page-break-inside: avoid;
  }
  img {
    max-width: 100% !important;
  }
  p,
  h2,
  h3 {
    orphans: 3;
    widows: 3;
  }
  h2,
  h3 {
    page-break-after: avoid;
  }
  .navbar {
    display: none;
  }
  .btn > .caret,
  .dropup > .btn > .caret {
    border-top-color: #000 !important;
  }
  .label {
    border: 1px solid #000;
  }
  .table {
    border-collapse: collapse !important;
  }
  .table td,
  .table th {
    background-color: #fff !important;
  }
  .table-bordered th,
  .table-bordered td {
    border: 1px solid #ddd !important;
  }
}
@font-face {
  font-family: 'Glyphicons Halflings';
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot');
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot?#iefix') format('embedded-opentype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff2') format('woff2'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff') format('woff'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.ttf') format('truetype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular') format('svg');
}
.glyphicon {
  position: relative;
  top: 1px;
  display: inline-block;
  font-family: 'Glyphicons Halflings';
  font-style: normal;
  font-weight: normal;
  line-height: 1;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.glyphicon-asterisk:before {
  content: "\002a";
}
.glyphicon-plus:before {
  content: "\002b";
}
.glyphicon-euro:before,
.glyphicon-eur:before {
  content: "\20ac";
}
.glyphicon-minus:before {
  content: "\2212";
}
.glyphicon-cloud:before {
  content: "\2601";
}
.glyphicon-envelope:before {
  content: "\2709";
}
.glyphicon-pencil:before {
  content: "\270f";
}
.glyphicon-glass:before {
  content: "\e001";
}
.glyphicon-music:before {
  content: "\e002";
}
.glyphicon-search:before {
  content: "\e003";
}
.glyphicon-heart:before {
  content: "\e005";
}
.glyphicon-star:before {
  content: "\e006";
}
.glyphicon-star-empty:before {
  content: "\e007";
}
.glyphicon-user:before {
  content: "\e008";
}
.glyphicon-film:before {
  content: "\e009";
}
.glyphicon-th-large:before {
  content: "\e010";
}
.glyphicon-th:before {
  content: "\e011";
}
.glyphicon-th-list:before {
  content: "\e012";
}
.glyphicon-ok:before {
  content: "\e013";
}
.glyphicon-remove:before {
  content: "\e014";
}
.glyphicon-zoom-in:before {
  content: "\e015";
}
.glyphicon-zoom-out:before {
  content: "\e016";
}
.glyphicon-off:before {
  content: "\e017";
}
.glyphicon-signal:before {
  content: "\e018";
}
.glyphicon-cog:before {
  content: "\e019";
}
.glyphicon-trash:before {
  content: "\e020";
}
.glyphicon-home:before {
  content: "\e021";
}
.glyphicon-file:before {
  content: "\e022";
}
.glyphicon-time:before {
  content: "\e023";
}
.glyphicon-road:before {
  content: "\e024";
}
.glyphicon-download-alt:before {
  content: "\e025";
}
.glyphicon-download:before {
  content: "\e026";
}
.glyphicon-upload:before {
  content: "\e027";
}
.glyphicon-inbox:before {
  content: "\e028";
}
.glyphicon-play-circle:before {
  content: "\e029";
}
.glyphicon-repeat:before {
  content: "\e030";
}
.glyphicon-refresh:before {
  content: "\e031";
}
.glyphicon-list-alt:before {
  content: "\e032";
}
.glyphicon-lock:before {
  content: "\e033";
}
.glyphicon-flag:before {
  content: "\e034";
}
.glyphicon-headphones:before {
  content: "\e035";
}
.glyphicon-volume-off:before {
  content: "\e036";
}
.glyphicon-volume-down:before {
  content: "\e037";
}
.glyphicon-volume-up:before {
  content: "\e038";
}
.glyphicon-qrcode:before {
  content: "\e039";
}
.glyphicon-barcode:before {
  content: "\e040";
}
.glyphicon-tag:before {
  content: "\e041";
}
.glyphicon-tags:before {
  content: "\e042";
}
.glyphicon-book:before {
  content: "\e043";
}
.glyphicon-bookmark:before {
  content: "\e044";
}
.glyphicon-print:before {
  content: "\e045";
}
.glyphicon-camera:before {
  content: "\e046";
}
.glyphicon-font:before {
  content: "\e047";
}
.glyphicon-bold:before {
  content: "\e048";
}
.glyphicon-italic:before {
  content: "\e049";
}
.glyphicon-text-height:before {
  content: "\e050";
}
.glyphicon-text-width:before {
  content: "\e051";
}
.glyphicon-align-left:before {
  content: "\e052";
}
.glyphicon-align-center:before {
  content: "\e053";
}
.glyphicon-align-right:before {
  content: "\e054";
}
.glyphicon-align-justify:before {
  content: "\e055";
}
.glyphicon-list:before {
  content: "\e056";
}
.glyphicon-indent-left:before {
  content: "\e057";
}
.glyphicon-indent-right:before {
  content: "\e058";
}
.glyphicon-facetime-video:before {
  content: "\e059";
}
.glyphicon-picture:before {
  content: "\e060";
}
.glyphicon-map-marker:before {
  content: "\e062";
}
.glyphicon-adjust:before {
  content: "\e063";
}
.glyphicon-tint:before {
  content: "\e064";
}
.glyphicon-edit:before {
  content: "\e065";
}
.glyphicon-share:before {
  content: "\e066";
}
.glyphicon-check:before {
  content: "\e067";
}
.glyphicon-move:before {
  content: "\e068";
}
.glyphicon-step-backward:before {
  content: "\e069";
}
.glyphicon-fast-backward:before {
  content: "\e070";
}
.glyphicon-backward:before {
  content: "\e071";
}
.glyphicon-play:before {
  content: "\e072";
}
.glyphicon-pause:before {
  content: "\e073";
}
.glyphicon-stop:before {
  content: "\e074";
}
.glyphicon-forward:before {
  content: "\e075";
}
.glyphicon-fast-forward:before {
  content: "\e076";
}
.glyphicon-step-forward:before {
  content: "\e077";
}
.glyphicon-eject:before {
  content: "\e078";
}
.glyphicon-chevron-left:before {
  content: "\e079";
}
.glyphicon-chevron-right:before {
  content: "\e080";
}
.glyphicon-plus-sign:before {
  content: "\e081";
}
.glyphicon-minus-sign:before {
  content: "\e082";
}
.glyphicon-remove-sign:before {
  content: "\e083";
}
.glyphicon-ok-sign:before {
  content: "\e084";
}
.glyphicon-question-sign:before {
  content: "\e085";
}
.glyphicon-info-sign:before {
  content: "\e086";
}
.glyphicon-screenshot:before {
  content: "\e087";
}
.glyphicon-remove-circle:before {
  content: "\e088";
}
.glyphicon-ok-circle:before {
  content: "\e089";
}
.glyphicon-ban-circle:before {
  content: "\e090";
}
.glyphicon-arrow-left:before {
  content: "\e091";
}
.glyphicon-arrow-right:before {
  content: "\e092";
}
.glyphicon-arrow-up:before {
  content: "\e093";
}
.glyphicon-arrow-down:before {
  content: "\e094";
}
.glyphicon-share-alt:before {
  content: "\e095";
}
.glyphicon-resize-full:before {
  content: "\e096";
}
.glyphicon-resize-small:before {
  content: "\e097";
}
.glyphicon-exclamation-sign:before {
  content: "\e101";
}
.glyphicon-gift:before {
  content: "\e102";
}
.glyphicon-leaf:before {
  content: "\e103";
}
.glyphicon-fire:before {
  content: "\e104";
}
.glyphicon-eye-open:before {
  content: "\e105";
}
.glyphicon-eye-close:before {
  content: "\e106";
}
.glyphicon-warning-sign:before {
  content: "\e107";
}
.glyphicon-plane:before {
  content: "\e108";
}
.glyphicon-calendar:before {
  content: "\e109";
}
.glyphicon-random:before {
  content: "\e110";
}
.glyphicon-comment:before {
  content: "\e111";
}
.glyphicon-magnet:before {
  content: "\e112";
}
.glyphicon-chevron-up:before {
  content: "\e113";
}
.glyphicon-chevron-down:before {
  content: "\e114";
}
.glyphicon-retweet:before {
  content: "\e115";
}
.glyphicon-shopping-cart:before {
  content: "\e116";
}
.glyphicon-folder-close:before {
  content: "\e117";
}
.glyphicon-folder-open:before {
  content: "\e118";
}
.glyphicon-resize-vertical:before {
  content: "\e119";
}
.glyphicon-resize-horizontal:before {
  content: "\e120";
}
.glyphicon-hdd:before {
  content: "\e121";
}
.glyphicon-bullhorn:before {
  content: "\e122";
}
.glyphicon-bell:before {
  content: "\e123";
}
.glyphicon-certificate:before {
  content: "\e124";
}
.glyphicon-thumbs-up:before {
  content: "\e125";
}
.glyphicon-thumbs-down:before {
  content: "\e126";
}
.glyphicon-hand-right:before {
  content: "\e127";
}
.glyphicon-hand-left:before {
  content: "\e128";
}
.glyphicon-hand-up:before {
  content: "\e129";
}
.glyphicon-hand-down:before {
  content: "\e130";
}
.glyphicon-circle-arrow-right:before {
  content: "\e131";
}
.glyphicon-circle-arrow-left:before {
  content: "\e132";
}
.glyphicon-circle-arrow-up:before {
  content: "\e133";
}
.glyphicon-circle-arrow-down:before {
  content: "\e134";
}
.glyphicon-globe:before {
  content: "\e135";
}
.glyphicon-wrench:before {
  content: "\e136";
}
.glyphicon-tasks:before {
  content: "\e137";
}
.glyphicon-filter:before {
  content: "\e138";
}
.glyphicon-briefcase:before {
  content: "\e139";
}
.glyphicon-fullscreen:before {
  content: "\e140";
}
.glyphicon-dashboard:before {
  content: "\e141";
}
.glyphicon-paperclip:before {
  content: "\e142";
}
.glyphicon-heart-empty:before {
  content: "\e143";
}
.glyphicon-link:before {
  content: "\e144";
}
.glyphicon-phone:before {
  content: "\e145";
}
.glyphicon-pushpin:before {
  content: "\e146";
}
.glyphicon-usd:before {
  content: "\e148";
}
.glyphicon-gbp:before {
  content: "\e149";
}
.glyphicon-sort:before {
  content: "\e150";
}
.glyphicon-sort-by-alphabet:before {
  content: "\e151";
}
.glyphicon-sort-by-alphabet-alt:before {
  content: "\e152";
}
.glyphicon-sort-by-order:before {
  content: "\e153";
}
.glyphicon-sort-by-order-alt:before {
  content: "\e154";
}
.glyphicon-sort-by-attributes:before {
  content: "\e155";
}
.glyphicon-sort-by-attributes-alt:before {
  content: "\e156";
}
.glyphicon-unchecked:before {
  content: "\e157";
}
.glyphicon-expand:before {
  content: "\e158";
}
.glyphicon-collapse-down:before {
  content: "\e159";
}
.glyphicon-collapse-up:before {
  content: "\e160";
}
.glyphicon-log-in:before {
  content: "\e161";
}
.glyphicon-flash:before {
  content: "\e162";
}
.glyphicon-log-out:before {
  content: "\e163";
}
.glyphicon-new-window:before {
  content: "\e164";
}
.glyphicon-record:before {
  content: "\e165";
}
.glyphicon-save:before {
  content: "\e166";
}
.glyphicon-open:before {
  content: "\e167";
}
.glyphicon-saved:before {
  content: "\e168";
}
.glyphicon-import:before {
  content: "\e169";
}
.glyphicon-export:before {
  content: "\e170";
}
.glyphicon-send:before {
  content: "\e171";
}
.glyphicon-floppy-disk:before {
  content: "\e172";
}
.glyphicon-floppy-saved:before {
  content: "\e173";
}
.glyphicon-floppy-remove:before {
  content: "\e174";
}
.glyphicon-floppy-save:before {
  content: "\e175";
}
.glyphicon-floppy-open:before {
  content: "\e176";
}
.glyphicon-credit-card:before {
  content: "\e177";
}
.glyphicon-transfer:before {
  content: "\e178";
}
.glyphicon-cutlery:before {
  content: "\e179";
}
.glyphicon-header:before {
  content: "\e180";
}
.glyphicon-compressed:before {
  content: "\e181";
}
.glyphicon-earphone:before {
  content: "\e182";
}
.glyphicon-phone-alt:before {
  content: "\e183";
}
.glyphicon-tower:before {
  content: "\e184";
}
.glyphicon-stats:before {
  content: "\e185";
}
.glyphicon-sd-video:before {
  content: "\e186";
}
.glyphicon-hd-video:before {
  content: "\e187";
}
.glyphicon-subtitles:before {
  content: "\e188";
}
.glyphicon-sound-stereo:before {
  content: "\e189";
}
.glyphicon-sound-dolby:before {
  content: "\e190";
}
.glyphicon-sound-5-1:before {
  content: "\e191";
}
.glyphicon-sound-6-1:before {
  content: "\e192";
}
.glyphicon-sound-7-1:before {
  content: "\e193";
}
.glyphicon-copyright-mark:before {
  content: "\e194";
}
.glyphicon-registration-mark:before {
  content: "\e195";
}
.glyphicon-cloud-download:before {
  content: "\e197";
}
.glyphicon-cloud-upload:before {
  content: "\e198";
}
.glyphicon-tree-conifer:before {
  content: "\e199";
}
.glyphicon-tree-deciduous:before {
  content: "\e200";
}
.glyphicon-cd:before {
  content: "\e201";
}
.glyphicon-save-file:before {
  content: "\e202";
}
.glyphicon-open-file:before {
  content: "\e203";
}
.glyphicon-level-up:before {
  content: "\e204";
}
.glyphicon-copy:before {
  content: "\e205";
}
.glyphicon-paste:before {
  content: "\e206";
}
.glyphicon-alert:before {
  content: "\e209";
}
.glyphicon-equalizer:before {
  content: "\e210";
}
.glyphicon-king:before {
  content: "\e211";
}
.glyphicon-queen:before {
  content: "\e212";
}
.glyphicon-pawn:before {
  content: "\e213";
}
.glyphicon-bishop:before {
  content: "\e214";
}
.glyphicon-knight:before {
  content: "\e215";
}
.glyphicon-baby-formula:before {
  content: "\e216";
}
.glyphicon-tent:before {
  content: "\26fa";
}
.glyphicon-blackboard:before {
  content: "\e218";
}
.glyphicon-bed:before {
  content: "\e219";
}
.glyphicon-apple:before {
  content: "\f8ff";
}
.glyphicon-erase:before {
  content: "\e221";
}
.glyphicon-hourglass:before {
  content: "\231b";
}
.glyphicon-lamp:before {
  content: "\e223";
}
.glyphicon-duplicate:before {
  content: "\e224";
}
.glyphicon-piggy-bank:before {
  content: "\e225";
}
.glyphicon-scissors:before {
  content: "\e226";
}
.glyphicon-bitcoin:before {
  content: "\e227";
}
.glyphicon-btc:before {
  content: "\e227";
}
.glyphicon-xbt:before {
  content: "\e227";
}
.glyphicon-yen:before {
  content: "\00a5";
}
.glyphicon-jpy:before {
  content: "\00a5";
}
.glyphicon-ruble:before {
  content: "\20bd";
}
.glyphicon-rub:before {
  content: "\20bd";
}
.glyphicon-scale:before {
  content: "\e230";
}
.glyphicon-ice-lolly:before {
  content: "\e231";
}
.glyphicon-ice-lolly-tasted:before {
  content: "\e232";
}
.glyphicon-education:before {
  content: "\e233";
}
.glyphicon-option-horizontal:before {
  content: "\e234";
}
.glyphicon-option-vertical:before {
  content: "\e235";
}
.glyphicon-menu-hamburger:before {
  content: "\e236";
}
.glyphicon-modal-window:before {
  content: "\e237";
}
.glyphicon-oil:before {
  content: "\e238";
}
.glyphicon-grain:before {
  content: "\e239";
}
.glyphicon-sunglasses:before {
  content: "\e240";
}
.glyphicon-text-size:before {
  content: "\e241";
}
.glyphicon-text-color:before {
  content: "\e242";
}
.glyphicon-text-background:before {
  content: "\e243";
}
.glyphicon-object-align-top:before {
  content: "\e244";
}
.glyphicon-object-align-bottom:before {
  content: "\e245";
}
.glyphicon-object-align-horizontal:before {
  content: "\e246";
}
.glyphicon-object-align-left:before {
  content: "\e247";
}
.glyphicon-object-align-vertical:before {
  content: "\e248";
}
.glyphicon-object-align-right:before {
  content: "\e249";
}
.glyphicon-triangle-right:before {
  content: "\e250";
}
.glyphicon-triangle-left:before {
  content: "\e251";
}
.glyphicon-triangle-bottom:before {
  content: "\e252";
}
.glyphicon-triangle-top:before {
  content: "\e253";
}
.glyphicon-console:before {
  content: "\e254";
}
.glyphicon-superscript:before {
  content: "\e255";
}
.glyphicon-subscript:before {
  content: "\e256";
}
.glyphicon-menu-left:before {
  content: "\e257";
}
.glyphicon-menu-right:before {
  content: "\e258";
}
.glyphicon-menu-down:before {
  content: "\e259";
}
.glyphicon-menu-up:before {
  content: "\e260";
}
* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
*:before,
*:after {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
html {
  font-size: 10px;
  -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
}
body {
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 13px;
  line-height: 1.42857143;
  color: #000;
  background-color: #fff;
}
input,
button,
select,
textarea {
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
}
a {
  color: #337ab7;
  text-decoration: none;
}
a:hover,
a:focus {
  color: #23527c;
  text-decoration: underline;
}
a:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
figure {
  margin: 0;
}
img {
  vertical-align: middle;
}
.img-responsive,
.thumbnail > img,
.thumbnail a > img,
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  display: block;
  max-width: 100%;
  height: auto;
}
.img-rounded {
  border-radius: 3px;
}
.img-thumbnail {
  padding: 4px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: all 0.2s ease-in-out;
  -o-transition: all 0.2s ease-in-out;
  transition: all 0.2s ease-in-out;
  display: inline-block;
  max-width: 100%;
  height: auto;
}
.img-circle {
  border-radius: 50%;
}
hr {
  margin-top: 18px;
  margin-bottom: 18px;
  border: 0;
  border-top: 1px solid #eeeeee;
}
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  margin: -1px;
  padding: 0;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
[role="button"] {
  cursor: pointer;
}
h1,
h2,
h3,
h4,
h5,
h6,
.h1,
.h2,
.h3,
.h4,
.h5,
.h6 {
  font-family: inherit;
  font-weight: 500;
  line-height: 1.1;
  color: inherit;
}
h1 small,
h2 small,
h3 small,
h4 small,
h5 small,
h6 small,
.h1 small,
.h2 small,
.h3 small,
.h4 small,
.h5 small,
.h6 small,
h1 .small,
h2 .small,
h3 .small,
h4 .small,
h5 .small,
h6 .small,
.h1 .small,
.h2 .small,
.h3 .small,
.h4 .small,
.h5 .small,
.h6 .small {
  font-weight: normal;
  line-height: 1;
  color: #777777;
}
h1,
.h1,
h2,
.h2,
h3,
.h3 {
  margin-top: 18px;
  margin-bottom: 9px;
}
h1 small,
.h1 small,
h2 small,
.h2 small,
h3 small,
.h3 small,
h1 .small,
.h1 .small,
h2 .small,
.h2 .small,
h3 .small,
.h3 .small {
  font-size: 65%;
}
h4,
.h4,
h5,
.h5,
h6,
.h6 {
  margin-top: 9px;
  margin-bottom: 9px;
}
h4 small,
.h4 small,
h5 small,
.h5 small,
h6 small,
.h6 small,
h4 .small,
.h4 .small,
h5 .small,
.h5 .small,
h6 .small,
.h6 .small {
  font-size: 75%;
}
h1,
.h1 {
  font-size: 33px;
}
h2,
.h2 {
  font-size: 27px;
}
h3,
.h3 {
  font-size: 23px;
}
h4,
.h4 {
  font-size: 17px;
}
h5,
.h5 {
  font-size: 13px;
}
h6,
.h6 {
  font-size: 12px;
}
p {
  margin: 0 0 9px;
}
.lead {
  margin-bottom: 18px;
  font-size: 14px;
  font-weight: 300;
  line-height: 1.4;
}
@media (min-width: 768px) {
  .lead {
    font-size: 19.5px;
  }
}
small,
.small {
  font-size: 92%;
}
mark,
.mark {
  background-color: #fcf8e3;
  padding: .2em;
}
.text-left {
  text-align: left;
}
.text-right {
  text-align: right;
}
.text-center {
  text-align: center;
}
.text-justify {
  text-align: justify;
}
.text-nowrap {
  white-space: nowrap;
}
.text-lowercase {
  text-transform: lowercase;
}
.text-uppercase {
  text-transform: uppercase;
}
.text-capitalize {
  text-transform: capitalize;
}
.text-muted {
  color: #777777;
}
.text-primary {
  color: #337ab7;
}
a.text-primary:hover,
a.text-primary:focus {
  color: #286090;
}
.text-success {
  color: #3c763d;
}
a.text-success:hover,
a.text-success:focus {
  color: #2b542c;
}
.text-info {
  color: #31708f;
}
a.text-info:hover,
a.text-info:focus {
  color: #245269;
}
.text-warning {
  color: #8a6d3b;
}
a.text-warning:hover,
a.text-warning:focus {
  color: #66512c;
}
.text-danger {
  color: #a94442;
}
a.text-danger:hover,
a.text-danger:focus {
  color: #843534;
}
.bg-primary {
  color: #fff;
  background-color: #337ab7;
}
a.bg-primary:hover,
a.bg-primary:focus {
  background-color: #286090;
}
.bg-success {
  background-color: #dff0d8;
}
a.bg-success:hover,
a.bg-success:focus {
  background-color: #c1e2b3;
}
.bg-info {
  background-color: #d9edf7;
}
a.bg-info:hover,
a.bg-info:focus {
  background-color: #afd9ee;
}
.bg-warning {
  background-color: #fcf8e3;
}
a.bg-warning:hover,
a.bg-warning:focus {
  background-color: #f7ecb5;
}
.bg-danger {
  background-color: #f2dede;
}
a.bg-danger:hover,
a.bg-danger:focus {
  background-color: #e4b9b9;
}
.page-header {
  padding-bottom: 8px;
  margin: 36px 0 18px;
  border-bottom: 1px solid #eeeeee;
}
ul,
ol {
  margin-top: 0;
  margin-bottom: 9px;
}
ul ul,
ol ul,
ul ol,
ol ol {
  margin-bottom: 0;
}
.list-unstyled {
  padding-left: 0;
  list-style: none;
}
.list-inline {
  padding-left: 0;
  list-style: none;
  margin-left: -5px;
}
.list-inline > li {
  display: inline-block;
  padding-left: 5px;
  padding-right: 5px;
}
dl {
  margin-top: 0;
  margin-bottom: 18px;
}
dt,
dd {
  line-height: 1.42857143;
}
dt {
  font-weight: bold;
}
dd {
  margin-left: 0;
}
@media (min-width: 541px) {
  .dl-horizontal dt {
    float: left;
    width: 160px;
    clear: left;
    text-align: right;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
  }
  .dl-horizontal dd {
    margin-left: 180px;
  }
}
abbr[title],
abbr[data-original-title] {
  cursor: help;
  border-bottom: 1px dotted #777777;
}
.initialism {
  font-size: 90%;
  text-transform: uppercase;
}
blockquote {
  padding: 9px 18px;
  margin: 0 0 18px;
  font-size: inherit;
  border-left: 5px solid #eeeeee;
}
blockquote p:last-child,
blockquote ul:last-child,
blockquote ol:last-child {
  margin-bottom: 0;
}
blockquote footer,
blockquote small,
blockquote .small {
  display: block;
  font-size: 80%;
  line-height: 1.42857143;
  color: #777777;
}
blockquote footer:before,
blockquote small:before,
blockquote .small:before {
  content: '\2014 \00A0';
}
.blockquote-reverse,
blockquote.pull-right {
  padding-right: 15px;
  padding-left: 0;
  border-right: 5px solid #eeeeee;
  border-left: 0;
  text-align: right;
}
.blockquote-reverse footer:before,
blockquote.pull-right footer:before,
.blockquote-reverse small:before,
blockquote.pull-right small:before,
.blockquote-reverse .small:before,
blockquote.pull-right .small:before {
  content: '';
}
.blockquote-reverse footer:after,
blockquote.pull-right footer:after,
.blockquote-reverse small:after,
blockquote.pull-right small:after,
.blockquote-reverse .small:after,
blockquote.pull-right .small:after {
  content: '\00A0 \2014';
}
address {
  margin-bottom: 18px;
  font-style: normal;
  line-height: 1.42857143;
}
code,
kbd,
pre,
samp {
  font-family: monospace;
}
code {
  padding: 2px 4px;
  font-size: 90%;
  color: #c7254e;
  background-color: #f9f2f4;
  border-radius: 2px;
}
kbd {
  padding: 2px 4px;
  font-size: 90%;
  color: #888;
  background-color: transparent;
  border-radius: 1px;
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
}
kbd kbd {
  padding: 0;
  font-size: 100%;
  font-weight: bold;
  box-shadow: none;
}
pre {
  display: block;
  padding: 8.5px;
  margin: 0 0 9px;
  font-size: 12px;
  line-height: 1.42857143;
  word-break: break-all;
  word-wrap: break-word;
  color: #333333;
  background-color: #f5f5f5;
  border: 1px solid #ccc;
  border-radius: 2px;
}
pre code {
  padding: 0;
  font-size: inherit;
  color: inherit;
  white-space: pre-wrap;
  background-color: transparent;
  border-radius: 0;
}
.pre-scrollable {
  max-height: 340px;
  overflow-y: scroll;
}
.container {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
@media (min-width: 768px) {
  .container {
    width: 768px;
  }
}
@media (min-width: 992px) {
  .container {
    width: 940px;
  }
}
@media (min-width: 1200px) {
  .container {
    width: 1140px;
  }
}
.container-fluid {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
.row {
  margin-left: 0px;
  margin-right: 0px;
}
.col-xs-1, .col-sm-1, .col-md-1, .col-lg-1, .col-xs-2, .col-sm-2, .col-md-2, .col-lg-2, .col-xs-3, .col-sm-3, .col-md-3, .col-lg-3, .col-xs-4, .col-sm-4, .col-md-4, .col-lg-4, .col-xs-5, .col-sm-5, .col-md-5, .col-lg-5, .col-xs-6, .col-sm-6, .col-md-6, .col-lg-6, .col-xs-7, .col-sm-7, .col-md-7, .col-lg-7, .col-xs-8, .col-sm-8, .col-md-8, .col-lg-8, .col-xs-9, .col-sm-9, .col-md-9, .col-lg-9, .col-xs-10, .col-sm-10, .col-md-10, .col-lg-10, .col-xs-11, .col-sm-11, .col-md-11, .col-lg-11, .col-xs-12, .col-sm-12, .col-md-12, .col-lg-12 {
  position: relative;
  min-height: 1px;
  padding-left: 0px;
  padding-right: 0px;
}
.col-xs-1, .col-xs-2, .col-xs-3, .col-xs-4, .col-xs-5, .col-xs-6, .col-xs-7, .col-xs-8, .col-xs-9, .col-xs-10, .col-xs-11, .col-xs-12 {
  float: left;
}
.col-xs-12 {
  width: 100%;
}
.col-xs-11 {
  width: 91.66666667%;
}
.col-xs-10 {
  width: 83.33333333%;
}
.col-xs-9 {
  width: 75%;
}
.col-xs-8 {
  width: 66.66666667%;
}
.col-xs-7 {
  width: 58.33333333%;
}
.col-xs-6 {
  width: 50%;
}
.col-xs-5 {
  width: 41.66666667%;
}
.col-xs-4 {
  width: 33.33333333%;
}
.col-xs-3 {
  width: 25%;
}
.col-xs-2 {
  width: 16.66666667%;
}
.col-xs-1 {
  width: 8.33333333%;
}
.col-xs-pull-12 {
  right: 100%;
}
.col-xs-pull-11 {
  right: 91.66666667%;
}
.col-xs-pull-10 {
  right: 83.33333333%;
}
.col-xs-pull-9 {
  right: 75%;
}
.col-xs-pull-8 {
  right: 66.66666667%;
}
.col-xs-pull-7 {
  right: 58.33333333%;
}
.col-xs-pull-6 {
  right: 50%;
}
.col-xs-pull-5 {
  right: 41.66666667%;
}
.col-xs-pull-4 {
  right: 33.33333333%;
}
.col-xs-pull-3 {
  right: 25%;
}
.col-xs-pull-2 {
  right: 16.66666667%;
}
.col-xs-pull-1 {
  right: 8.33333333%;
}
.col-xs-pull-0 {
  right: auto;
}
.col-xs-push-12 {
  left: 100%;
}
.col-xs-push-11 {
  left: 91.66666667%;
}
.col-xs-push-10 {
  left: 83.33333333%;
}
.col-xs-push-9 {
  left: 75%;
}
.col-xs-push-8 {
  left: 66.66666667%;
}
.col-xs-push-7 {
  left: 58.33333333%;
}
.col-xs-push-6 {
  left: 50%;
}
.col-xs-push-5 {
  left: 41.66666667%;
}
.col-xs-push-4 {
  left: 33.33333333%;
}
.col-xs-push-3 {
  left: 25%;
}
.col-xs-push-2 {
  left: 16.66666667%;
}
.col-xs-push-1 {
  left: 8.33333333%;
}
.col-xs-push-0 {
  left: auto;
}
.col-xs-offset-12 {
  margin-left: 100%;
}
.col-xs-offset-11 {
  margin-left: 91.66666667%;
}
.col-xs-offset-10 {
  margin-left: 83.33333333%;
}
.col-xs-offset-9 {
  margin-left: 75%;
}
.col-xs-offset-8 {
  margin-left: 66.66666667%;
}
.col-xs-offset-7 {
  margin-left: 58.33333333%;
}
.col-xs-offset-6 {
  margin-left: 50%;
}
.col-xs-offset-5 {
  margin-left: 41.66666667%;
}
.col-xs-offset-4 {
  margin-left: 33.33333333%;
}
.col-xs-offset-3 {
  margin-left: 25%;
}
.col-xs-offset-2 {
  margin-left: 16.66666667%;
}
.col-xs-offset-1 {
  margin-left: 8.33333333%;
}
.col-xs-offset-0 {
  margin-left: 0%;
}
@media (min-width: 768px) {
  .col-sm-1, .col-sm-2, .col-sm-3, .col-sm-4, .col-sm-5, .col-sm-6, .col-sm-7, .col-sm-8, .col-sm-9, .col-sm-10, .col-sm-11, .col-sm-12 {
    float: left;
  }
  .col-sm-12 {
    width: 100%;
  }
  .col-sm-11 {
    width: 91.66666667%;
  }
  .col-sm-10 {
    width: 83.33333333%;
  }
  .col-sm-9 {
    width: 75%;
  }
  .col-sm-8 {
    width: 66.66666667%;
  }
  .col-sm-7 {
    width: 58.33333333%;
  }
  .col-sm-6 {
    width: 50%;
  }
  .col-sm-5 {
    width: 41.66666667%;
  }
  .col-sm-4 {
    width: 33.33333333%;
  }
  .col-sm-3 {
    width: 25%;
  }
  .col-sm-2 {
    width: 16.66666667%;
  }
  .col-sm-1 {
    width: 8.33333333%;
  }
  .col-sm-pull-12 {
    right: 100%;
  }
  .col-sm-pull-11 {
    right: 91.66666667%;
  }
  .col-sm-pull-10 {
    right: 83.33333333%;
  }
  .col-sm-pull-9 {
    right: 75%;
  }
  .col-sm-pull-8 {
    right: 66.66666667%;
  }
  .col-sm-pull-7 {
    right: 58.33333333%;
  }
  .col-sm-pull-6 {
    right: 50%;
  }
  .col-sm-pull-5 {
    right: 41.66666667%;
  }
  .col-sm-pull-4 {
    right: 33.33333333%;
  }
  .col-sm-pull-3 {
    right: 25%;
  }
  .col-sm-pull-2 {
    right: 16.66666667%;
  }
  .col-sm-pull-1 {
    right: 8.33333333%;
  }
  .col-sm-pull-0 {
    right: auto;
  }
  .col-sm-push-12 {
    left: 100%;
  }
  .col-sm-push-11 {
    left: 91.66666667%;
  }
  .col-sm-push-10 {
    left: 83.33333333%;
  }
  .col-sm-push-9 {
    left: 75%;
  }
  .col-sm-push-8 {
    left: 66.66666667%;
  }
  .col-sm-push-7 {
    left: 58.33333333%;
  }
  .col-sm-push-6 {
    left: 50%;
  }
  .col-sm-push-5 {
    left: 41.66666667%;
  }
  .col-sm-push-4 {
    left: 33.33333333%;
  }
  .col-sm-push-3 {
    left: 25%;
  }
  .col-sm-push-2 {
    left: 16.66666667%;
  }
  .col-sm-push-1 {
    left: 8.33333333%;
  }
  .col-sm-push-0 {
    left: auto;
  }
  .col-sm-offset-12 {
    margin-left: 100%;
  }
  .col-sm-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-sm-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-sm-offset-9 {
    margin-left: 75%;
  }
  .col-sm-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-sm-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-sm-offset-6 {
    margin-left: 50%;
  }
  .col-sm-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-sm-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-sm-offset-3 {
    margin-left: 25%;
  }
  .col-sm-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-sm-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-sm-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 992px) {
  .col-md-1, .col-md-2, .col-md-3, .col-md-4, .col-md-5, .col-md-6, .col-md-7, .col-md-8, .col-md-9, .col-md-10, .col-md-11, .col-md-12 {
    float: left;
  }
  .col-md-12 {
    width: 100%;
  }
  .col-md-11 {
    width: 91.66666667%;
  }
  .col-md-10 {
    width: 83.33333333%;
  }
  .col-md-9 {
    width: 75%;
  }
  .col-md-8 {
    width: 66.66666667%;
  }
  .col-md-7 {
    width: 58.33333333%;
  }
  .col-md-6 {
    width: 50%;
  }
  .col-md-5 {
    width: 41.66666667%;
  }
  .col-md-4 {
    width: 33.33333333%;
  }
  .col-md-3 {
    width: 25%;
  }
  .col-md-2 {
    width: 16.66666667%;
  }
  .col-md-1 {
    width: 8.33333333%;
  }
  .col-md-pull-12 {
    right: 100%;
  }
  .col-md-pull-11 {
    right: 91.66666667%;
  }
  .col-md-pull-10 {
    right: 83.33333333%;
  }
  .col-md-pull-9 {
    right: 75%;
  }
  .col-md-pull-8 {
    right: 66.66666667%;
  }
  .col-md-pull-7 {
    right: 58.33333333%;
  }
  .col-md-pull-6 {
    right: 50%;
  }
  .col-md-pull-5 {
    right: 41.66666667%;
  }
  .col-md-pull-4 {
    right: 33.33333333%;
  }
  .col-md-pull-3 {
    right: 25%;
  }
  .col-md-pull-2 {
    right: 16.66666667%;
  }
  .col-md-pull-1 {
    right: 8.33333333%;
  }
  .col-md-pull-0 {
    right: auto;
  }
  .col-md-push-12 {
    left: 100%;
  }
  .col-md-push-11 {
    left: 91.66666667%;
  }
  .col-md-push-10 {
    left: 83.33333333%;
  }
  .col-md-push-9 {
    left: 75%;
  }
  .col-md-push-8 {
    left: 66.66666667%;
  }
  .col-md-push-7 {
    left: 58.33333333%;
  }
  .col-md-push-6 {
    left: 50%;
  }
  .col-md-push-5 {
    left: 41.66666667%;
  }
  .col-md-push-4 {
    left: 33.33333333%;
  }
  .col-md-push-3 {
    left: 25%;
  }
  .col-md-push-2 {
    left: 16.66666667%;
  }
  .col-md-push-1 {
    left: 8.33333333%;
  }
  .col-md-push-0 {
    left: auto;
  }
  .col-md-offset-12 {
    margin-left: 100%;
  }
  .col-md-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-md-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-md-offset-9 {
    margin-left: 75%;
  }
  .col-md-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-md-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-md-offset-6 {
    margin-left: 50%;
  }
  .col-md-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-md-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-md-offset-3 {
    margin-left: 25%;
  }
  .col-md-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-md-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-md-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 1200px) {
  .col-lg-1, .col-lg-2, .col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg-7, .col-lg-8, .col-lg-9, .col-lg-10, .col-lg-11, .col-lg-12 {
    float: left;
  }
  .col-lg-12 {
    width: 100%;
  }
  .col-lg-11 {
    width: 91.66666667%;
  }
  .col-lg-10 {
    width: 83.33333333%;
  }
  .col-lg-9 {
    width: 75%;
  }
  .col-lg-8 {
    width: 66.66666667%;
  }
  .col-lg-7 {
    width: 58.33333333%;
  }
  .col-lg-6 {
    width: 50%;
  }
  .col-lg-5 {
    width: 41.66666667%;
  }
  .col-lg-4 {
    width: 33.33333333%;
  }
  .col-lg-3 {
    width: 25%;
  }
  .col-lg-2 {
    width: 16.66666667%;
  }
  .col-lg-1 {
    width: 8.33333333%;
  }
  .col-lg-pull-12 {
    right: 100%;
  }
  .col-lg-pull-11 {
    right: 91.66666667%;
  }
  .col-lg-pull-10 {
    right: 83.33333333%;
  }
  .col-lg-pull-9 {
    right: 75%;
  }
  .col-lg-pull-8 {
    right: 66.66666667%;
  }
  .col-lg-pull-7 {
    right: 58.33333333%;
  }
  .col-lg-pull-6 {
    right: 50%;
  }
  .col-lg-pull-5 {
    right: 41.66666667%;
  }
  .col-lg-pull-4 {
    right: 33.33333333%;
  }
  .col-lg-pull-3 {
    right: 25%;
  }
  .col-lg-pull-2 {
    right: 16.66666667%;
  }
  .col-lg-pull-1 {
    right: 8.33333333%;
  }
  .col-lg-pull-0 {
    right: auto;
  }
  .col-lg-push-12 {
    left: 100%;
  }
  .col-lg-push-11 {
    left: 91.66666667%;
  }
  .col-lg-push-10 {
    left: 83.33333333%;
  }
  .col-lg-push-9 {
    left: 75%;
  }
  .col-lg-push-8 {
    left: 66.66666667%;
  }
  .col-lg-push-7 {
    left: 58.33333333%;
  }
  .col-lg-push-6 {
    left: 50%;
  }
  .col-lg-push-5 {
    left: 41.66666667%;
  }
  .col-lg-push-4 {
    left: 33.33333333%;
  }
  .col-lg-push-3 {
    left: 25%;
  }
  .col-lg-push-2 {
    left: 16.66666667%;
  }
  .col-lg-push-1 {
    left: 8.33333333%;
  }
  .col-lg-push-0 {
    left: auto;
  }
  .col-lg-offset-12 {
    margin-left: 100%;
  }
  .col-lg-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-lg-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-lg-offset-9 {
    margin-left: 75%;
  }
  .col-lg-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-lg-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-lg-offset-6 {
    margin-left: 50%;
  }
  .col-lg-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-lg-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-lg-offset-3 {
    margin-left: 25%;
  }
  .col-lg-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-lg-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-lg-offset-0 {
    margin-left: 0%;
  }
}
table {
  background-color: transparent;
}
caption {
  padding-top: 8px;
  padding-bottom: 8px;
  color: #777777;
  text-align: left;
}
th {
  text-align: left;
}
.table {
  width: 100%;
  max-width: 100%;
  margin-bottom: 18px;
}
.table > thead > tr > th,
.table > tbody > tr > th,
.table > tfoot > tr > th,
.table > thead > tr > td,
.table > tbody > tr > td,
.table > tfoot > tr > td {
  padding: 8px;
  line-height: 1.42857143;
  vertical-align: top;
  border-top: 1px solid #ddd;
}
.table > thead > tr > th {
  vertical-align: bottom;
  border-bottom: 2px solid #ddd;
}
.table > caption + thead > tr:first-child > th,
.table > colgroup + thead > tr:first-child > th,
.table > thead:first-child > tr:first-child > th,
.table > caption + thead > tr:first-child > td,
.table > colgroup + thead > tr:first-child > td,
.table > thead:first-child > tr:first-child > td {
  border-top: 0;
}
.table > tbody + tbody {
  border-top: 2px solid #ddd;
}
.table .table {
  background-color: #fff;
}
.table-condensed > thead > tr > th,
.table-condensed > tbody > tr > th,
.table-condensed > tfoot > tr > th,
.table-condensed > thead > tr > td,
.table-condensed > tbody > tr > td,
.table-condensed > tfoot > tr > td {
  padding: 5px;
}
.table-bordered {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > tbody > tr > th,
.table-bordered > tfoot > tr > th,
.table-bordered > thead > tr > td,
.table-bordered > tbody > tr > td,
.table-bordered > tfoot > tr > td {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > thead > tr > td {
  border-bottom-width: 2px;
}
.table-striped > tbody > tr:nth-of-type(odd) {
  background-color: #f9f9f9;
}
.table-hover > tbody > tr:hover {
  background-color: #f5f5f5;
}
table col[class*="col-"] {
  position: static;
  float: none;
  display: table-column;
}
table td[class*="col-"],
table th[class*="col-"] {
  position: static;
  float: none;
  display: table-cell;
}
.table > thead > tr > td.active,
.table > tbody > tr > td.active,
.table > tfoot > tr > td.active,
.table > thead > tr > th.active,
.table > tbody > tr > th.active,
.table > tfoot > tr > th.active,
.table > thead > tr.active > td,
.table > tbody > tr.active > td,
.table > tfoot > tr.active > td,
.table > thead > tr.active > th,
.table > tbody > tr.active > th,
.table > tfoot > tr.active > th {
  background-color: #f5f5f5;
}
.table-hover > tbody > tr > td.active:hover,
.table-hover > tbody > tr > th.active:hover,
.table-hover > tbody > tr.active:hover > td,
.table-hover > tbody > tr:hover > .active,
.table-hover > tbody > tr.active:hover > th {
  background-color: #e8e8e8;
}
.table > thead > tr > td.success,
.table > tbody > tr > td.success,
.table > tfoot > tr > td.success,
.table > thead > tr > th.success,
.table > tbody > tr > th.success,
.table > tfoot > tr > th.success,
.table > thead > tr.success > td,
.table > tbody > tr.success > td,
.table > tfoot > tr.success > td,
.table > thead > tr.success > th,
.table > tbody > tr.success > th,
.table > tfoot > tr.success > th {
  background-color: #dff0d8;
}
.table-hover > tbody > tr > td.success:hover,
.table-hover > tbody > tr > th.success:hover,
.table-hover > tbody > tr.success:hover > td,
.table-hover > tbody > tr:hover > .success,
.table-hover > tbody > tr.success:hover > th {
  background-color: #d0e9c6;
}
.table > thead > tr > td.info,
.table > tbody > tr > td.info,
.table > tfoot > tr > td.info,
.table > thead > tr > th.info,
.table > tbody > tr > th.info,
.table > tfoot > tr > th.info,
.table > thead > tr.info > td,
.table > tbody > tr.info > td,
.table > tfoot > tr.info > td,
.table > thead > tr.info > th,
.table > tbody > tr.info > th,
.table > tfoot > tr.info > th {
  background-color: #d9edf7;
}
.table-hover > tbody > tr > td.info:hover,
.table-hover > tbody > tr > th.info:hover,
.table-hover > tbody > tr.info:hover > td,
.table-hover > tbody > tr:hover > .info,
.table-hover > tbody > tr.info:hover > th {
  background-color: #c4e3f3;
}
.table > thead > tr > td.warning,
.table > tbody > tr > td.warning,
.table > tfoot > tr > td.warning,
.table > thead > tr > th.warning,
.table > tbody > tr > th.warning,
.table > tfoot > tr > th.warning,
.table > thead > tr.warning > td,
.table > tbody > tr.warning > td,
.table > tfoot > tr.warning > td,
.table > thead > tr.warning > th,
.table > tbody > tr.warning > th,
.table > tfoot > tr.warning > th {
  background-color: #fcf8e3;
}
.table-hover > tbody > tr > td.warning:hover,
.table-hover > tbody > tr > th.warning:hover,
.table-hover > tbody > tr.warning:hover > td,
.table-hover > tbody > tr:hover > .warning,
.table-hover > tbody > tr.warning:hover > th {
  background-color: #faf2cc;
}
.table > thead > tr > td.danger,
.table > tbody > tr > td.danger,
.table > tfoot > tr > td.danger,
.table > thead > tr > th.danger,
.table > tbody > tr > th.danger,
.table > tfoot > tr > th.danger,
.table > thead > tr.danger > td,
.table > tbody > tr.danger > td,
.table > tfoot > tr.danger > td,
.table > thead > tr.danger > th,
.table > tbody > tr.danger > th,
.table > tfoot > tr.danger > th {
  background-color: #f2dede;
}
.table-hover > tbody > tr > td.danger:hover,
.table-hover > tbody > tr > th.danger:hover,
.table-hover > tbody > tr.danger:hover > td,
.table-hover > tbody > tr:hover > .danger,
.table-hover > tbody > tr.danger:hover > th {
  background-color: #ebcccc;
}
.table-responsive {
  overflow-x: auto;
  min-height: 0.01%;
}
@media screen and (max-width: 767px) {
  .table-responsive {
    width: 100%;
    margin-bottom: 13.5px;
    overflow-y: hidden;
    -ms-overflow-style: -ms-autohiding-scrollbar;
    border: 1px solid #ddd;
  }
  .table-responsive > .table {
    margin-bottom: 0;
  }
  .table-responsive > .table > thead > tr > th,
  .table-responsive > .table > tbody > tr > th,
  .table-responsive > .table > tfoot > tr > th,
  .table-responsive > .table > thead > tr > td,
  .table-responsive > .table > tbody > tr > td,
  .table-responsive > .table > tfoot > tr > td {
    white-space: nowrap;
  }
  .table-responsive > .table-bordered {
    border: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:first-child,
  .table-responsive > .table-bordered > tbody > tr > th:first-child,
  .table-responsive > .table-bordered > tfoot > tr > th:first-child,
  .table-responsive > .table-bordered > thead > tr > td:first-child,
  .table-responsive > .table-bordered > tbody > tr > td:first-child,
  .table-responsive > .table-bordered > tfoot > tr > td:first-child {
    border-left: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:last-child,
  .table-responsive > .table-bordered > tbody > tr > th:last-child,
  .table-responsive > .table-bordered > tfoot > tr > th:last-child,
  .table-responsive > .table-bordered > thead > tr > td:last-child,
  .table-responsive > .table-bordered > tbody > tr > td:last-child,
  .table-responsive > .table-bordered > tfoot > tr > td:last-child {
    border-right: 0;
  }
  .table-responsive > .table-bordered > tbody > tr:last-child > th,
  .table-responsive > .table-bordered > tfoot > tr:last-child > th,
  .table-responsive > .table-bordered > tbody > tr:last-child > td,
  .table-responsive > .table-bordered > tfoot > tr:last-child > td {
    border-bottom: 0;
  }
}
fieldset {
  padding: 0;
  margin: 0;
  border: 0;
  min-width: 0;
}
legend {
  display: block;
  width: 100%;
  padding: 0;
  margin-bottom: 18px;
  font-size: 19.5px;
  line-height: inherit;
  color: #333333;
  border: 0;
  border-bottom: 1px solid #e5e5e5;
}
label {
  display: inline-block;
  max-width: 100%;
  margin-bottom: 5px;
  font-weight: bold;
}
input[type="search"] {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
input[type="radio"],
input[type="checkbox"] {
  margin: 4px 0 0;
  margin-top: 1px \9;
  line-height: normal;
}
input[type="file"] {
  display: block;
}
input[type="range"] {
  display: block;
  width: 100%;
}
select[multiple],
select[size] {
  height: auto;
}
input[type="file"]:focus,
input[type="radio"]:focus,
input[type="checkbox"]:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
output {
  display: block;
  padding-top: 7px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
}
.form-control {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
}
.form-control:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.form-control::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.form-control:-ms-input-placeholder {
  color: #999;
}
.form-control::-webkit-input-placeholder {
  color: #999;
}
.form-control::-ms-expand {
  border: 0;
  background-color: transparent;
}
.form-control[disabled],
.form-control[readonly],
fieldset[disabled] .form-control {
  background-color: #eeeeee;
  opacity: 1;
}
.form-control[disabled],
fieldset[disabled] .form-control {
  cursor: not-allowed;
}
textarea.form-control {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: none;
}
@media screen and (-webkit-min-device-pixel-ratio: 0) {
  input[type="date"].form-control,
  input[type="time"].form-control,
  input[type="datetime-local"].form-control,
  input[type="month"].form-control {
    line-height: 32px;
  }
  input[type="date"].input-sm,
  input[type="time"].input-sm,
  input[type="datetime-local"].input-sm,
  input[type="month"].input-sm,
  .input-group-sm input[type="date"],
  .input-group-sm input[type="time"],
  .input-group-sm input[type="datetime-local"],
  .input-group-sm input[type="month"] {
    line-height: 30px;
  }
  input[type="date"].input-lg,
  input[type="time"].input-lg,
  input[type="datetime-local"].input-lg,
  input[type="month"].input-lg,
  .input-group-lg input[type="date"],
  .input-group-lg input[type="time"],
  .input-group-lg input[type="datetime-local"],
  .input-group-lg input[type="month"] {
    line-height: 45px;
  }
}
.form-group {
  margin-bottom: 15px;
}
.radio,
.checkbox {
  position: relative;
  display: block;
  margin-top: 10px;
  margin-bottom: 10px;
}
.radio label,
.checkbox label {
  min-height: 18px;
  padding-left: 20px;
  margin-bottom: 0;
  font-weight: normal;
  cursor: pointer;
}
.radio input[type="radio"],
.radio-inline input[type="radio"],
.checkbox input[type="checkbox"],
.checkbox-inline input[type="checkbox"] {
  position: absolute;
  margin-left: -20px;
  margin-top: 4px \9;
}
.radio + .radio,
.checkbox + .checkbox {
  margin-top: -5px;
}
.radio-inline,
.checkbox-inline {
  position: relative;
  display: inline-block;
  padding-left: 20px;
  margin-bottom: 0;
  vertical-align: middle;
  font-weight: normal;
  cursor: pointer;
}
.radio-inline + .radio-inline,
.checkbox-inline + .checkbox-inline {
  margin-top: 0;
  margin-left: 10px;
}
input[type="radio"][disabled],
input[type="checkbox"][disabled],
input[type="radio"].disabled,
input[type="checkbox"].disabled,
fieldset[disabled] input[type="radio"],
fieldset[disabled] input[type="checkbox"] {
  cursor: not-allowed;
}
.radio-inline.disabled,
.checkbox-inline.disabled,
fieldset[disabled] .radio-inline,
fieldset[disabled] .checkbox-inline {
  cursor: not-allowed;
}
.radio.disabled label,
.checkbox.disabled label,
fieldset[disabled] .radio label,
fieldset[disabled] .checkbox label {
  cursor: not-allowed;
}
.form-control-static {
  padding-top: 7px;
  padding-bottom: 7px;
  margin-bottom: 0;
  min-height: 31px;
}
.form-control-static.input-lg,
.form-control-static.input-sm {
  padding-left: 0;
  padding-right: 0;
}
.input-sm {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-sm {
  height: 30px;
  line-height: 30px;
}
textarea.input-sm,
select[multiple].input-sm {
  height: auto;
}
.form-group-sm .form-control {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.form-group-sm select.form-control {
  height: 30px;
  line-height: 30px;
}
.form-group-sm textarea.form-control,
.form-group-sm select[multiple].form-control {
  height: auto;
}
.form-group-sm .form-control-static {
  height: 30px;
  min-height: 30px;
  padding: 6px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.input-lg {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-lg {
  height: 45px;
  line-height: 45px;
}
textarea.input-lg,
select[multiple].input-lg {
  height: auto;
}
.form-group-lg .form-control {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.form-group-lg select.form-control {
  height: 45px;
  line-height: 45px;
}
.form-group-lg textarea.form-control,
.form-group-lg select[multiple].form-control {
  height: auto;
}
.form-group-lg .form-control-static {
  height: 45px;
  min-height: 35px;
  padding: 11px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.has-feedback {
  position: relative;
}
.has-feedback .form-control {
  padding-right: 40px;
}
.form-control-feedback {
  position: absolute;
  top: 0;
  right: 0;
  z-index: 2;
  display: block;
  width: 32px;
  height: 32px;
  line-height: 32px;
  text-align: center;
  pointer-events: none;
}
.input-lg + .form-control-feedback,
.input-group-lg + .form-control-feedback,
.form-group-lg .form-control + .form-control-feedback {
  width: 45px;
  height: 45px;
  line-height: 45px;
}
.input-sm + .form-control-feedback,
.input-group-sm + .form-control-feedback,
.form-group-sm .form-control + .form-control-feedback {
  width: 30px;
  height: 30px;
  line-height: 30px;
}
.has-success .help-block,
.has-success .control-label,
.has-success .radio,
.has-success .checkbox,
.has-success .radio-inline,
.has-success .checkbox-inline,
.has-success.radio label,
.has-success.checkbox label,
.has-success.radio-inline label,
.has-success.checkbox-inline label {
  color: #3c763d;
}
.has-success .form-control {
  border-color: #3c763d;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-success .form-control:focus {
  border-color: #2b542c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
}
.has-success .input-group-addon {
  color: #3c763d;
  border-color: #3c763d;
  background-color: #dff0d8;
}
.has-success .form-control-feedback {
  color: #3c763d;
}
.has-warning .help-block,
.has-warning .control-label,
.has-warning .radio,
.has-warning .checkbox,
.has-warning .radio-inline,
.has-warning .checkbox-inline,
.has-warning.radio label,
.has-warning.checkbox label,
.has-warning.radio-inline label,
.has-warning.checkbox-inline label {
  color: #8a6d3b;
}
.has-warning .form-control {
  border-color: #8a6d3b;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-warning .form-control:focus {
  border-color: #66512c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
}
.has-warning .input-group-addon {
  color: #8a6d3b;
  border-color: #8a6d3b;
  background-color: #fcf8e3;
}
.has-warning .form-control-feedback {
  color: #8a6d3b;
}
.has-error .help-block,
.has-error .control-label,
.has-error .radio,
.has-error .checkbox,
.has-error .radio-inline,
.has-error .checkbox-inline,
.has-error.radio label,
.has-error.checkbox label,
.has-error.radio-inline label,
.has-error.checkbox-inline label {
  color: #a94442;
}
.has-error .form-control {
  border-color: #a94442;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-error .form-control:focus {
  border-color: #843534;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
}
.has-error .input-group-addon {
  color: #a94442;
  border-color: #a94442;
  background-color: #f2dede;
}
.has-error .form-control-feedback {
  color: #a94442;
}
.has-feedback label ~ .form-control-feedback {
  top: 23px;
}
.has-feedback label.sr-only ~ .form-control-feedback {
  top: 0;
}
.help-block {
  display: block;
  margin-top: 5px;
  margin-bottom: 10px;
  color: #404040;
}
@media (min-width: 768px) {
  .form-inline .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .form-inline .form-control-static {
    display: inline-block;
  }
  .form-inline .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .form-inline .input-group .input-group-addon,
  .form-inline .input-group .input-group-btn,
  .form-inline .input-group .form-control {
    width: auto;
  }
  .form-inline .input-group > .form-control {
    width: 100%;
  }
  .form-inline .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio,
  .form-inline .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio label,
  .form-inline .checkbox label {
    padding-left: 0;
  }
  .form-inline .radio input[type="radio"],
  .form-inline .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .form-inline .has-feedback .form-control-feedback {
    top: 0;
  }
}
.form-horizontal .radio,
.form-horizontal .checkbox,
.form-horizontal .radio-inline,
.form-horizontal .checkbox-inline {
  margin-top: 0;
  margin-bottom: 0;
  padding-top: 7px;
}
.form-horizontal .radio,
.form-horizontal .checkbox {
  min-height: 25px;
}
.form-horizontal .form-group {
  margin-left: 0px;
  margin-right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .control-label {
    text-align: right;
    margin-bottom: 0;
    padding-top: 7px;
  }
}
.form-horizontal .has-feedback .form-control-feedback {
  right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .form-group-lg .control-label {
    padding-top: 11px;
    font-size: 17px;
  }
}
@media (min-width: 768px) {
  .form-horizontal .form-group-sm .control-label {
    padding-top: 6px;
    font-size: 12px;
  }
}
.btn {
  display: inline-block;
  margin-bottom: 0;
  font-weight: normal;
  text-align: center;
  vertical-align: middle;
  touch-action: manipulation;
  cursor: pointer;
  background-image: none;
  border: 1px solid transparent;
  white-space: nowrap;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  border-radius: 2px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.btn:focus,
.btn:active:focus,
.btn.active:focus,
.btn.focus,
.btn:active.focus,
.btn.active.focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
.btn:hover,
.btn:focus,
.btn.focus {
  color: #333;
  text-decoration: none;
}
.btn:active,
.btn.active {
  outline: 0;
  background-image: none;
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn.disabled,
.btn[disabled],
fieldset[disabled] .btn {
  cursor: not-allowed;
  opacity: 0.65;
  filter: alpha(opacity=65);
  -webkit-box-shadow: none;
  box-shadow: none;
}
a.btn.disabled,
fieldset[disabled] a.btn {
  pointer-events: none;
}
.btn-default {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.btn-default:focus,
.btn-default.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.btn-default:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active:hover,
.btn-default.active:hover,
.open > .dropdown-toggle.btn-default:hover,
.btn-default:active:focus,
.btn-default.active:focus,
.open > .dropdown-toggle.btn-default:focus,
.btn-default:active.focus,
.btn-default.active.focus,
.open > .dropdown-toggle.btn-default.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  background-image: none;
}
.btn-default.disabled:hover,
.btn-default[disabled]:hover,
fieldset[disabled] .btn-default:hover,
.btn-default.disabled:focus,
.btn-default[disabled]:focus,
fieldset[disabled] .btn-default:focus,
.btn-default.disabled.focus,
.btn-default[disabled].focus,
fieldset[disabled] .btn-default.focus {
  background-color: #fff;
  border-color: #ccc;
}
.btn-default .badge {
  color: #fff;
  background-color: #333;
}
.btn-primary {
  color: #fff;
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary:focus,
.btn-primary.focus {
  color: #fff;
  background-color: #286090;
  border-color: #122b40;
}
.btn-primary:hover {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active:hover,
.btn-primary.active:hover,
.open > .dropdown-toggle.btn-primary:hover,
.btn-primary:active:focus,
.btn-primary.active:focus,
.open > .dropdown-toggle.btn-primary:focus,
.btn-primary:active.focus,
.btn-primary.active.focus,
.open > .dropdown-toggle.btn-primary.focus {
  color: #fff;
  background-color: #204d74;
  border-color: #122b40;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  background-image: none;
}
.btn-primary.disabled:hover,
.btn-primary[disabled]:hover,
fieldset[disabled] .btn-primary:hover,
.btn-primary.disabled:focus,
.btn-primary[disabled]:focus,
fieldset[disabled] .btn-primary:focus,
.btn-primary.disabled.focus,
.btn-primary[disabled].focus,
fieldset[disabled] .btn-primary.focus {
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary .badge {
  color: #337ab7;
  background-color: #fff;
}
.btn-success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success:focus,
.btn-success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.btn-success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active:hover,
.btn-success.active:hover,
.open > .dropdown-toggle.btn-success:hover,
.btn-success:active:focus,
.btn-success.active:focus,
.open > .dropdown-toggle.btn-success:focus,
.btn-success:active.focus,
.btn-success.active.focus,
.open > .dropdown-toggle.btn-success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  background-image: none;
}
.btn-success.disabled:hover,
.btn-success[disabled]:hover,
fieldset[disabled] .btn-success:hover,
.btn-success.disabled:focus,
.btn-success[disabled]:focus,
fieldset[disabled] .btn-success:focus,
.btn-success.disabled.focus,
.btn-success[disabled].focus,
fieldset[disabled] .btn-success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.btn-info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info:focus,
.btn-info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.btn-info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active:hover,
.btn-info.active:hover,
.open > .dropdown-toggle.btn-info:hover,
.btn-info:active:focus,
.btn-info.active:focus,
.open > .dropdown-toggle.btn-info:focus,
.btn-info:active.focus,
.btn-info.active.focus,
.open > .dropdown-toggle.btn-info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  background-image: none;
}
.btn-info.disabled:hover,
.btn-info[disabled]:hover,
fieldset[disabled] .btn-info:hover,
.btn-info.disabled:focus,
.btn-info[disabled]:focus,
fieldset[disabled] .btn-info:focus,
.btn-info.disabled.focus,
.btn-info[disabled].focus,
fieldset[disabled] .btn-info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.btn-warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning:focus,
.btn-warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.btn-warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active:hover,
.btn-warning.active:hover,
.open > .dropdown-toggle.btn-warning:hover,
.btn-warning:active:focus,
.btn-warning.active:focus,
.open > .dropdown-toggle.btn-warning:focus,
.btn-warning:active.focus,
.btn-warning.active.focus,
.open > .dropdown-toggle.btn-warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  background-image: none;
}
.btn-warning.disabled:hover,
.btn-warning[disabled]:hover,
fieldset[disabled] .btn-warning:hover,
.btn-warning.disabled:focus,
.btn-warning[disabled]:focus,
fieldset[disabled] .btn-warning:focus,
.btn-warning.disabled.focus,
.btn-warning[disabled].focus,
fieldset[disabled] .btn-warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.btn-danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger:focus,
.btn-danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.btn-danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active:hover,
.btn-danger.active:hover,
.open > .dropdown-toggle.btn-danger:hover,
.btn-danger:active:focus,
.btn-danger.active:focus,
.open > .dropdown-toggle.btn-danger:focus,
.btn-danger:active.focus,
.btn-danger.active.focus,
.open > .dropdown-toggle.btn-danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  background-image: none;
}
.btn-danger.disabled:hover,
.btn-danger[disabled]:hover,
fieldset[disabled] .btn-danger:hover,
.btn-danger.disabled:focus,
.btn-danger[disabled]:focus,
fieldset[disabled] .btn-danger:focus,
.btn-danger.disabled.focus,
.btn-danger[disabled].focus,
fieldset[disabled] .btn-danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger .badge {
  color: #d9534f;
  background-color: #fff;
}
.btn-link {
  color: #337ab7;
  font-weight: normal;
  border-radius: 0;
}
.btn-link,
.btn-link:active,
.btn-link.active,
.btn-link[disabled],
fieldset[disabled] .btn-link {
  background-color: transparent;
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn-link,
.btn-link:hover,
.btn-link:focus,
.btn-link:active {
  border-color: transparent;
}
.btn-link:hover,
.btn-link:focus {
  color: #23527c;
  text-decoration: underline;
  background-color: transparent;
}
.btn-link[disabled]:hover,
fieldset[disabled] .btn-link:hover,
.btn-link[disabled]:focus,
fieldset[disabled] .btn-link:focus {
  color: #777777;
  text-decoration: none;
}
.btn-lg,
.btn-group-lg > .btn {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.btn-sm,
.btn-group-sm > .btn {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-xs,
.btn-group-xs > .btn {
  padding: 1px 5px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-block {
  display: block;
  width: 100%;
}
.btn-block + .btn-block {
  margin-top: 5px;
}
input[type="submit"].btn-block,
input[type="reset"].btn-block,
input[type="button"].btn-block {
  width: 100%;
}
.fade {
  opacity: 0;
  -webkit-transition: opacity 0.15s linear;
  -o-transition: opacity 0.15s linear;
  transition: opacity 0.15s linear;
}
.fade.in {
  opacity: 1;
}
.collapse {
  display: none;
}
.collapse.in {
  display: block;
}
tr.collapse.in {
  display: table-row;
}
tbody.collapse.in {
  display: table-row-group;
}
.collapsing {
  position: relative;
  height: 0;
  overflow: hidden;
  -webkit-transition-property: height, visibility;
  transition-property: height, visibility;
  -webkit-transition-duration: 0.35s;
  transition-duration: 0.35s;
  -webkit-transition-timing-function: ease;
  transition-timing-function: ease;
}
.caret {
  display: inline-block;
  width: 0;
  height: 0;
  margin-left: 2px;
  vertical-align: middle;
  border-top: 4px dashed;
  border-top: 4px solid \9;
  border-right: 4px solid transparent;
  border-left: 4px solid transparent;
}
.dropup,
.dropdown {
  position: relative;
}
.dropdown-toggle:focus {
  outline: 0;
}
.dropdown-menu {
  position: absolute;
  top: 100%;
  left: 0;
  z-index: 1000;
  display: none;
  float: left;
  min-width: 160px;
  padding: 5px 0;
  margin: 2px 0 0;
  list-style: none;
  font-size: 13px;
  text-align: left;
  background-color: #fff;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.15);
  border-radius: 2px;
  -webkit-box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  background-clip: padding-box;
}
.dropdown-menu.pull-right {
  right: 0;
  left: auto;
}
.dropdown-menu .divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.dropdown-menu > li > a {
  display: block;
  padding: 3px 20px;
  clear: both;
  font-weight: normal;
  line-height: 1.42857143;
  color: #333333;
  white-space: nowrap;
}
.dropdown-menu > li > a:hover,
.dropdown-menu > li > a:focus {
  text-decoration: none;
  color: #262626;
  background-color: #f5f5f5;
}
.dropdown-menu > .active > a,
.dropdown-menu > .active > a:hover,
.dropdown-menu > .active > a:focus {
  color: #fff;
  text-decoration: none;
  outline: 0;
  background-color: #337ab7;
}
.dropdown-menu > .disabled > a,
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  color: #777777;
}
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  text-decoration: none;
  background-color: transparent;
  background-image: none;
  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
  cursor: not-allowed;
}
.open > .dropdown-menu {
  display: block;
}
.open > a {
  outline: 0;
}
.dropdown-menu-right {
  left: auto;
  right: 0;
}
.dropdown-menu-left {
  left: 0;
  right: auto;
}
.dropdown-header {
  display: block;
  padding: 3px 20px;
  font-size: 12px;
  line-height: 1.42857143;
  color: #777777;
  white-space: nowrap;
}
.dropdown-backdrop {
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  top: 0;
  z-index: 990;
}
.pull-right > .dropdown-menu {
  right: 0;
  left: auto;
}
.dropup .caret,
.navbar-fixed-bottom .dropdown .caret {
  border-top: 0;
  border-bottom: 4px dashed;
  border-bottom: 4px solid \9;
  content: "";
}
.dropup .dropdown-menu,
.navbar-fixed-bottom .dropdown .dropdown-menu {
  top: auto;
  bottom: 100%;
  margin-bottom: 2px;
}
@media (min-width: 541px) {
  .navbar-right .dropdown-menu {
    left: auto;
    right: 0;
  }
  .navbar-right .dropdown-menu-left {
    left: 0;
    right: auto;
  }
}
.btn-group,
.btn-group-vertical {
  position: relative;
  display: inline-block;
  vertical-align: middle;
}
.btn-group > .btn,
.btn-group-vertical > .btn {
  position: relative;
  float: left;
}
.btn-group > .btn:hover,
.btn-group-vertical > .btn:hover,
.btn-group > .btn:focus,
.btn-group-vertical > .btn:focus,
.btn-group > .btn:active,
.btn-group-vertical > .btn:active,
.btn-group > .btn.active,
.btn-group-vertical > .btn.active {
  z-index: 2;
}
.btn-group .btn + .btn,
.btn-group .btn + .btn-group,
.btn-group .btn-group + .btn,
.btn-group .btn-group + .btn-group {
  margin-left: -1px;
}
.btn-toolbar {
  margin-left: -5px;
}
.btn-toolbar .btn,
.btn-toolbar .btn-group,
.btn-toolbar .input-group {
  float: left;
}
.btn-toolbar > .btn,
.btn-toolbar > .btn-group,
.btn-toolbar > .input-group {
  margin-left: 5px;
}
.btn-group > .btn:not(:first-child):not(:last-child):not(.dropdown-toggle) {
  border-radius: 0;
}
.btn-group > .btn:first-child {
  margin-left: 0;
}
.btn-group > .btn:first-child:not(:last-child):not(.dropdown-toggle) {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn:last-child:not(:first-child),
.btn-group > .dropdown-toggle:not(:first-child) {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group > .btn-group {
  float: left;
}
.btn-group > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group .dropdown-toggle:active,
.btn-group.open .dropdown-toggle {
  outline: 0;
}
.btn-group > .btn + .dropdown-toggle {
  padding-left: 8px;
  padding-right: 8px;
}
.btn-group > .btn-lg + .dropdown-toggle {
  padding-left: 12px;
  padding-right: 12px;
}
.btn-group.open .dropdown-toggle {
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn-group.open .dropdown-toggle.btn-link {
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn .caret {
  margin-left: 0;
}
.btn-lg .caret {
  border-width: 5px 5px 0;
  border-bottom-width: 0;
}
.dropup .btn-lg .caret {
  border-width: 0 5px 5px;
}
.btn-group-vertical > .btn,
.btn-group-vertical > .btn-group,
.btn-group-vertical > .btn-group > .btn {
  display: block;
  float: none;
  width: 100%;
  max-width: 100%;
}
.btn-group-vertical > .btn-group > .btn {
  float: none;
}
.btn-group-vertical > .btn + .btn,
.btn-group-vertical > .btn + .btn-group,
.btn-group-vertical > .btn-group + .btn,
.btn-group-vertical > .btn-group + .btn-group {
  margin-top: -1px;
  margin-left: 0;
}
.btn-group-vertical > .btn:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.btn-group-vertical > .btn:first-child:not(:last-child) {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn:last-child:not(:first-child) {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
.btn-group-vertical > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.btn-group-justified {
  display: table;
  width: 100%;
  table-layout: fixed;
  border-collapse: separate;
}
.btn-group-justified > .btn,
.btn-group-justified > .btn-group {
  float: none;
  display: table-cell;
  width: 1%;
}
.btn-group-justified > .btn-group .btn {
  width: 100%;
}
.btn-group-justified > .btn-group .dropdown-menu {
  left: auto;
}
[data-toggle="buttons"] > .btn input[type="radio"],
[data-toggle="buttons"] > .btn-group > .btn input[type="radio"],
[data-toggle="buttons"] > .btn input[type="checkbox"],
[data-toggle="buttons"] > .btn-group > .btn input[type="checkbox"] {
  position: absolute;
  clip: rect(0, 0, 0, 0);
  pointer-events: none;
}
.input-group {
  position: relative;
  display: table;
  border-collapse: separate;
}
.input-group[class*="col-"] {
  float: none;
  padding-left: 0;
  padding-right: 0;
}
.input-group .form-control {
  position: relative;
  z-index: 2;
  float: left;
  width: 100%;
  margin-bottom: 0;
}
.input-group .form-control:focus {
  z-index: 3;
}
.input-group-lg > .form-control,
.input-group-lg > .input-group-addon,
.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-group-lg > .form-control,
select.input-group-lg > .input-group-addon,
select.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  line-height: 45px;
}
textarea.input-group-lg > .form-control,
textarea.input-group-lg > .input-group-addon,
textarea.input-group-lg > .input-group-btn > .btn,
select[multiple].input-group-lg > .form-control,
select[multiple].input-group-lg > .input-group-addon,
select[multiple].input-group-lg > .input-group-btn > .btn {
  height: auto;
}
.input-group-sm > .form-control,
.input-group-sm > .input-group-addon,
.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-group-sm > .form-control,
select.input-group-sm > .input-group-addon,
select.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  line-height: 30px;
}
textarea.input-group-sm > .form-control,
textarea.input-group-sm > .input-group-addon,
textarea.input-group-sm > .input-group-btn > .btn,
select[multiple].input-group-sm > .form-control,
select[multiple].input-group-sm > .input-group-addon,
select[multiple].input-group-sm > .input-group-btn > .btn {
  height: auto;
}
.input-group-addon,
.input-group-btn,
.input-group .form-control {
  display: table-cell;
}
.input-group-addon:not(:first-child):not(:last-child),
.input-group-btn:not(:first-child):not(:last-child),
.input-group .form-control:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.input-group-addon,
.input-group-btn {
  width: 1%;
  white-space: nowrap;
  vertical-align: middle;
}
.input-group-addon {
  padding: 6px 12px;
  font-size: 13px;
  font-weight: normal;
  line-height: 1;
  color: #555555;
  text-align: center;
  background-color: #eeeeee;
  border: 1px solid #ccc;
  border-radius: 2px;
}
.input-group-addon.input-sm {
  padding: 5px 10px;
  font-size: 12px;
  border-radius: 1px;
}
.input-group-addon.input-lg {
  padding: 10px 16px;
  font-size: 17px;
  border-radius: 3px;
}
.input-group-addon input[type="radio"],
.input-group-addon input[type="checkbox"] {
  margin-top: 0;
}
.input-group .form-control:first-child,
.input-group-addon:first-child,
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group > .btn,
.input-group-btn:first-child > .dropdown-toggle,
.input-group-btn:last-child > .btn:not(:last-child):not(.dropdown-toggle),
.input-group-btn:last-child > .btn-group:not(:last-child) > .btn {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.input-group-addon:first-child {
  border-right: 0;
}
.input-group .form-control:last-child,
.input-group-addon:last-child,
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group > .btn,
.input-group-btn:last-child > .dropdown-toggle,
.input-group-btn:first-child > .btn:not(:first-child),
.input-group-btn:first-child > .btn-group:not(:first-child) > .btn {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.input-group-addon:last-child {
  border-left: 0;
}
.input-group-btn {
  position: relative;
  font-size: 0;
  white-space: nowrap;
}
.input-group-btn > .btn {
  position: relative;
}
.input-group-btn > .btn + .btn {
  margin-left: -1px;
}
.input-group-btn > .btn:hover,
.input-group-btn > .btn:focus,
.input-group-btn > .btn:active {
  z-index: 2;
}
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group {
  margin-right: -1px;
}
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group {
  z-index: 2;
  margin-left: -1px;
}
.nav {
  margin-bottom: 0;
  padding-left: 0;
  list-style: none;
}
.nav > li {
  position: relative;
  display: block;
}
.nav > li > a {
  position: relative;
  display: block;
  padding: 10px 15px;
}
.nav > li > a:hover,
.nav > li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.nav > li.disabled > a {
  color: #777777;
}
.nav > li.disabled > a:hover,
.nav > li.disabled > a:focus {
  color: #777777;
  text-decoration: none;
  background-color: transparent;
  cursor: not-allowed;
}
.nav .open > a,
.nav .open > a:hover,
.nav .open > a:focus {
  background-color: #eeeeee;
  border-color: #337ab7;
}
.nav .nav-divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.nav > li > a > img {
  max-width: none;
}
.nav-tabs {
  border-bottom: 1px solid #ddd;
}
.nav-tabs > li {
  float: left;
  margin-bottom: -1px;
}
.nav-tabs > li > a {
  margin-right: 2px;
  line-height: 1.42857143;
  border: 1px solid transparent;
  border-radius: 2px 2px 0 0;
}
.nav-tabs > li > a:hover {
  border-color: #eeeeee #eeeeee #ddd;
}
.nav-tabs > li.active > a,
.nav-tabs > li.active > a:hover,
.nav-tabs > li.active > a:focus {
  color: #555555;
  background-color: #fff;
  border: 1px solid #ddd;
  border-bottom-color: transparent;
  cursor: default;
}
.nav-tabs.nav-justified {
  width: 100%;
  border-bottom: 0;
}
.nav-tabs.nav-justified > li {
  float: none;
}
.nav-tabs.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-tabs.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-tabs.nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs.nav-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs.nav-justified > .active > a,
.nav-tabs.nav-justified > .active > a:hover,
.nav-tabs.nav-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs.nav-justified > .active > a,
  .nav-tabs.nav-justified > .active > a:hover,
  .nav-tabs.nav-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.nav-pills > li {
  float: left;
}
.nav-pills > li > a {
  border-radius: 2px;
}
.nav-pills > li + li {
  margin-left: 2px;
}
.nav-pills > li.active > a,
.nav-pills > li.active > a:hover,
.nav-pills > li.active > a:focus {
  color: #fff;
  background-color: #337ab7;
}
.nav-stacked > li {
  float: none;
}
.nav-stacked > li + li {
  margin-top: 2px;
  margin-left: 0;
}
.nav-justified {
  width: 100%;
}
.nav-justified > li {
  float: none;
}
.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs-justified {
  border-bottom: 0;
}
.nav-tabs-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs-justified > .active > a,
.nav-tabs-justified > .active > a:hover,
.nav-tabs-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs-justified > .active > a,
  .nav-tabs-justified > .active > a:hover,
  .nav-tabs-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.tab-content > .tab-pane {
  display: none;
}
.tab-content > .active {
  display: block;
}
.nav-tabs .dropdown-menu {
  margin-top: -1px;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar {
  position: relative;
  min-height: 30px;
  margin-bottom: 18px;
  border: 1px solid transparent;
}
@media (min-width: 541px) {
  .navbar {
    border-radius: 2px;
  }
}
@media (min-width: 541px) {
  .navbar-header {
    float: left;
  }
}
.navbar-collapse {
  overflow-x: visible;
  padding-right: 0px;
  padding-left: 0px;
  border-top: 1px solid transparent;
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1);
  -webkit-overflow-scrolling: touch;
}
.navbar-collapse.in {
  overflow-y: auto;
}
@media (min-width: 541px) {
  .navbar-collapse {
    width: auto;
    border-top: 0;
    box-shadow: none;
  }
  .navbar-collapse.collapse {
    display: block !important;
    height: auto !important;
    padding-bottom: 0;
    overflow: visible !important;
  }
  .navbar-collapse.in {
    overflow-y: visible;
  }
  .navbar-fixed-top .navbar-collapse,
  .navbar-static-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    padding-left: 0;
    padding-right: 0;
  }
}
.navbar-fixed-top .navbar-collapse,
.navbar-fixed-bottom .navbar-collapse {
  max-height: 340px;
}
@media (max-device-width: 540px) and (orientation: landscape) {
  .navbar-fixed-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    max-height: 200px;
  }
}
.container > .navbar-header,
.container-fluid > .navbar-header,
.container > .navbar-collapse,
.container-fluid > .navbar-collapse {
  margin-right: 0px;
  margin-left: 0px;
}
@media (min-width: 541px) {
  .container > .navbar-header,
  .container-fluid > .navbar-header,
  .container > .navbar-collapse,
  .container-fluid > .navbar-collapse {
    margin-right: 0;
    margin-left: 0;
  }
}
.navbar-static-top {
  z-index: 1000;
  border-width: 0 0 1px;
}
@media (min-width: 541px) {
  .navbar-static-top {
    border-radius: 0;
  }
}
.navbar-fixed-top,
.navbar-fixed-bottom {
  position: fixed;
  right: 0;
  left: 0;
  z-index: 1030;
}
@media (min-width: 541px) {
  .navbar-fixed-top,
  .navbar-fixed-bottom {
    border-radius: 0;
  }
}
.navbar-fixed-top {
  top: 0;
  border-width: 0 0 1px;
}
.navbar-fixed-bottom {
  bottom: 0;
  margin-bottom: 0;
  border-width: 1px 0 0;
}
.navbar-brand {
  float: left;
  padding: 6px 0px;
  font-size: 17px;
  line-height: 18px;
  height: 30px;
}
.navbar-brand:hover,
.navbar-brand:focus {
  text-decoration: none;
}
.navbar-brand > img {
  display: block;
}
@media (min-width: 541px) {
  .navbar > .container .navbar-brand,
  .navbar > .container-fluid .navbar-brand {
    margin-left: 0px;
  }
}
.navbar-toggle {
  position: relative;
  float: right;
  margin-right: 0px;
  padding: 9px 10px;
  margin-top: -2px;
  margin-bottom: -2px;
  background-color: transparent;
  background-image: none;
  border: 1px solid transparent;
  border-radius: 2px;
}
.navbar-toggle:focus {
  outline: 0;
}
.navbar-toggle .icon-bar {
  display: block;
  width: 22px;
  height: 2px;
  border-radius: 1px;
}
.navbar-toggle .icon-bar + .icon-bar {
  margin-top: 4px;
}
@media (min-width: 541px) {
  .navbar-toggle {
    display: none;
  }
}
.navbar-nav {
  margin: 3px 0px;
}
.navbar-nav > li > a {
  padding-top: 10px;
  padding-bottom: 10px;
  line-height: 18px;
}
@media (max-width: 540px) {
  .navbar-nav .open .dropdown-menu {
    position: static;
    float: none;
    width: auto;
    margin-top: 0;
    background-color: transparent;
    border: 0;
    box-shadow: none;
  }
  .navbar-nav .open .dropdown-menu > li > a,
  .navbar-nav .open .dropdown-menu .dropdown-header {
    padding: 5px 15px 5px 25px;
  }
  .navbar-nav .open .dropdown-menu > li > a {
    line-height: 18px;
  }
  .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-nav .open .dropdown-menu > li > a:focus {
    background-image: none;
  }
}
@media (min-width: 541px) {
  .navbar-nav {
    float: left;
    margin: 0;
  }
  .navbar-nav > li {
    float: left;
  }
  .navbar-nav > li > a {
    padding-top: 6px;
    padding-bottom: 6px;
  }
}
.navbar-form {
  margin-left: 0px;
  margin-right: 0px;
  padding: 10px 0px;
  border-top: 1px solid transparent;
  border-bottom: 1px solid transparent;
  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  margin-top: -1px;
  margin-bottom: -1px;
}
@media (min-width: 768px) {
  .navbar-form .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .navbar-form .form-control-static {
    display: inline-block;
  }
  .navbar-form .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .navbar-form .input-group .input-group-addon,
  .navbar-form .input-group .input-group-btn,
  .navbar-form .input-group .form-control {
    width: auto;
  }
  .navbar-form .input-group > .form-control {
    width: 100%;
  }
  .navbar-form .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio,
  .navbar-form .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio label,
  .navbar-form .checkbox label {
    padding-left: 0;
  }
  .navbar-form .radio input[type="radio"],
  .navbar-form .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .navbar-form .has-feedback .form-control-feedback {
    top: 0;
  }
}
@media (max-width: 540px) {
  .navbar-form .form-group {
    margin-bottom: 5px;
  }
  .navbar-form .form-group:last-child {
    margin-bottom: 0;
  }
}
@media (min-width: 541px) {
  .navbar-form {
    width: auto;
    border: 0;
    margin-left: 0;
    margin-right: 0;
    padding-top: 0;
    padding-bottom: 0;
    -webkit-box-shadow: none;
    box-shadow: none;
  }
}
.navbar-nav > li > .dropdown-menu {
  margin-top: 0;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar-fixed-bottom .navbar-nav > li > .dropdown-menu {
  margin-bottom: 0;
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.navbar-btn {
  margin-top: -1px;
  margin-bottom: -1px;
}
.navbar-btn.btn-sm {
  margin-top: 0px;
  margin-bottom: 0px;
}
.navbar-btn.btn-xs {
  margin-top: 4px;
  margin-bottom: 4px;
}
.navbar-text {
  margin-top: 6px;
  margin-bottom: 6px;
}
@media (min-width: 541px) {
  .navbar-text {
    float: left;
    margin-left: 0px;
    margin-right: 0px;
  }
}
@media (min-width: 541px) {
  .navbar-left {
    float: left !important;
    float: left;
  }
  .navbar-right {
    float: right !important;
    float: right;
    margin-right: 0px;
  }
  .navbar-right ~ .navbar-right {
    margin-right: 0;
  }
}
.navbar-default {
  background-color: #f8f8f8;
  border-color: #e7e7e7;
}
.navbar-default .navbar-brand {
  color: #777;
}
.navbar-default .navbar-brand:hover,
.navbar-default .navbar-brand:focus {
  color: #5e5e5e;
  background-color: transparent;
}
.navbar-default .navbar-text {
  color: #777;
}
.navbar-default .navbar-nav > li > a {
  color: #777;
}
.navbar-default .navbar-nav > li > a:hover,
.navbar-default .navbar-nav > li > a:focus {
  color: #333;
  background-color: transparent;
}
.navbar-default .navbar-nav > .active > a,
.navbar-default .navbar-nav > .active > a:hover,
.navbar-default .navbar-nav > .active > a:focus {
  color: #555;
  background-color: #e7e7e7;
}
.navbar-default .navbar-nav > .disabled > a,
.navbar-default .navbar-nav > .disabled > a:hover,
.navbar-default .navbar-nav > .disabled > a:focus {
  color: #ccc;
  background-color: transparent;
}
.navbar-default .navbar-toggle {
  border-color: #ddd;
}
.navbar-default .navbar-toggle:hover,
.navbar-default .navbar-toggle:focus {
  background-color: #ddd;
}
.navbar-default .navbar-toggle .icon-bar {
  background-color: #888;
}
.navbar-default .navbar-collapse,
.navbar-default .navbar-form {
  border-color: #e7e7e7;
}
.navbar-default .navbar-nav > .open > a,
.navbar-default .navbar-nav > .open > a:hover,
.navbar-default .navbar-nav > .open > a:focus {
  background-color: #e7e7e7;
  color: #555;
}
@media (max-width: 540px) {
  .navbar-default .navbar-nav .open .dropdown-menu > li > a {
    color: #777;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #333;
    background-color: transparent;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #555;
    background-color: #e7e7e7;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #ccc;
    background-color: transparent;
  }
}
.navbar-default .navbar-link {
  color: #777;
}
.navbar-default .navbar-link:hover {
  color: #333;
}
.navbar-default .btn-link {
  color: #777;
}
.navbar-default .btn-link:hover,
.navbar-default .btn-link:focus {
  color: #333;
}
.navbar-default .btn-link[disabled]:hover,
fieldset[disabled] .navbar-default .btn-link:hover,
.navbar-default .btn-link[disabled]:focus,
fieldset[disabled] .navbar-default .btn-link:focus {
  color: #ccc;
}
.navbar-inverse {
  background-color: #222;
  border-color: #080808;
}
.navbar-inverse .navbar-brand {
  color: #9d9d9d;
}
.navbar-inverse .navbar-brand:hover,
.navbar-inverse .navbar-brand:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-text {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a:hover,
.navbar-inverse .navbar-nav > li > a:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-nav > .active > a,
.navbar-inverse .navbar-nav > .active > a:hover,
.navbar-inverse .navbar-nav > .active > a:focus {
  color: #fff;
  background-color: #080808;
}
.navbar-inverse .navbar-nav > .disabled > a,
.navbar-inverse .navbar-nav > .disabled > a:hover,
.navbar-inverse .navbar-nav > .disabled > a:focus {
  color: #444;
  background-color: transparent;
}
.navbar-inverse .navbar-toggle {
  border-color: #333;
}
.navbar-inverse .navbar-toggle:hover,
.navbar-inverse .navbar-toggle:focus {
  background-color: #333;
}
.navbar-inverse .navbar-toggle .icon-bar {
  background-color: #fff;
}
.navbar-inverse .navbar-collapse,
.navbar-inverse .navbar-form {
  border-color: #101010;
}
.navbar-inverse .navbar-nav > .open > a,
.navbar-inverse .navbar-nav > .open > a:hover,
.navbar-inverse .navbar-nav > .open > a:focus {
  background-color: #080808;
  color: #fff;
}
@media (max-width: 540px) {
  .navbar-inverse .navbar-nav .open .dropdown-menu > .dropdown-header {
    border-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu .divider {
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a {
    color: #9d9d9d;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #fff;
    background-color: transparent;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #fff;
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #444;
    background-color: transparent;
  }
}
.navbar-inverse .navbar-link {
  color: #9d9d9d;
}
.navbar-inverse .navbar-link:hover {
  color: #fff;
}
.navbar-inverse .btn-link {
  color: #9d9d9d;
}
.navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link:focus {
  color: #fff;
}
.navbar-inverse .btn-link[disabled]:hover,
fieldset[disabled] .navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link[disabled]:focus,
fieldset[disabled] .navbar-inverse .btn-link:focus {
  color: #444;
}
.breadcrumb {
  padding: 8px 15px;
  margin-bottom: 18px;
  list-style: none;
  background-color: #f5f5f5;
  border-radius: 2px;
}
.breadcrumb > li {
  display: inline-block;
}
.breadcrumb > li + li:before {
  content: "/\00a0";
  padding: 0 5px;
  color: #5e5e5e;
}
.breadcrumb > .active {
  color: #777777;
}
.pagination {
  display: inline-block;
  padding-left: 0;
  margin: 18px 0;
  border-radius: 2px;
}
.pagination > li {
  display: inline;
}
.pagination > li > a,
.pagination > li > span {
  position: relative;
  float: left;
  padding: 6px 12px;
  line-height: 1.42857143;
  text-decoration: none;
  color: #337ab7;
  background-color: #fff;
  border: 1px solid #ddd;
  margin-left: -1px;
}
.pagination > li:first-child > a,
.pagination > li:first-child > span {
  margin-left: 0;
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.pagination > li:last-child > a,
.pagination > li:last-child > span {
  border-bottom-right-radius: 2px;
  border-top-right-radius: 2px;
}
.pagination > li > a:hover,
.pagination > li > span:hover,
.pagination > li > a:focus,
.pagination > li > span:focus {
  z-index: 2;
  color: #23527c;
  background-color: #eeeeee;
  border-color: #ddd;
}
.pagination > .active > a,
.pagination > .active > span,
.pagination > .active > a:hover,
.pagination > .active > span:hover,
.pagination > .active > a:focus,
.pagination > .active > span:focus {
  z-index: 3;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
  cursor: default;
}
.pagination > .disabled > span,
.pagination > .disabled > span:hover,
.pagination > .disabled > span:focus,
.pagination > .disabled > a,
.pagination > .disabled > a:hover,
.pagination > .disabled > a:focus {
  color: #777777;
  background-color: #fff;
  border-color: #ddd;
  cursor: not-allowed;
}
.pagination-lg > li > a,
.pagination-lg > li > span {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.pagination-lg > li:first-child > a,
.pagination-lg > li:first-child > span {
  border-bottom-left-radius: 3px;
  border-top-left-radius: 3px;
}
.pagination-lg > li:last-child > a,
.pagination-lg > li:last-child > span {
  border-bottom-right-radius: 3px;
  border-top-right-radius: 3px;
}
.pagination-sm > li > a,
.pagination-sm > li > span {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.pagination-sm > li:first-child > a,
.pagination-sm > li:first-child > span {
  border-bottom-left-radius: 1px;
  border-top-left-radius: 1px;
}
.pagination-sm > li:last-child > a,
.pagination-sm > li:last-child > span {
  border-bottom-right-radius: 1px;
  border-top-right-radius: 1px;
}
.pager {
  padding-left: 0;
  margin: 18px 0;
  list-style: none;
  text-align: center;
}
.pager li {
  display: inline;
}
.pager li > a,
.pager li > span {
  display: inline-block;
  padding: 5px 14px;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 15px;
}
.pager li > a:hover,
.pager li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.pager .next > a,
.pager .next > span {
  float: right;
}
.pager .previous > a,
.pager .previous > span {
  float: left;
}
.pager .disabled > a,
.pager .disabled > a:hover,
.pager .disabled > a:focus,
.pager .disabled > span {
  color: #777777;
  background-color: #fff;
  cursor: not-allowed;
}
.label {
  display: inline;
  padding: .2em .6em .3em;
  font-size: 75%;
  font-weight: bold;
  line-height: 1;
  color: #fff;
  text-align: center;
  white-space: nowrap;
  vertical-align: baseline;
  border-radius: .25em;
}
a.label:hover,
a.label:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.label:empty {
  display: none;
}
.btn .label {
  position: relative;
  top: -1px;
}
.label-default {
  background-color: #777777;
}
.label-default[href]:hover,
.label-default[href]:focus {
  background-color: #5e5e5e;
}
.label-primary {
  background-color: #337ab7;
}
.label-primary[href]:hover,
.label-primary[href]:focus {
  background-color: #286090;
}
.label-success {
  background-color: #5cb85c;
}
.label-success[href]:hover,
.label-success[href]:focus {
  background-color: #449d44;
}
.label-info {
  background-color: #5bc0de;
}
.label-info[href]:hover,
.label-info[href]:focus {
  background-color: #31b0d5;
}
.label-warning {
  background-color: #f0ad4e;
}
.label-warning[href]:hover,
.label-warning[href]:focus {
  background-color: #ec971f;
}
.label-danger {
  background-color: #d9534f;
}
.label-danger[href]:hover,
.label-danger[href]:focus {
  background-color: #c9302c;
}
.badge {
  display: inline-block;
  min-width: 10px;
  padding: 3px 7px;
  font-size: 12px;
  font-weight: bold;
  color: #fff;
  line-height: 1;
  vertical-align: middle;
  white-space: nowrap;
  text-align: center;
  background-color: #777777;
  border-radius: 10px;
}
.badge:empty {
  display: none;
}
.btn .badge {
  position: relative;
  top: -1px;
}
.btn-xs .badge,
.btn-group-xs > .btn .badge {
  top: 0;
  padding: 1px 5px;
}
a.badge:hover,
a.badge:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.list-group-item.active > .badge,
.nav-pills > .active > a > .badge {
  color: #337ab7;
  background-color: #fff;
}
.list-group-item > .badge {
  float: right;
}
.list-group-item > .badge + .badge {
  margin-right: 5px;
}
.nav-pills > li > a > .badge {
  margin-left: 3px;
}
.jumbotron {
  padding-top: 30px;
  padding-bottom: 30px;
  margin-bottom: 30px;
  color: inherit;
  background-color: #eeeeee;
}
.jumbotron h1,
.jumbotron .h1 {
  color: inherit;
}
.jumbotron p {
  margin-bottom: 15px;
  font-size: 20px;
  font-weight: 200;
}
.jumbotron > hr {
  border-top-color: #d5d5d5;
}
.container .jumbotron,
.container-fluid .jumbotron {
  border-radius: 3px;
  padding-left: 0px;
  padding-right: 0px;
}
.jumbotron .container {
  max-width: 100%;
}
@media screen and (min-width: 768px) {
  .jumbotron {
    padding-top: 48px;
    padding-bottom: 48px;
  }
  .container .jumbotron,
  .container-fluid .jumbotron {
    padding-left: 60px;
    padding-right: 60px;
  }
  .jumbotron h1,
  .jumbotron .h1 {
    font-size: 59px;
  }
}
.thumbnail {
  display: block;
  padding: 4px;
  margin-bottom: 18px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: border 0.2s ease-in-out;
  -o-transition: border 0.2s ease-in-out;
  transition: border 0.2s ease-in-out;
}
.thumbnail > img,
.thumbnail a > img {
  margin-left: auto;
  margin-right: auto;
}
a.thumbnail:hover,
a.thumbnail:focus,
a.thumbnail.active {
  border-color: #337ab7;
}
.thumbnail .caption {
  padding: 9px;
  color: #000;
}
.alert {
  padding: 15px;
  margin-bottom: 18px;
  border: 1px solid transparent;
  border-radius: 2px;
}
.alert h4 {
  margin-top: 0;
  color: inherit;
}
.alert .alert-link {
  font-weight: bold;
}
.alert > p,
.alert > ul {
  margin-bottom: 0;
}
.alert > p + p {
  margin-top: 5px;
}
.alert-dismissable,
.alert-dismissible {
  padding-right: 35px;
}
.alert-dismissable .close,
.alert-dismissible .close {
  position: relative;
  top: -2px;
  right: -21px;
  color: inherit;
}
.alert-success {
  background-color: #dff0d8;
  border-color: #d6e9c6;
  color: #3c763d;
}
.alert-success hr {
  border-top-color: #c9e2b3;
}
.alert-success .alert-link {
  color: #2b542c;
}
.alert-info {
  background-color: #d9edf7;
  border-color: #bce8f1;
  color: #31708f;
}
.alert-info hr {
  border-top-color: #a6e1ec;
}
.alert-info .alert-link {
  color: #245269;
}
.alert-warning {
  background-color: #fcf8e3;
  border-color: #faebcc;
  color: #8a6d3b;
}
.alert-warning hr {
  border-top-color: #f7e1b5;
}
.alert-warning .alert-link {
  color: #66512c;
}
.alert-danger {
  background-color: #f2dede;
  border-color: #ebccd1;
  color: #a94442;
}
.alert-danger hr {
  border-top-color: #e4b9c0;
}
.alert-danger .alert-link {
  color: #843534;
}
@-webkit-keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
@keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
.progress {
  overflow: hidden;
  height: 18px;
  margin-bottom: 18px;
  background-color: #f5f5f5;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
  box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
}
.progress-bar {
  float: left;
  width: 0%;
  height: 100%;
  font-size: 12px;
  line-height: 18px;
  color: #fff;
  text-align: center;
  background-color: #337ab7;
  -webkit-box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  -webkit-transition: width 0.6s ease;
  -o-transition: width 0.6s ease;
  transition: width 0.6s ease;
}
.progress-striped .progress-bar,
.progress-bar-striped {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-size: 40px 40px;
}
.progress.active .progress-bar,
.progress-bar.active {
  -webkit-animation: progress-bar-stripes 2s linear infinite;
  -o-animation: progress-bar-stripes 2s linear infinite;
  animation: progress-bar-stripes 2s linear infinite;
}
.progress-bar-success {
  background-color: #5cb85c;
}
.progress-striped .progress-bar-success {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-info {
  background-color: #5bc0de;
}
.progress-striped .progress-bar-info {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-warning {
  background-color: #f0ad4e;
}
.progress-striped .progress-bar-warning {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-danger {
  background-color: #d9534f;
}
.progress-striped .progress-bar-danger {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.media {
  margin-top: 15px;
}
.media:first-child {
  margin-top: 0;
}
.media,
.media-body {
  zoom: 1;
  overflow: hidden;
}
.media-body {
  width: 10000px;
}
.media-object {
  display: block;
}
.media-object.img-thumbnail {
  max-width: none;
}
.media-right,
.media > .pull-right {
  padding-left: 10px;
}
.media-left,
.media > .pull-left {
  padding-right: 10px;
}
.media-left,
.media-right,
.media-body {
  display: table-cell;
  vertical-align: top;
}
.media-middle {
  vertical-align: middle;
}
.media-bottom {
  vertical-align: bottom;
}
.media-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.media-list {
  padding-left: 0;
  list-style: none;
}
.list-group {
  margin-bottom: 20px;
  padding-left: 0;
}
.list-group-item {
  position: relative;
  display: block;
  padding: 10px 15px;
  margin-bottom: -1px;
  background-color: #fff;
  border: 1px solid #ddd;
}
.list-group-item:first-child {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
}
.list-group-item:last-child {
  margin-bottom: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
a.list-group-item,
button.list-group-item {
  color: #555;
}
a.list-group-item .list-group-item-heading,
button.list-group-item .list-group-item-heading {
  color: #333;
}
a.list-group-item:hover,
button.list-group-item:hover,
a.list-group-item:focus,
button.list-group-item:focus {
  text-decoration: none;
  color: #555;
  background-color: #f5f5f5;
}
button.list-group-item {
  width: 100%;
  text-align: left;
}
.list-group-item.disabled,
.list-group-item.disabled:hover,
.list-group-item.disabled:focus {
  background-color: #eeeeee;
  color: #777777;
  cursor: not-allowed;
}
.list-group-item.disabled .list-group-item-heading,
.list-group-item.disabled:hover .list-group-item-heading,
.list-group-item.disabled:focus .list-group-item-heading {
  color: inherit;
}
.list-group-item.disabled .list-group-item-text,
.list-group-item.disabled:hover .list-group-item-text,
.list-group-item.disabled:focus .list-group-item-text {
  color: #777777;
}
.list-group-item.active,
.list-group-item.active:hover,
.list-group-item.active:focus {
  z-index: 2;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.list-group-item.active .list-group-item-heading,
.list-group-item.active:hover .list-group-item-heading,
.list-group-item.active:focus .list-group-item-heading,
.list-group-item.active .list-group-item-heading > small,
.list-group-item.active:hover .list-group-item-heading > small,
.list-group-item.active:focus .list-group-item-heading > small,
.list-group-item.active .list-group-item-heading > .small,
.list-group-item.active:hover .list-group-item-heading > .small,
.list-group-item.active:focus .list-group-item-heading > .small {
  color: inherit;
}
.list-group-item.active .list-group-item-text,
.list-group-item.active:hover .list-group-item-text,
.list-group-item.active:focus .list-group-item-text {
  color: #c7ddef;
}
.list-group-item-success {
  color: #3c763d;
  background-color: #dff0d8;
}
a.list-group-item-success,
button.list-group-item-success {
  color: #3c763d;
}
a.list-group-item-success .list-group-item-heading,
button.list-group-item-success .list-group-item-heading {
  color: inherit;
}
a.list-group-item-success:hover,
button.list-group-item-success:hover,
a.list-group-item-success:focus,
button.list-group-item-success:focus {
  color: #3c763d;
  background-color: #d0e9c6;
}
a.list-group-item-success.active,
button.list-group-item-success.active,
a.list-group-item-success.active:hover,
button.list-group-item-success.active:hover,
a.list-group-item-success.active:focus,
button.list-group-item-success.active:focus {
  color: #fff;
  background-color: #3c763d;
  border-color: #3c763d;
}
.list-group-item-info {
  color: #31708f;
  background-color: #d9edf7;
}
a.list-group-item-info,
button.list-group-item-info {
  color: #31708f;
}
a.list-group-item-info .list-group-item-heading,
button.list-group-item-info .list-group-item-heading {
  color: inherit;
}
a.list-group-item-info:hover,
button.list-group-item-info:hover,
a.list-group-item-info:focus,
button.list-group-item-info:focus {
  color: #31708f;
  background-color: #c4e3f3;
}
a.list-group-item-info.active,
button.list-group-item-info.active,
a.list-group-item-info.active:hover,
button.list-group-item-info.active:hover,
a.list-group-item-info.active:focus,
button.list-group-item-info.active:focus {
  color: #fff;
  background-color: #31708f;
  border-color: #31708f;
}
.list-group-item-warning {
  color: #8a6d3b;
  background-color: #fcf8e3;
}
a.list-group-item-warning,
button.list-group-item-warning {
  color: #8a6d3b;
}
a.list-group-item-warning .list-group-item-heading,
button.list-group-item-warning .list-group-item-heading {
  color: inherit;
}
a.list-group-item-warning:hover,
button.list-group-item-warning:hover,
a.list-group-item-warning:focus,
button.list-group-item-warning:focus {
  color: #8a6d3b;
  background-color: #faf2cc;
}
a.list-group-item-warning.active,
button.list-group-item-warning.active,
a.list-group-item-warning.active:hover,
button.list-group-item-warning.active:hover,
a.list-group-item-warning.active:focus,
button.list-group-item-warning.active:focus {
  color: #fff;
  background-color: #8a6d3b;
  border-color: #8a6d3b;
}
.list-group-item-danger {
  color: #a94442;
  background-color: #f2dede;
}
a.list-group-item-danger,
button.list-group-item-danger {
  color: #a94442;
}
a.list-group-item-danger .list-group-item-heading,
button.list-group-item-danger .list-group-item-heading {
  color: inherit;
}
a.list-group-item-danger:hover,
button.list-group-item-danger:hover,
a.list-group-item-danger:focus,
button.list-group-item-danger:focus {
  color: #a94442;
  background-color: #ebcccc;
}
a.list-group-item-danger.active,
button.list-group-item-danger.active,
a.list-group-item-danger.active:hover,
button.list-group-item-danger.active:hover,
a.list-group-item-danger.active:focus,
button.list-group-item-danger.active:focus {
  color: #fff;
  background-color: #a94442;
  border-color: #a94442;
}
.list-group-item-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.list-group-item-text {
  margin-bottom: 0;
  line-height: 1.3;
}
.panel {
  margin-bottom: 18px;
  background-color: #fff;
  border: 1px solid transparent;
  border-radius: 2px;
  -webkit-box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
}
.panel-body {
  padding: 15px;
}
.panel-heading {
  padding: 10px 15px;
  border-bottom: 1px solid transparent;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel-heading > .dropdown .dropdown-toggle {
  color: inherit;
}
.panel-title {
  margin-top: 0;
  margin-bottom: 0;
  font-size: 15px;
  color: inherit;
}
.panel-title > a,
.panel-title > small,
.panel-title > .small,
.panel-title > small > a,
.panel-title > .small > a {
  color: inherit;
}
.panel-footer {
  padding: 10px 15px;
  background-color: #f5f5f5;
  border-top: 1px solid #ddd;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .list-group,
.panel > .panel-collapse > .list-group {
  margin-bottom: 0;
}
.panel > .list-group .list-group-item,
.panel > .panel-collapse > .list-group .list-group-item {
  border-width: 1px 0;
  border-radius: 0;
}
.panel > .list-group:first-child .list-group-item:first-child,
.panel > .panel-collapse > .list-group:first-child .list-group-item:first-child {
  border-top: 0;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .list-group:last-child .list-group-item:last-child,
.panel > .panel-collapse > .list-group:last-child .list-group-item:last-child {
  border-bottom: 0;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .panel-heading + .panel-collapse > .list-group .list-group-item:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.panel-heading + .list-group .list-group-item:first-child {
  border-top-width: 0;
}
.list-group + .panel-footer {
  border-top-width: 0;
}
.panel > .table,
.panel > .table-responsive > .table,
.panel > .panel-collapse > .table {
  margin-bottom: 0;
}
.panel > .table caption,
.panel > .table-responsive > .table caption,
.panel > .panel-collapse > .table caption {
  padding-left: 15px;
  padding-right: 15px;
}
.panel > .table:first-child,
.panel > .table-responsive:first-child > .table:first-child {
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child {
  border-top-left-radius: 1px;
  border-top-right-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:first-child {
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:last-child {
  border-top-right-radius: 1px;
}
.panel > .table:last-child,
.panel > .table-responsive:last-child > .table:last-child {
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child {
  border-bottom-left-radius: 1px;
  border-bottom-right-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:first-child {
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:last-child {
  border-bottom-right-radius: 1px;
}
.panel > .panel-body + .table,
.panel > .panel-body + .table-responsive,
.panel > .table + .panel-body,
.panel > .table-responsive + .panel-body {
  border-top: 1px solid #ddd;
}
.panel > .table > tbody:first-child > tr:first-child th,
.panel > .table > tbody:first-child > tr:first-child td {
  border-top: 0;
}
.panel > .table-bordered,
.panel > .table-responsive > .table-bordered {
  border: 0;
}
.panel > .table-bordered > thead > tr > th:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:first-child,
.panel > .table-bordered > tbody > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:first-child,
.panel > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-bordered > thead > tr > td:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:first-child,
.panel > .table-bordered > tbody > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:first-child,
.panel > .table-bordered > tfoot > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:first-child {
  border-left: 0;
}
.panel > .table-bordered > thead > tr > th:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:last-child,
.panel > .table-bordered > tbody > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:last-child,
.panel > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-bordered > thead > tr > td:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:last-child,
.panel > .table-bordered > tbody > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:last-child,
.panel > .table-bordered > tfoot > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:last-child {
  border-right: 0;
}
.panel > .table-bordered > thead > tr:first-child > td,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > td,
.panel > .table-bordered > tbody > tr:first-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > td,
.panel > .table-bordered > thead > tr:first-child > th,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > th,
.panel > .table-bordered > tbody > tr:first-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > th {
  border-bottom: 0;
}
.panel > .table-bordered > tbody > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > td,
.panel > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-bordered > tbody > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > th,
.panel > .table-bordered > tfoot > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > th {
  border-bottom: 0;
}
.panel > .table-responsive {
  border: 0;
  margin-bottom: 0;
}
.panel-group {
  margin-bottom: 18px;
}
.panel-group .panel {
  margin-bottom: 0;
  border-radius: 2px;
}
.panel-group .panel + .panel {
  margin-top: 5px;
}
.panel-group .panel-heading {
  border-bottom: 0;
}
.panel-group .panel-heading + .panel-collapse > .panel-body,
.panel-group .panel-heading + .panel-collapse > .list-group {
  border-top: 1px solid #ddd;
}
.panel-group .panel-footer {
  border-top: 0;
}
.panel-group .panel-footer + .panel-collapse .panel-body {
  border-bottom: 1px solid #ddd;
}
.panel-default {
  border-color: #ddd;
}
.panel-default > .panel-heading {
  color: #333333;
  background-color: #f5f5f5;
  border-color: #ddd;
}
.panel-default > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ddd;
}
.panel-default > .panel-heading .badge {
  color: #f5f5f5;
  background-color: #333333;
}
.panel-default > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ddd;
}
.panel-primary {
  border-color: #337ab7;
}
.panel-primary > .panel-heading {
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.panel-primary > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #337ab7;
}
.panel-primary > .panel-heading .badge {
  color: #337ab7;
  background-color: #fff;
}
.panel-primary > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #337ab7;
}
.panel-success {
  border-color: #d6e9c6;
}
.panel-success > .panel-heading {
  color: #3c763d;
  background-color: #dff0d8;
  border-color: #d6e9c6;
}
.panel-success > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #d6e9c6;
}
.panel-success > .panel-heading .badge {
  color: #dff0d8;
  background-color: #3c763d;
}
.panel-success > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #d6e9c6;
}
.panel-info {
  border-color: #bce8f1;
}
.panel-info > .panel-heading {
  color: #31708f;
  background-color: #d9edf7;
  border-color: #bce8f1;
}
.panel-info > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #bce8f1;
}
.panel-info > .panel-heading .badge {
  color: #d9edf7;
  background-color: #31708f;
}
.panel-info > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #bce8f1;
}
.panel-warning {
  border-color: #faebcc;
}
.panel-warning > .panel-heading {
  color: #8a6d3b;
  background-color: #fcf8e3;
  border-color: #faebcc;
}
.panel-warning > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #faebcc;
}
.panel-warning > .panel-heading .badge {
  color: #fcf8e3;
  background-color: #8a6d3b;
}
.panel-warning > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #faebcc;
}
.panel-danger {
  border-color: #ebccd1;
}
.panel-danger > .panel-heading {
  color: #a94442;
  background-color: #f2dede;
  border-color: #ebccd1;
}
.panel-danger > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ebccd1;
}
.panel-danger > .panel-heading .badge {
  color: #f2dede;
  background-color: #a94442;
}
.panel-danger > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ebccd1;
}
.embed-responsive {
  position: relative;
  display: block;
  height: 0;
  padding: 0;
  overflow: hidden;
}
.embed-responsive .embed-responsive-item,
.embed-responsive iframe,
.embed-responsive embed,
.embed-responsive object,
.embed-responsive video {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  height: 100%;
  width: 100%;
  border: 0;
}
.embed-responsive-16by9 {
  padding-bottom: 56.25%;
}
.embed-responsive-4by3 {
  padding-bottom: 75%;
}
.well {
  min-height: 20px;
  padding: 19px;
  margin-bottom: 20px;
  background-color: #f5f5f5;
  border: 1px solid #e3e3e3;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
}
.well blockquote {
  border-color: #ddd;
  border-color: rgba(0, 0, 0, 0.15);
}
.well-lg {
  padding: 24px;
  border-radius: 3px;
}
.well-sm {
  padding: 9px;
  border-radius: 1px;
}
.close {
  float: right;
  font-size: 19.5px;
  font-weight: bold;
  line-height: 1;
  color: #000;
  text-shadow: 0 1px 0 #fff;
  opacity: 0.2;
  filter: alpha(opacity=20);
}
.close:hover,
.close:focus {
  color: #000;
  text-decoration: none;
  cursor: pointer;
  opacity: 0.5;
  filter: alpha(opacity=50);
}
button.close {
  padding: 0;
  cursor: pointer;
  background: transparent;
  border: 0;
  -webkit-appearance: none;
}
.modal-open {
  overflow: hidden;
}
.modal {
  display: none;
  overflow: hidden;
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1050;
  -webkit-overflow-scrolling: touch;
  outline: 0;
}
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, -25%);
  -ms-transform: translate(0, -25%);
  -o-transform: translate(0, -25%);
  transform: translate(0, -25%);
  -webkit-transition: -webkit-transform 0.3s ease-out;
  -moz-transition: -moz-transform 0.3s ease-out;
  -o-transition: -o-transform 0.3s ease-out;
  transition: transform 0.3s ease-out;
}
.modal.in .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
.modal-open .modal {
  overflow-x: hidden;
  overflow-y: auto;
}
.modal-dialog {
  position: relative;
  width: auto;
  margin: 10px;
}
.modal-content {
  position: relative;
  background-color: #fff;
  border: 1px solid #999;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  background-clip: padding-box;
  outline: 0;
}
.modal-backdrop {
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1040;
  background-color: #000;
}
.modal-backdrop.fade {
  opacity: 0;
  filter: alpha(opacity=0);
}
.modal-backdrop.in {
  opacity: 0.5;
  filter: alpha(opacity=50);
}
.modal-header {
  padding: 15px;
  border-bottom: 1px solid #e5e5e5;
}
.modal-header .close {
  margin-top: -2px;
}
.modal-title {
  margin: 0;
  line-height: 1.42857143;
}
.modal-body {
  position: relative;
  padding: 15px;
}
.modal-footer {
  padding: 15px;
  text-align: right;
  border-top: 1px solid #e5e5e5;
}
.modal-footer .btn + .btn {
  margin-left: 5px;
  margin-bottom: 0;
}
.modal-footer .btn-group .btn + .btn {
  margin-left: -1px;
}
.modal-footer .btn-block + .btn-block {
  margin-left: 0;
}
.modal-scrollbar-measure {
  position: absolute;
  top: -9999px;
  width: 50px;
  height: 50px;
  overflow: scroll;
}
@media (min-width: 768px) {
  .modal-dialog {
    width: 600px;
    margin: 30px auto;
  }
  .modal-content {
    -webkit-box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
  }
  .modal-sm {
    width: 300px;
  }
}
@media (min-width: 992px) {
  .modal-lg {
    width: 900px;
  }
}
.tooltip {
  position: absolute;
  z-index: 1070;
  display: block;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 12px;
  opacity: 0;
  filter: alpha(opacity=0);
}
.tooltip.in {
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.tooltip.top {
  margin-top: -3px;
  padding: 5px 0;
}
.tooltip.right {
  margin-left: 3px;
  padding: 0 5px;
}
.tooltip.bottom {
  margin-top: 3px;
  padding: 5px 0;
}
.tooltip.left {
  margin-left: -3px;
  padding: 0 5px;
}
.tooltip-inner {
  max-width: 200px;
  padding: 3px 8px;
  color: #fff;
  text-align: center;
  background-color: #000;
  border-radius: 2px;
}
.tooltip-arrow {
  position: absolute;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.tooltip.top .tooltip-arrow {
  bottom: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-left .tooltip-arrow {
  bottom: 0;
  right: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-right .tooltip-arrow {
  bottom: 0;
  left: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.right .tooltip-arrow {
  top: 50%;
  left: 0;
  margin-top: -5px;
  border-width: 5px 5px 5px 0;
  border-right-color: #000;
}
.tooltip.left .tooltip-arrow {
  top: 50%;
  right: 0;
  margin-top: -5px;
  border-width: 5px 0 5px 5px;
  border-left-color: #000;
}
.tooltip.bottom .tooltip-arrow {
  top: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-left .tooltip-arrow {
  top: 0;
  right: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-right .tooltip-arrow {
  top: 0;
  left: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.popover {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 1060;
  display: none;
  max-width: 276px;
  padding: 1px;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 13px;
  background-color: #fff;
  background-clip: padding-box;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
}
.popover.top {
  margin-top: -10px;
}
.popover.right {
  margin-left: 10px;
}
.popover.bottom {
  margin-top: 10px;
}
.popover.left {
  margin-left: -10px;
}
.popover-title {
  margin: 0;
  padding: 8px 14px;
  font-size: 13px;
  background-color: #f7f7f7;
  border-bottom: 1px solid #ebebeb;
  border-radius: 2px 2px 0 0;
}
.popover-content {
  padding: 9px 14px;
}
.popover > .arrow,
.popover > .arrow:after {
  position: absolute;
  display: block;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.popover > .arrow {
  border-width: 11px;
}
.popover > .arrow:after {
  border-width: 10px;
  content: "";
}
.popover.top > .arrow {
  left: 50%;
  margin-left: -11px;
  border-bottom-width: 0;
  border-top-color: #999999;
  border-top-color: rgba(0, 0, 0, 0.25);
  bottom: -11px;
}
.popover.top > .arrow:after {
  content: " ";
  bottom: 1px;
  margin-left: -10px;
  border-bottom-width: 0;
  border-top-color: #fff;
}
.popover.right > .arrow {
  top: 50%;
  left: -11px;
  margin-top: -11px;
  border-left-width: 0;
  border-right-color: #999999;
  border-right-color: rgba(0, 0, 0, 0.25);
}
.popover.right > .arrow:after {
  content: " ";
  left: 1px;
  bottom: -10px;
  border-left-width: 0;
  border-right-color: #fff;
}
.popover.bottom > .arrow {
  left: 50%;
  margin-left: -11px;
  border-top-width: 0;
  border-bottom-color: #999999;
  border-bottom-color: rgba(0, 0, 0, 0.25);
  top: -11px;
}
.popover.bottom > .arrow:after {
  content: " ";
  top: 1px;
  margin-left: -10px;
  border-top-width: 0;
  border-bottom-color: #fff;
}
.popover.left > .arrow {
  top: 50%;
  right: -11px;
  margin-top: -11px;
  border-right-width: 0;
  border-left-color: #999999;
  border-left-color: rgba(0, 0, 0, 0.25);
}
.popover.left > .arrow:after {
  content: " ";
  right: 1px;
  border-right-width: 0;
  border-left-color: #fff;
  bottom: -10px;
}
.carousel {
  position: relative;
}
.carousel-inner {
  position: relative;
  overflow: hidden;
  width: 100%;
}
.carousel-inner > .item {
  display: none;
  position: relative;
  -webkit-transition: 0.6s ease-in-out left;
  -o-transition: 0.6s ease-in-out left;
  transition: 0.6s ease-in-out left;
}
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  line-height: 1;
}
@media all and (transform-3d), (-webkit-transform-3d) {
  .carousel-inner > .item {
    -webkit-transition: -webkit-transform 0.6s ease-in-out;
    -moz-transition: -moz-transform 0.6s ease-in-out;
    -o-transition: -o-transform 0.6s ease-in-out;
    transition: transform 0.6s ease-in-out;
    -webkit-backface-visibility: hidden;
    -moz-backface-visibility: hidden;
    backface-visibility: hidden;
    -webkit-perspective: 1000px;
    -moz-perspective: 1000px;
    perspective: 1000px;
  }
  .carousel-inner > .item.next,
  .carousel-inner > .item.active.right {
    -webkit-transform: translate3d(100%, 0, 0);
    transform: translate3d(100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.prev,
  .carousel-inner > .item.active.left {
    -webkit-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.next.left,
  .carousel-inner > .item.prev.right,
  .carousel-inner > .item.active {
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
    left: 0;
  }
}
.carousel-inner > .active,
.carousel-inner > .next,
.carousel-inner > .prev {
  display: block;
}
.carousel-inner > .active {
  left: 0;
}
.carousel-inner > .next,
.carousel-inner > .prev {
  position: absolute;
  top: 0;
  width: 100%;
}
.carousel-inner > .next {
  left: 100%;
}
.carousel-inner > .prev {
  left: -100%;
}
.carousel-inner > .next.left,
.carousel-inner > .prev.right {
  left: 0;
}
.carousel-inner > .active.left {
  left: -100%;
}
.carousel-inner > .active.right {
  left: 100%;
}
.carousel-control {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  width: 15%;
  opacity: 0.5;
  filter: alpha(opacity=50);
  font-size: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
  background-color: rgba(0, 0, 0, 0);
}
.carousel-control.left {
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);
}
.carousel-control.right {
  left: auto;
  right: 0;
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);
}
.carousel-control:hover,
.carousel-control:focus {
  outline: 0;
  color: #fff;
  text-decoration: none;
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.carousel-control .icon-prev,
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-left,
.carousel-control .glyphicon-chevron-right {
  position: absolute;
  top: 50%;
  margin-top: -10px;
  z-index: 5;
  display: inline-block;
}
.carousel-control .icon-prev,
.carousel-control .glyphicon-chevron-left {
  left: 50%;
  margin-left: -10px;
}
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-right {
  right: 50%;
  margin-right: -10px;
}
.carousel-control .icon-prev,
.carousel-control .icon-next {
  width: 20px;
  height: 20px;
  line-height: 1;
  font-family: serif;
}
.carousel-control .icon-prev:before {
  content: '\2039';
}
.carousel-control .icon-next:before {
  content: '\203a';
}
.carousel-indicators {
  position: absolute;
  bottom: 10px;
  left: 50%;
  z-index: 15;
  width: 60%;
  margin-left: -30%;
  padding-left: 0;
  list-style: none;
  text-align: center;
}
.carousel-indicators li {
  display: inline-block;
  width: 10px;
  height: 10px;
  margin: 1px;
  text-indent: -999px;
  border: 1px solid #fff;
  border-radius: 10px;
  cursor: pointer;
  background-color: #000 \9;
  background-color: rgba(0, 0, 0, 0);
}
.carousel-indicators .active {
  margin: 0;
  width: 12px;
  height: 12px;
  background-color: #fff;
}
.carousel-caption {
  position: absolute;
  left: 15%;
  right: 15%;
  bottom: 20px;
  z-index: 10;
  padding-top: 20px;
  padding-bottom: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
}
.carousel-caption .btn {
  text-shadow: none;
}
@media screen and (min-width: 768px) {
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-prev,
  .carousel-control .icon-next {
    width: 30px;
    height: 30px;
    margin-top: -10px;
    font-size: 30px;
  }
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .icon-prev {
    margin-left: -10px;
  }
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-next {
    margin-right: -10px;
  }
  .carousel-caption {
    left: 20%;
    right: 20%;
    padding-bottom: 30px;
  }
  .carousel-indicators {
    bottom: 20px;
  }
}
.clearfix:before,
.clearfix:after,
.dl-horizontal dd:before,
.dl-horizontal dd:after,
.container:before,
.container:after,
.container-fluid:before,
.container-fluid:after,
.row:before,
.row:after,
.form-horizontal .form-group:before,
.form-horizontal .form-group:after,
.btn-toolbar:before,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:before,
.btn-group-vertical > .btn-group:after,
.nav:before,
.nav:after,
.navbar:before,
.navbar:after,
.navbar-header:before,
.navbar-header:after,
.navbar-collapse:before,
.navbar-collapse:after,
.pager:before,
.pager:after,
.panel-body:before,
.panel-body:after,
.modal-header:before,
.modal-header:after,
.modal-footer:before,
.modal-footer:after,
.item_buttons:before,
.item_buttons:after {
  content: " ";
  display: table;
}
.clearfix:after,
.dl-horizontal dd:after,
.container:after,
.container-fluid:after,
.row:after,
.form-horizontal .form-group:after,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:after,
.nav:after,
.navbar:after,
.navbar-header:after,
.navbar-collapse:after,
.pager:after,
.panel-body:after,
.modal-header:after,
.modal-footer:after,
.item_buttons:after {
  clear: both;
}
.center-block {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.pull-right {
  float: right !important;
}
.pull-left {
  float: left !important;
}
.hide {
  display: none !important;
}
.show {
  display: block !important;
}
.invisible {
  visibility: hidden;
}
.text-hide {
  font: 0/0 a;
  color: transparent;
  text-shadow: none;
  background-color: transparent;
  border: 0;
}
.hidden {
  display: none !important;
}
.affix {
  position: fixed;
}
@-ms-viewport {
  width: device-width;
}
.visible-xs,
.visible-sm,
.visible-md,
.visible-lg {
  display: none !important;
}
.visible-xs-block,
.visible-xs-inline,
.visible-xs-inline-block,
.visible-sm-block,
.visible-sm-inline,
.visible-sm-inline-block,
.visible-md-block,
.visible-md-inline,
.visible-md-inline-block,
.visible-lg-block,
.visible-lg-inline,
.visible-lg-inline-block {
  display: none !important;
}
@media (max-width: 767px) {
  .visible-xs {
    display: block !important;
  }
  table.visible-xs {
    display: table !important;
  }
  tr.visible-xs {
    display: table-row !important;
  }
  th.visible-xs,
  td.visible-xs {
    display: table-cell !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-block {
    display: block !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline {
    display: inline !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm {
    display: block !important;
  }
  table.visible-sm {
    display: table !important;
  }
  tr.visible-sm {
    display: table-row !important;
  }
  th.visible-sm,
  td.visible-sm {
    display: table-cell !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-block {
    display: block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline {
    display: inline !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md {
    display: block !important;
  }
  table.visible-md {
    display: table !important;
  }
  tr.visible-md {
    display: table-row !important;
  }
  th.visible-md,
  td.visible-md {
    display: table-cell !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-block {
    display: block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline {
    display: inline !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg {
    display: block !important;
  }
  table.visible-lg {
    display: table !important;
  }
  tr.visible-lg {
    display: table-row !important;
  }
  th.visible-lg,
  td.visible-lg {
    display: table-cell !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-block {
    display: block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline {
    display: inline !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline-block {
    display: inline-block !important;
  }
}
@media (max-width: 767px) {
  .hidden-xs {
    display: none !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .hidden-sm {
    display: none !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .hidden-md {
    display: none !important;
  }
}
@media (min-width: 1200px) {
  .hidden-lg {
    display: none !important;
  }
}
.visible-print {
  display: none !important;
}
@media print {
  .visible-print {
    display: block !important;
  }
  table.visible-print {
    display: table !important;
  }
  tr.visible-print {
    display: table-row !important;
  }
  th.visible-print,
  td.visible-print {
    display: table-cell !important;
  }
}
.visible-print-block {
  display: none !important;
}
@media print {
  .visible-print-block {
    display: block !important;
  }
}
.visible-print-inline {
  display: none !important;
}
@media print {
  .visible-print-inline {
    display: inline !important;
  }
}
.visible-print-inline-block {
  display: none !important;
}
@media print {
  .visible-print-inline-block {
    display: inline-block !important;
  }
}
@media print {
  .hidden-print {
    display: none !important;
  }
}
/*!
*
* Font Awesome
*
*/
/*!
 *  Font Awesome 4.2.0 by @davegandy - http://fontawesome.io - @fontawesome
 *  License - http://fontawesome.io/license (Font: SIL OFL 1.1, CSS: MIT License)
 */
/* FONT PATH
 * -------------------------- */
@font-face {
  font-family: 'FontAwesome';
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?v=4.2.0');
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?#iefix&v=4.2.0') format('embedded-opentype'), url('../components/font-awesome/fonts/fontawesome-webfont.woff?v=4.2.0') format('woff'), url('../components/font-awesome/fonts/fontawesome-webfont.ttf?v=4.2.0') format('truetype'), url('../components/font-awesome/fonts/fontawesome-webfont.svg?v=4.2.0#fontawesomeregular') format('svg');
  font-weight: normal;
  font-style: normal;
}
.fa {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
/* makes the font 33% larger relative to the icon container */
.fa-lg {
  font-size: 1.33333333em;
  line-height: 0.75em;
  vertical-align: -15%;
}
.fa-2x {
  font-size: 2em;
}
.fa-3x {
  font-size: 3em;
}
.fa-4x {
  font-size: 4em;
}
.fa-5x {
  font-size: 5em;
}
.fa-fw {
  width: 1.28571429em;
  text-align: center;
}
.fa-ul {
  padding-left: 0;
  margin-left: 2.14285714em;
  list-style-type: none;
}
.fa-ul > li {
  position: relative;
}
.fa-li {
  position: absolute;
  left: -2.14285714em;
  width: 2.14285714em;
  top: 0.14285714em;
  text-align: center;
}
.fa-li.fa-lg {
  left: -1.85714286em;
}
.fa-border {
  padding: .2em .25em .15em;
  border: solid 0.08em #eee;
  border-radius: .1em;
}
.pull-right {
  float: right;
}
.pull-left {
  float: left;
}
.fa.pull-left {
  margin-right: .3em;
}
.fa.pull-right {
  margin-left: .3em;
}
.fa-spin {
  -webkit-animation: fa-spin 2s infinite linear;
  animation: fa-spin 2s infinite linear;
}
@-webkit-keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
@keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
.fa-rotate-90 {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=1);
  -webkit-transform: rotate(90deg);
  -ms-transform: rotate(90deg);
  transform: rotate(90deg);
}
.fa-rotate-180 {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=2);
  -webkit-transform: rotate(180deg);
  -ms-transform: rotate(180deg);
  transform: rotate(180deg);
}
.fa-rotate-270 {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=3);
  -webkit-transform: rotate(270deg);
  -ms-transform: rotate(270deg);
  transform: rotate(270deg);
}
.fa-flip-horizontal {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=0, mirror=1);
  -webkit-transform: scale(-1, 1);
  -ms-transform: scale(-1, 1);
  transform: scale(-1, 1);
}
.fa-flip-vertical {
  filter: progid:DXImageTransform.Microsoft.BasicImage(rotation=2, mirror=1);
  -webkit-transform: scale(1, -1);
  -ms-transform: scale(1, -1);
  transform: scale(1, -1);
}
:root .fa-rotate-90,
:root .fa-rotate-180,
:root .fa-rotate-270,
:root .fa-flip-horizontal,
:root .fa-flip-vertical {
  filter: none;
}
.fa-stack {
  position: relative;
  display: inline-block;
  width: 2em;
  height: 2em;
  line-height: 2em;
  vertical-align: middle;
}
.fa-stack-1x,
.fa-stack-2x {
  position: absolute;
  left: 0;
  width: 100%;
  text-align: center;
}
.fa-stack-1x {
  line-height: inherit;
}
.fa-stack-2x {
  font-size: 2em;
}
.fa-inverse {
  color: #fff;
}
/* Font Awesome uses the Unicode Private Use Area (PUA) to ensure screen
   readers do not read off random characters that represent icons */
.fa-glass:before {
  content: "\f000";
}
.fa-music:before {
  content: "\f001";
}
.fa-search:before {
  content: "\f002";
}
.fa-envelope-o:before {
  content: "\f003";
}
.fa-heart:before {
  content: "\f004";
}
.fa-star:before {
  content: "\f005";
}
.fa-star-o:before {
  content: "\f006";
}
.fa-user:before {
  content: "\f007";
}
.fa-film:before {
  content: "\f008";
}
.fa-th-large:before {
  content: "\f009";
}
.fa-th:before {
  content: "\f00a";
}
.fa-th-list:before {
  content: "\f00b";
}
.fa-check:before {
  content: "\f00c";
}
.fa-remove:before,
.fa-close:before,
.fa-times:before {
  content: "\f00d";
}
.fa-search-plus:before {
  content: "\f00e";
}
.fa-search-minus:before {
  content: "\f010";
}
.fa-power-off:before {
  content: "\f011";
}
.fa-signal:before {
  content: "\f012";
}
.fa-gear:before,
.fa-cog:before {
  content: "\f013";
}
.fa-trash-o:before {
  content: "\f014";
}
.fa-home:before {
  content: "\f015";
}
.fa-file-o:before {
  content: "\f016";
}
.fa-clock-o:before {
  content: "\f017";
}
.fa-road:before {
  content: "\f018";
}
.fa-download:before {
  content: "\f019";
}
.fa-arrow-circle-o-down:before {
  content: "\f01a";
}
.fa-arrow-circle-o-up:before {
  content: "\f01b";
}
.fa-inbox:before {
  content: "\f01c";
}
.fa-play-circle-o:before {
  content: "\f01d";
}
.fa-rotate-right:before,
.fa-repeat:before {
  content: "\f01e";
}
.fa-refresh:before {
  content: "\f021";
}
.fa-list-alt:before {
  content: "\f022";
}
.fa-lock:before {
  content: "\f023";
}
.fa-flag:before {
  content: "\f024";
}
.fa-headphones:before {
  content: "\f025";
}
.fa-volume-off:before {
  content: "\f026";
}
.fa-volume-down:before {
  content: "\f027";
}
.fa-volume-up:before {
  content: "\f028";
}
.fa-qrcode:before {
  content: "\f029";
}
.fa-barcode:before {
  content: "\f02a";
}
.fa-tag:before {
  content: "\f02b";
}
.fa-tags:before {
  content: "\f02c";
}
.fa-book:before {
  content: "\f02d";
}
.fa-bookmark:before {
  content: "\f02e";
}
.fa-print:before {
  content: "\f02f";
}
.fa-camera:before {
  content: "\f030";
}
.fa-font:before {
  content: "\f031";
}
.fa-bold:before {
  content: "\f032";
}
.fa-italic:before {
  content: "\f033";
}
.fa-text-height:before {
  content: "\f034";
}
.fa-text-width:before {
  content: "\f035";
}
.fa-align-left:before {
  content: "\f036";
}
.fa-align-center:before {
  content: "\f037";
}
.fa-align-right:before {
  content: "\f038";
}
.fa-align-justify:before {
  content: "\f039";
}
.fa-list:before {
  content: "\f03a";
}
.fa-dedent:before,
.fa-outdent:before {
  content: "\f03b";
}
.fa-indent:before {
  content: "\f03c";
}
.fa-video-camera:before {
  content: "\f03d";
}
.fa-photo:before,
.fa-image:before,
.fa-picture-o:before {
  content: "\f03e";
}
.fa-pencil:before {
  content: "\f040";
}
.fa-map-marker:before {
  content: "\f041";
}
.fa-adjust:before {
  content: "\f042";
}
.fa-tint:before {
  content: "\f043";
}
.fa-edit:before,
.fa-pencil-square-o:before {
  content: "\f044";
}
.fa-share-square-o:before {
  content: "\f045";
}
.fa-check-square-o:before {
  content: "\f046";
}
.fa-arrows:before {
  content: "\f047";
}
.fa-step-backward:before {
  content: "\f048";
}
.fa-fast-backward:before {
  content: "\f049";
}
.fa-backward:before {
  content: "\f04a";
}
.fa-play:before {
  content: "\f04b";
}
.fa-pause:before {
  content: "\f04c";
}
.fa-stop:before {
  content: "\f04d";
}
.fa-forward:before {
  content: "\f04e";
}
.fa-fast-forward:before {
  content: "\f050";
}
.fa-step-forward:before {
  content: "\f051";
}
.fa-eject:before {
  content: "\f052";
}
.fa-chevron-left:before {
  content: "\f053";
}
.fa-chevron-right:before {
  content: "\f054";
}
.fa-plus-circle:before {
  content: "\f055";
}
.fa-minus-circle:before {
  content: "\f056";
}
.fa-times-circle:before {
  content: "\f057";
}
.fa-check-circle:before {
  content: "\f058";
}
.fa-question-circle:before {
  content: "\f059";
}
.fa-info-circle:before {
  content: "\f05a";
}
.fa-crosshairs:before {
  content: "\f05b";
}
.fa-times-circle-o:before {
  content: "\f05c";
}
.fa-check-circle-o:before {
  content: "\f05d";
}
.fa-ban:before {
  content: "\f05e";
}
.fa-arrow-left:before {
  content: "\f060";
}
.fa-arrow-right:before {
  content: "\f061";
}
.fa-arrow-up:before {
  content: "\f062";
}
.fa-arrow-down:before {
  content: "\f063";
}
.fa-mail-forward:before,
.fa-share:before {
  content: "\f064";
}
.fa-expand:before {
  content: "\f065";
}
.fa-compress:before {
  content: "\f066";
}
.fa-plus:before {
  content: "\f067";
}
.fa-minus:before {
  content: "\f068";
}
.fa-asterisk:before {
  content: "\f069";
}
.fa-exclamation-circle:before {
  content: "\f06a";
}
.fa-gift:before {
  content: "\f06b";
}
.fa-leaf:before {
  content: "\f06c";
}
.fa-fire:before {
  content: "\f06d";
}
.fa-eye:before {
  content: "\f06e";
}
.fa-eye-slash:before {
  content: "\f070";
}
.fa-warning:before,
.fa-exclamation-triangle:before {
  content: "\f071";
}
.fa-plane:before {
  content: "\f072";
}
.fa-calendar:before {
  content: "\f073";
}
.fa-random:before {
  content: "\f074";
}
.fa-comment:before {
  content: "\f075";
}
.fa-magnet:before {
  content: "\f076";
}
.fa-chevron-up:before {
  content: "\f077";
}
.fa-chevron-down:before {
  content: "\f078";
}
.fa-retweet:before {
  content: "\f079";
}
.fa-shopping-cart:before {
  content: "\f07a";
}
.fa-folder:before {
  content: "\f07b";
}
.fa-folder-open:before {
  content: "\f07c";
}
.fa-arrows-v:before {
  content: "\f07d";
}
.fa-arrows-h:before {
  content: "\f07e";
}
.fa-bar-chart-o:before,
.fa-bar-chart:before {
  content: "\f080";
}
.fa-twitter-square:before {
  content: "\f081";
}
.fa-facebook-square:before {
  content: "\f082";
}
.fa-camera-retro:before {
  content: "\f083";
}
.fa-key:before {
  content: "\f084";
}
.fa-gears:before,
.fa-cogs:before {
  content: "\f085";
}
.fa-comments:before {
  content: "\f086";
}
.fa-thumbs-o-up:before {
  content: "\f087";
}
.fa-thumbs-o-down:before {
  content: "\f088";
}
.fa-star-half:before {
  content: "\f089";
}
.fa-heart-o:before {
  content: "\f08a";
}
.fa-sign-out:before {
  content: "\f08b";
}
.fa-linkedin-square:before {
  content: "\f08c";
}
.fa-thumb-tack:before {
  content: "\f08d";
}
.fa-external-link:before {
  content: "\f08e";
}
.fa-sign-in:before {
  content: "\f090";
}
.fa-trophy:before {
  content: "\f091";
}
.fa-github-square:before {
  content: "\f092";
}
.fa-upload:before {
  content: "\f093";
}
.fa-lemon-o:before {
  content: "\f094";
}
.fa-phone:before {
  content: "\f095";
}
.fa-square-o:before {
  content: "\f096";
}
.fa-bookmark-o:before {
  content: "\f097";
}
.fa-phone-square:before {
  content: "\f098";
}
.fa-twitter:before {
  content: "\f099";
}
.fa-facebook:before {
  content: "\f09a";
}
.fa-github:before {
  content: "\f09b";
}
.fa-unlock:before {
  content: "\f09c";
}
.fa-credit-card:before {
  content: "\f09d";
}
.fa-rss:before {
  content: "\f09e";
}
.fa-hdd-o:before {
  content: "\f0a0";
}
.fa-bullhorn:before {
  content: "\f0a1";
}
.fa-bell:before {
  content: "\f0f3";
}
.fa-certificate:before {
  content: "\f0a3";
}
.fa-hand-o-right:before {
  content: "\f0a4";
}
.fa-hand-o-left:before {
  content: "\f0a5";
}
.fa-hand-o-up:before {
  content: "\f0a6";
}
.fa-hand-o-down:before {
  content: "\f0a7";
}
.fa-arrow-circle-left:before {
  content: "\f0a8";
}
.fa-arrow-circle-right:before {
  content: "\f0a9";
}
.fa-arrow-circle-up:before {
  content: "\f0aa";
}
.fa-arrow-circle-down:before {
  content: "\f0ab";
}
.fa-globe:before {
  content: "\f0ac";
}
.fa-wrench:before {
  content: "\f0ad";
}
.fa-tasks:before {
  content: "\f0ae";
}
.fa-filter:before {
  content: "\f0b0";
}
.fa-briefcase:before {
  content: "\f0b1";
}
.fa-arrows-alt:before {
  content: "\f0b2";
}
.fa-group:before,
.fa-users:before {
  content: "\f0c0";
}
.fa-chain:before,
.fa-link:before {
  content: "\f0c1";
}
.fa-cloud:before {
  content: "\f0c2";
}
.fa-flask:before {
  content: "\f0c3";
}
.fa-cut:before,
.fa-scissors:before {
  content: "\f0c4";
}
.fa-copy:before,
.fa-files-o:before {
  content: "\f0c5";
}
.fa-paperclip:before {
  content: "\f0c6";
}
.fa-save:before,
.fa-floppy-o:before {
  content: "\f0c7";
}
.fa-square:before {
  content: "\f0c8";
}
.fa-navicon:before,
.fa-reorder:before,
.fa-bars:before {
  content: "\f0c9";
}
.fa-list-ul:before {
  content: "\f0ca";
}
.fa-list-ol:before {
  content: "\f0cb";
}
.fa-strikethrough:before {
  content: "\f0cc";
}
.fa-underline:before {
  content: "\f0cd";
}
.fa-table:before {
  content: "\f0ce";
}
.fa-magic:before {
  content: "\f0d0";
}
.fa-truck:before {
  content: "\f0d1";
}
.fa-pinterest:before {
  content: "\f0d2";
}
.fa-pinterest-square:before {
  content: "\f0d3";
}
.fa-google-plus-square:before {
  content: "\f0d4";
}
.fa-google-plus:before {
  content: "\f0d5";
}
.fa-money:before {
  content: "\f0d6";
}
.fa-caret-down:before {
  content: "\f0d7";
}
.fa-caret-up:before {
  content: "\f0d8";
}
.fa-caret-left:before {
  content: "\f0d9";
}
.fa-caret-right:before {
  content: "\f0da";
}
.fa-columns:before {
  content: "\f0db";
}
.fa-unsorted:before,
.fa-sort:before {
  content: "\f0dc";
}
.fa-sort-down:before,
.fa-sort-desc:before {
  content: "\f0dd";
}
.fa-sort-up:before,
.fa-sort-asc:before {
  content: "\f0de";
}
.fa-envelope:before {
  content: "\f0e0";
}
.fa-linkedin:before {
  content: "\f0e1";
}
.fa-rotate-left:before,
.fa-undo:before {
  content: "\f0e2";
}
.fa-legal:before,
.fa-gavel:before {
  content: "\f0e3";
}
.fa-dashboard:before,
.fa-tachometer:before {
  content: "\f0e4";
}
.fa-comment-o:before {
  content: "\f0e5";
}
.fa-comments-o:before {
  content: "\f0e6";
}
.fa-flash:before,
.fa-bolt:before {
  content: "\f0e7";
}
.fa-sitemap:before {
  content: "\f0e8";
}
.fa-umbrella:before {
  content: "\f0e9";
}
.fa-paste:before,
.fa-clipboard:before {
  content: "\f0ea";
}
.fa-lightbulb-o:before {
  content: "\f0eb";
}
.fa-exchange:before {
  content: "\f0ec";
}
.fa-cloud-download:before {
  content: "\f0ed";
}
.fa-cloud-upload:before {
  content: "\f0ee";
}
.fa-user-md:before {
  content: "\f0f0";
}
.fa-stethoscope:before {
  content: "\f0f1";
}
.fa-suitcase:before {
  content: "\f0f2";
}
.fa-bell-o:before {
  content: "\f0a2";
}
.fa-coffee:before {
  content: "\f0f4";
}
.fa-cutlery:before {
  content: "\f0f5";
}
.fa-file-text-o:before {
  content: "\f0f6";
}
.fa-building-o:before {
  content: "\f0f7";
}
.fa-hospital-o:before {
  content: "\f0f8";
}
.fa-ambulance:before {
  content: "\f0f9";
}
.fa-medkit:before {
  content: "\f0fa";
}
.fa-fighter-jet:before {
  content: "\f0fb";
}
.fa-beer:before {
  content: "\f0fc";
}
.fa-h-square:before {
  content: "\f0fd";
}
.fa-plus-square:before {
  content: "\f0fe";
}
.fa-angle-double-left:before {
  content: "\f100";
}
.fa-angle-double-right:before {
  content: "\f101";
}
.fa-angle-double-up:before {
  content: "\f102";
}
.fa-angle-double-down:before {
  content: "\f103";
}
.fa-angle-left:before {
  content: "\f104";
}
.fa-angle-right:before {
  content: "\f105";
}
.fa-angle-up:before {
  content: "\f106";
}
.fa-angle-down:before {
  content: "\f107";
}
.fa-desktop:before {
  content: "\f108";
}
.fa-laptop:before {
  content: "\f109";
}
.fa-tablet:before {
  content: "\f10a";
}
.fa-mobile-phone:before,
.fa-mobile:before {
  content: "\f10b";
}
.fa-circle-o:before {
  content: "\f10c";
}
.fa-quote-left:before {
  content: "\f10d";
}
.fa-quote-right:before {
  content: "\f10e";
}
.fa-spinner:before {
  content: "\f110";
}
.fa-circle:before {
  content: "\f111";
}
.fa-mail-reply:before,
.fa-reply:before {
  content: "\f112";
}
.fa-github-alt:before {
  content: "\f113";
}
.fa-folder-o:before {
  content: "\f114";
}
.fa-folder-open-o:before {
  content: "\f115";
}
.fa-smile-o:before {
  content: "\f118";
}
.fa-frown-o:before {
  content: "\f119";
}
.fa-meh-o:before {
  content: "\f11a";
}
.fa-gamepad:before {
  content: "\f11b";
}
.fa-keyboard-o:before {
  content: "\f11c";
}
.fa-flag-o:before {
  content: "\f11d";
}
.fa-flag-checkered:before {
  content: "\f11e";
}
.fa-terminal:before {
  content: "\f120";
}
.fa-code:before {
  content: "\f121";
}
.fa-mail-reply-all:before,
.fa-reply-all:before {
  content: "\f122";
}
.fa-star-half-empty:before,
.fa-star-half-full:before,
.fa-star-half-o:before {
  content: "\f123";
}
.fa-location-arrow:before {
  content: "\f124";
}
.fa-crop:before {
  content: "\f125";
}
.fa-code-fork:before {
  content: "\f126";
}
.fa-unlink:before,
.fa-chain-broken:before {
  content: "\f127";
}
.fa-question:before {
  content: "\f128";
}
.fa-info:before {
  content: "\f129";
}
.fa-exclamation:before {
  content: "\f12a";
}
.fa-superscript:before {
  content: "\f12b";
}
.fa-subscript:before {
  content: "\f12c";
}
.fa-eraser:before {
  content: "\f12d";
}
.fa-puzzle-piece:before {
  content: "\f12e";
}
.fa-microphone:before {
  content: "\f130";
}
.fa-microphone-slash:before {
  content: "\f131";
}
.fa-shield:before {
  content: "\f132";
}
.fa-calendar-o:before {
  content: "\f133";
}
.fa-fire-extinguisher:before {
  content: "\f134";
}
.fa-rocket:before {
  content: "\f135";
}
.fa-maxcdn:before {
  content: "\f136";
}
.fa-chevron-circle-left:before {
  content: "\f137";
}
.fa-chevron-circle-right:before {
  content: "\f138";
}
.fa-chevron-circle-up:before {
  content: "\f139";
}
.fa-chevron-circle-down:before {
  content: "\f13a";
}
.fa-html5:before {
  content: "\f13b";
}
.fa-css3:before {
  content: "\f13c";
}
.fa-anchor:before {
  content: "\f13d";
}
.fa-unlock-alt:before {
  content: "\f13e";
}
.fa-bullseye:before {
  content: "\f140";
}
.fa-ellipsis-h:before {
  content: "\f141";
}
.fa-ellipsis-v:before {
  content: "\f142";
}
.fa-rss-square:before {
  content: "\f143";
}
.fa-play-circle:before {
  content: "\f144";
}
.fa-ticket:before {
  content: "\f145";
}
.fa-minus-square:before {
  content: "\f146";
}
.fa-minus-square-o:before {
  content: "\f147";
}
.fa-level-up:before {
  content: "\f148";
}
.fa-level-down:before {
  content: "\f149";
}
.fa-check-square:before {
  content: "\f14a";
}
.fa-pencil-square:before {
  content: "\f14b";
}
.fa-external-link-square:before {
  content: "\f14c";
}
.fa-share-square:before {
  content: "\f14d";
}
.fa-compass:before {
  content: "\f14e";
}
.fa-toggle-down:before,
.fa-caret-square-o-down:before {
  content: "\f150";
}
.fa-toggle-up:before,
.fa-caret-square-o-up:before {
  content: "\f151";
}
.fa-toggle-right:before,
.fa-caret-square-o-right:before {
  content: "\f152";
}
.fa-euro:before,
.fa-eur:before {
  content: "\f153";
}
.fa-gbp:before {
  content: "\f154";
}
.fa-dollar:before,
.fa-usd:before {
  content: "\f155";
}
.fa-rupee:before,
.fa-inr:before {
  content: "\f156";
}
.fa-cny:before,
.fa-rmb:before,
.fa-yen:before,
.fa-jpy:before {
  content: "\f157";
}
.fa-ruble:before,
.fa-rouble:before,
.fa-rub:before {
  content: "\f158";
}
.fa-won:before,
.fa-krw:before {
  content: "\f159";
}
.fa-bitcoin:before,
.fa-btc:before {
  content: "\f15a";
}
.fa-file:before {
  content: "\f15b";
}
.fa-file-text:before {
  content: "\f15c";
}
.fa-sort-alpha-asc:before {
  content: "\f15d";
}
.fa-sort-alpha-desc:before {
  content: "\f15e";
}
.fa-sort-amount-asc:before {
  content: "\f160";
}
.fa-sort-amount-desc:before {
  content: "\f161";
}
.fa-sort-numeric-asc:before {
  content: "\f162";
}
.fa-sort-numeric-desc:before {
  content: "\f163";
}
.fa-thumbs-up:before {
  content: "\f164";
}
.fa-thumbs-down:before {
  content: "\f165";
}
.fa-youtube-square:before {
  content: "\f166";
}
.fa-youtube:before {
  content: "\f167";
}
.fa-xing:before {
  content: "\f168";
}
.fa-xing-square:before {
  content: "\f169";
}
.fa-youtube-play:before {
  content: "\f16a";
}
.fa-dropbox:before {
  content: "\f16b";
}
.fa-stack-overflow:before {
  content: "\f16c";
}
.fa-instagram:before {
  content: "\f16d";
}
.fa-flickr:before {
  content: "\f16e";
}
.fa-adn:before {
  content: "\f170";
}
.fa-bitbucket:before {
  content: "\f171";
}
.fa-bitbucket-square:before {
  content: "\f172";
}
.fa-tumblr:before {
  content: "\f173";
}
.fa-tumblr-square:before {
  content: "\f174";
}
.fa-long-arrow-down:before {
  content: "\f175";
}
.fa-long-arrow-up:before {
  content: "\f176";
}
.fa-long-arrow-left:before {
  content: "\f177";
}
.fa-long-arrow-right:before {
  content: "\f178";
}
.fa-apple:before {
  content: "\f179";
}
.fa-windows:before {
  content: "\f17a";
}
.fa-android:before {
  content: "\f17b";
}
.fa-linux:before {
  content: "\f17c";
}
.fa-dribbble:before {
  content: "\f17d";
}
.fa-skype:before {
  content: "\f17e";
}
.fa-foursquare:before {
  content: "\f180";
}
.fa-trello:before {
  content: "\f181";
}
.fa-female:before {
  content: "\f182";
}
.fa-male:before {
  content: "\f183";
}
.fa-gittip:before {
  content: "\f184";
}
.fa-sun-o:before {
  content: "\f185";
}
.fa-moon-o:before {
  content: "\f186";
}
.fa-archive:before {
  content: "\f187";
}
.fa-bug:before {
  content: "\f188";
}
.fa-vk:before {
  content: "\f189";
}
.fa-weibo:before {
  content: "\f18a";
}
.fa-renren:before {
  content: "\f18b";
}
.fa-pagelines:before {
  content: "\f18c";
}
.fa-stack-exchange:before {
  content: "\f18d";
}
.fa-arrow-circle-o-right:before {
  content: "\f18e";
}
.fa-arrow-circle-o-left:before {
  content: "\f190";
}
.fa-toggle-left:before,
.fa-caret-square-o-left:before {
  content: "\f191";
}
.fa-dot-circle-o:before {
  content: "\f192";
}
.fa-wheelchair:before {
  content: "\f193";
}
.fa-vimeo-square:before {
  content: "\f194";
}
.fa-turkish-lira:before,
.fa-try:before {
  content: "\f195";
}
.fa-plus-square-o:before {
  content: "\f196";
}
.fa-space-shuttle:before {
  content: "\f197";
}
.fa-slack:before {
  content: "\f198";
}
.fa-envelope-square:before {
  content: "\f199";
}
.fa-wordpress:before {
  content: "\f19a";
}
.fa-openid:before {
  content: "\f19b";
}
.fa-institution:before,
.fa-bank:before,
.fa-university:before {
  content: "\f19c";
}
.fa-mortar-board:before,
.fa-graduation-cap:before {
  content: "\f19d";
}
.fa-yahoo:before {
  content: "\f19e";
}
.fa-google:before {
  content: "\f1a0";
}
.fa-reddit:before {
  content: "\f1a1";
}
.fa-reddit-square:before {
  content: "\f1a2";
}
.fa-stumbleupon-circle:before {
  content: "\f1a3";
}
.fa-stumbleupon:before {
  content: "\f1a4";
}
.fa-delicious:before {
  content: "\f1a5";
}
.fa-digg:before {
  content: "\f1a6";
}
.fa-pied-piper:before {
  content: "\f1a7";
}
.fa-pied-piper-alt:before {
  content: "\f1a8";
}
.fa-drupal:before {
  content: "\f1a9";
}
.fa-joomla:before {
  content: "\f1aa";
}
.fa-language:before {
  content: "\f1ab";
}
.fa-fax:before {
  content: "\f1ac";
}
.fa-building:before {
  content: "\f1ad";
}
.fa-child:before {
  content: "\f1ae";
}
.fa-paw:before {
  content: "\f1b0";
}
.fa-spoon:before {
  content: "\f1b1";
}
.fa-cube:before {
  content: "\f1b2";
}
.fa-cubes:before {
  content: "\f1b3";
}
.fa-behance:before {
  content: "\f1b4";
}
.fa-behance-square:before {
  content: "\f1b5";
}
.fa-steam:before {
  content: "\f1b6";
}
.fa-steam-square:before {
  content: "\f1b7";
}
.fa-recycle:before {
  content: "\f1b8";
}
.fa-automobile:before,
.fa-car:before {
  content: "\f1b9";
}
.fa-cab:before,
.fa-taxi:before {
  content: "\f1ba";
}
.fa-tree:before {
  content: "\f1bb";
}
.fa-spotify:before {
  content: "\f1bc";
}
.fa-deviantart:before {
  content: "\f1bd";
}
.fa-soundcloud:before {
  content: "\f1be";
}
.fa-database:before {
  content: "\f1c0";
}
.fa-file-pdf-o:before {
  content: "\f1c1";
}
.fa-file-word-o:before {
  content: "\f1c2";
}
.fa-file-excel-o:before {
  content: "\f1c3";
}
.fa-file-powerpoint-o:before {
  content: "\f1c4";
}
.fa-file-photo-o:before,
.fa-file-picture-o:before,
.fa-file-image-o:before {
  content: "\f1c5";
}
.fa-file-zip-o:before,
.fa-file-archive-o:before {
  content: "\f1c6";
}
.fa-file-sound-o:before,
.fa-file-audio-o:before {
  content: "\f1c7";
}
.fa-file-movie-o:before,
.fa-file-video-o:before {
  content: "\f1c8";
}
.fa-file-code-o:before {
  content: "\f1c9";
}
.fa-vine:before {
  content: "\f1ca";
}
.fa-codepen:before {
  content: "\f1cb";
}
.fa-jsfiddle:before {
  content: "\f1cc";
}
.fa-life-bouy:before,
.fa-life-buoy:before,
.fa-life-saver:before,
.fa-support:before,
.fa-life-ring:before {
  content: "\f1cd";
}
.fa-circle-o-notch:before {
  content: "\f1ce";
}
.fa-ra:before,
.fa-rebel:before {
  content: "\f1d0";
}
.fa-ge:before,
.fa-empire:before {
  content: "\f1d1";
}
.fa-git-square:before {
  content: "\f1d2";
}
.fa-git:before {
  content: "\f1d3";
}
.fa-hacker-news:before {
  content: "\f1d4";
}
.fa-tencent-weibo:before {
  content: "\f1d5";
}
.fa-qq:before {
  content: "\f1d6";
}
.fa-wechat:before,
.fa-weixin:before {
  content: "\f1d7";
}
.fa-send:before,
.fa-paper-plane:before {
  content: "\f1d8";
}
.fa-send-o:before,
.fa-paper-plane-o:before {
  content: "\f1d9";
}
.fa-history:before {
  content: "\f1da";
}
.fa-circle-thin:before {
  content: "\f1db";
}
.fa-header:before {
  content: "\f1dc";
}
.fa-paragraph:before {
  content: "\f1dd";
}
.fa-sliders:before {
  content: "\f1de";
}
.fa-share-alt:before {
  content: "\f1e0";
}
.fa-share-alt-square:before {
  content: "\f1e1";
}
.fa-bomb:before {
  content: "\f1e2";
}
.fa-soccer-ball-o:before,
.fa-futbol-o:before {
  content: "\f1e3";
}
.fa-tty:before {
  content: "\f1e4";
}
.fa-binoculars:before {
  content: "\f1e5";
}
.fa-plug:before {
  content: "\f1e6";
}
.fa-slideshare:before {
  content: "\f1e7";
}
.fa-twitch:before {
  content: "\f1e8";
}
.fa-yelp:before {
  content: "\f1e9";
}
.fa-newspaper-o:before {
  content: "\f1ea";
}
.fa-wifi:before {
  content: "\f1eb";
}
.fa-calculator:before {
  content: "\f1ec";
}
.fa-paypal:before {
  content: "\f1ed";
}
.fa-google-wallet:before {
  content: "\f1ee";
}
.fa-cc-visa:before {
  content: "\f1f0";
}
.fa-cc-mastercard:before {
  content: "\f1f1";
}
.fa-cc-discover:before {
  content: "\f1f2";
}
.fa-cc-amex:before {
  content: "\f1f3";
}
.fa-cc-paypal:before {
  content: "\f1f4";
}
.fa-cc-stripe:before {
  content: "\f1f5";
}
.fa-bell-slash:before {
  content: "\f1f6";
}
.fa-bell-slash-o:before {
  content: "\f1f7";
}
.fa-trash:before {
  content: "\f1f8";
}
.fa-copyright:before {
  content: "\f1f9";
}
.fa-at:before {
  content: "\f1fa";
}
.fa-eyedropper:before {
  content: "\f1fb";
}
.fa-paint-brush:before {
  content: "\f1fc";
}
.fa-birthday-cake:before {
  content: "\f1fd";
}
.fa-area-chart:before {
  content: "\f1fe";
}
.fa-pie-chart:before {
  content: "\f200";
}
.fa-line-chart:before {
  content: "\f201";
}
.fa-lastfm:before {
  content: "\f202";
}
.fa-lastfm-square:before {
  content: "\f203";
}
.fa-toggle-off:before {
  content: "\f204";
}
.fa-toggle-on:before {
  content: "\f205";
}
.fa-bicycle:before {
  content: "\f206";
}
.fa-bus:before {
  content: "\f207";
}
.fa-ioxhost:before {
  content: "\f208";
}
.fa-angellist:before {
  content: "\f209";
}
.fa-cc:before {
  content: "\f20a";
}
.fa-shekel:before,
.fa-sheqel:before,
.fa-ils:before {
  content: "\f20b";
}
.fa-meanpath:before {
  content: "\f20c";
}
/*!
*
* IPython base
*
*/
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
code {
  color: #000;
}
pre {
  font-size: inherit;
  line-height: inherit;
}
label {
  font-weight: normal;
}
/* Make the page background atleast 100% the height of the view port */
/* Make the page itself atleast 70% the height of the view port */
.border-box-sizing {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.corner-all {
  border-radius: 2px;
}
.no-padding {
  padding: 0px;
}
/* Flexible box model classes */
/* Taken from Alex Russell http://infrequently.org/2009/08/css-3-progress/ */
/* This file is a compatability layer.  It allows the usage of flexible box 
model layouts accross multiple browsers, including older browsers.  The newest,
universal implementation of the flexible box model is used when available (see
`Modern browsers` comments below).  Browsers that are known to implement this 
new spec completely include:

    Firefox 28.0+
    Chrome 29.0+
    Internet Explorer 11+ 
    Opera 17.0+

Browsers not listed, including Safari, are supported via the styling under the
`Old browsers` comments below.
*/
.hbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
.hbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.vbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
.vbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.hbox.reverse,
.vbox.reverse,
.reverse {
  /* Old browsers */
  -webkit-box-direction: reverse;
  -moz-box-direction: reverse;
  box-direction: reverse;
  /* Modern browsers */
  flex-direction: row-reverse;
}
.hbox.box-flex0,
.vbox.box-flex0,
.box-flex0 {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
  width: auto;
}
.hbox.box-flex1,
.vbox.box-flex1,
.box-flex1 {
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex,
.vbox.box-flex,
.box-flex {
  /* Old browsers */
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex2,
.vbox.box-flex2,
.box-flex2 {
  /* Old browsers */
  -webkit-box-flex: 2;
  -moz-box-flex: 2;
  box-flex: 2;
  /* Modern browsers */
  flex: 2;
}
.box-group1 {
  /*  Deprecated */
  -webkit-box-flex-group: 1;
  -moz-box-flex-group: 1;
  box-flex-group: 1;
}
.box-group2 {
  /* Deprecated */
  -webkit-box-flex-group: 2;
  -moz-box-flex-group: 2;
  box-flex-group: 2;
}
.hbox.start,
.vbox.start,
.start {
  /* Old browsers */
  -webkit-box-pack: start;
  -moz-box-pack: start;
  box-pack: start;
  /* Modern browsers */
  justify-content: flex-start;
}
.hbox.end,
.vbox.end,
.end {
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
}
.hbox.center,
.vbox.center,
.center {
  /* Old browsers */
  -webkit-box-pack: center;
  -moz-box-pack: center;
  box-pack: center;
  /* Modern browsers */
  justify-content: center;
}
.hbox.baseline,
.vbox.baseline,
.baseline {
  /* Old browsers */
  -webkit-box-pack: baseline;
  -moz-box-pack: baseline;
  box-pack: baseline;
  /* Modern browsers */
  justify-content: baseline;
}
.hbox.stretch,
.vbox.stretch,
.stretch {
  /* Old browsers */
  -webkit-box-pack: stretch;
  -moz-box-pack: stretch;
  box-pack: stretch;
  /* Modern browsers */
  justify-content: stretch;
}
.hbox.align-start,
.vbox.align-start,
.align-start {
  /* Old browsers */
  -webkit-box-align: start;
  -moz-box-align: start;
  box-align: start;
  /* Modern browsers */
  align-items: flex-start;
}
.hbox.align-end,
.vbox.align-end,
.align-end {
  /* Old browsers */
  -webkit-box-align: end;
  -moz-box-align: end;
  box-align: end;
  /* Modern browsers */
  align-items: flex-end;
}
.hbox.align-center,
.vbox.align-center,
.align-center {
  /* Old browsers */
  -webkit-box-align: center;
  -moz-box-align: center;
  box-align: center;
  /* Modern browsers */
  align-items: center;
}
.hbox.align-baseline,
.vbox.align-baseline,
.align-baseline {
  /* Old browsers */
  -webkit-box-align: baseline;
  -moz-box-align: baseline;
  box-align: baseline;
  /* Modern browsers */
  align-items: baseline;
}
.hbox.align-stretch,
.vbox.align-stretch,
.align-stretch {
  /* Old browsers */
  -webkit-box-align: stretch;
  -moz-box-align: stretch;
  box-align: stretch;
  /* Modern browsers */
  align-items: stretch;
}
div.error {
  margin: 2em;
  text-align: center;
}
div.error > h1 {
  font-size: 500%;
  line-height: normal;
}
div.error > p {
  font-size: 200%;
  line-height: normal;
}
div.traceback-wrapper {
  text-align: left;
  max-width: 800px;
  margin: auto;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
body {
  background-color: #fff;
  /* This makes sure that the body covers the entire window and needs to
       be in a different element than the display: box in wrapper below */
  position: absolute;
  left: 0px;
  right: 0px;
  top: 0px;
  bottom: 0px;
  overflow: visible;
}
body > #header {
  /* Initially hidden to prevent FLOUC */
  display: none;
  background-color: #fff;
  /* Display over codemirror */
  position: relative;
  z-index: 100;
}
body > #header #header-container {
  padding-bottom: 5px;
  padding-top: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
body > #header .header-bar {
  width: 100%;
  height: 1px;
  background: #e7e7e7;
  margin-bottom: -1px;
}
@media print {
  body > #header {
    display: none !important;
  }
}
#header-spacer {
  width: 100%;
  visibility: hidden;
}
@media print {
  #header-spacer {
    display: none;
  }
}
#ipython_notebook {
  padding-left: 0px;
  padding-top: 1px;
  padding-bottom: 1px;
}
@media (max-width: 991px) {
  #ipython_notebook {
    margin-left: 10px;
  }
}
[dir="rtl"] #ipython_notebook {
  float: right !important;
}
#noscript {
  width: auto;
  padding-top: 16px;
  padding-bottom: 16px;
  text-align: center;
  font-size: 22px;
  color: red;
  font-weight: bold;
}
#ipython_notebook img {
  height: 28px;
}
#site {
  width: 100%;
  display: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  overflow: auto;
}
@media print {
  #site {
    height: auto !important;
  }
}
/* Smaller buttons */
.ui-button .ui-button-text {
  padding: 0.2em 0.8em;
  font-size: 77%;
}
input.ui-button {
  padding: 0.3em 0.9em;
}
span#login_widget {
  float: right;
}
span#login_widget > .button,
#logout {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button:focus,
#logout:focus,
span#login_widget > .button.focus,
#logout.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
span#login_widget > .button:hover,
#logout:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active:hover,
#logout:active:hover,
span#login_widget > .button.active:hover,
#logout.active:hover,
.open > .dropdown-togglespan#login_widget > .button:hover,
.open > .dropdown-toggle#logout:hover,
span#login_widget > .button:active:focus,
#logout:active:focus,
span#login_widget > .button.active:focus,
#logout.active:focus,
.open > .dropdown-togglespan#login_widget > .button:focus,
.open > .dropdown-toggle#logout:focus,
span#login_widget > .button:active.focus,
#logout:active.focus,
span#login_widget > .button.active.focus,
#logout.active.focus,
.open > .dropdown-togglespan#login_widget > .button.focus,
.open > .dropdown-toggle#logout.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  background-image: none;
}
span#login_widget > .button.disabled:hover,
#logout.disabled:hover,
span#login_widget > .button[disabled]:hover,
#logout[disabled]:hover,
fieldset[disabled] span#login_widget > .button:hover,
fieldset[disabled] #logout:hover,
span#login_widget > .button.disabled:focus,
#logout.disabled:focus,
span#login_widget > .button[disabled]:focus,
#logout[disabled]:focus,
fieldset[disabled] span#login_widget > .button:focus,
fieldset[disabled] #logout:focus,
span#login_widget > .button.disabled.focus,
#logout.disabled.focus,
span#login_widget > .button[disabled].focus,
#logout[disabled].focus,
fieldset[disabled] span#login_widget > .button.focus,
fieldset[disabled] #logout.focus {
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button .badge,
#logout .badge {
  color: #fff;
  background-color: #333;
}
.nav-header {
  text-transform: none;
}
#header > span {
  margin-top: 10px;
}
.modal_stretch .modal-dialog {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  min-height: 80vh;
}
.modal_stretch .modal-dialog .modal-body {
  max-height: calc(100vh - 200px);
  overflow: auto;
  flex: 1;
}
@media (min-width: 768px) {
  .modal .modal-dialog {
    width: 700px;
  }
}
@media (min-width: 768px) {
  select.form-control {
    margin-left: 12px;
    margin-right: 12px;
  }
}
/*!
*
* IPython auth
*
*/
.center-nav {
  display: inline-block;
  margin-bottom: -4px;
}
/*!
*
* IPython tree view
*
*/
/* We need an invisible input field on top of the sentense*/
/* "Drag file onto the list ..." */
.alternate_upload {
  background-color: none;
  display: inline;
}
.alternate_upload.form {
  padding: 0;
  margin: 0;
}
.alternate_upload input.fileinput {
  text-align: center;
  vertical-align: middle;
  display: inline;
  opacity: 0;
  z-index: 2;
  width: 12ex;
  margin-right: -12ex;
}
.alternate_upload .btn-upload {
  height: 22px;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
[dir="rtl"] #tabs li {
  float: right;
}
ul#tabs {
  margin-bottom: 4px;
}
[dir="rtl"] ul#tabs {
  margin-right: 0px;
}
ul#tabs a {
  padding-top: 6px;
  padding-bottom: 4px;
}
ul.breadcrumb a:focus,
ul.breadcrumb a:hover {
  text-decoration: none;
}
ul.breadcrumb i.icon-home {
  font-size: 16px;
  margin-right: 4px;
}
ul.breadcrumb span {
  color: #5e5e5e;
}
.list_toolbar {
  padding: 4px 0 4px 0;
  vertical-align: middle;
}
.list_toolbar .tree-buttons {
  padding-top: 1px;
}
[dir="rtl"] .list_toolbar .tree-buttons {
  float: left !important;
}
[dir="rtl"] .list_toolbar .pull-right {
  padding-top: 1px;
  float: left !important;
}
[dir="rtl"] .list_toolbar .pull-left {
  float: right !important;
}
.dynamic-buttons {
  padding-top: 3px;
  display: inline-block;
}
.list_toolbar [class*="span"] {
  min-height: 24px;
}
.list_header {
  font-weight: bold;
  background-color: #EEE;
}
.list_placeholder {
  font-weight: bold;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
}
.list_container {
  margin-top: 4px;
  margin-bottom: 20px;
  border: 1px solid #ddd;
  border-radius: 2px;
}
.list_container > div {
  border-bottom: 1px solid #ddd;
}
.list_container > div:hover .list-item {
  background-color: red;
}
.list_container > div:last-child {
  border: none;
}
.list_item:hover .list_item {
  background-color: #ddd;
}
.list_item a {
  text-decoration: none;
}
.list_item:hover {
  background-color: #fafafa;
}
.list_header > div,
.list_item > div {
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
.list_header > div input,
.list_item > div input {
  margin-right: 7px;
  margin-left: 14px;
  vertical-align: baseline;
  line-height: 22px;
  position: relative;
  top: -1px;
}
.list_header > div .item_link,
.list_item > div .item_link {
  margin-left: -1px;
  vertical-align: baseline;
  line-height: 22px;
}
.new-file input[type=checkbox] {
  visibility: hidden;
}
.item_name {
  line-height: 22px;
  height: 24px;
}
.item_icon {
  font-size: 14px;
  color: #5e5e5e;
  margin-right: 7px;
  margin-left: 7px;
  line-height: 22px;
  vertical-align: baseline;
}
.item_buttons {
  line-height: 1em;
  margin-left: -5px;
}
.item_buttons .btn,
.item_buttons .btn-group,
.item_buttons .input-group {
  float: left;
}
.item_buttons > .btn,
.item_buttons > .btn-group,
.item_buttons > .input-group {
  margin-left: 5px;
}
.item_buttons .btn {
  min-width: 13ex;
}
.item_buttons .running-indicator {
  padding-top: 4px;
  color: #5cb85c;
}
.item_buttons .kernel-name {
  padding-top: 4px;
  color: #5bc0de;
  margin-right: 7px;
  float: left;
}
.toolbar_info {
  height: 24px;
  line-height: 24px;
}
.list_item input:not([type=checkbox]) {
  padding-top: 3px;
  padding-bottom: 3px;
  height: 22px;
  line-height: 14px;
  margin: 0px;
}
.highlight_text {
  color: blue;
}
#project_name {
  display: inline-block;
  padding-left: 7px;
  margin-left: -2px;
}
#project_name > .breadcrumb {
  padding: 0px;
  margin-bottom: 0px;
  background-color: transparent;
  font-weight: bold;
}
#tree-selector {
  padding-right: 0px;
}
[dir="rtl"] #tree-selector a {
  float: right;
}
#button-select-all {
  min-width: 50px;
}
#select-all {
  margin-left: 7px;
  margin-right: 2px;
}
.menu_icon {
  margin-right: 2px;
}
.tab-content .row {
  margin-left: 0px;
  margin-right: 0px;
}
.folder_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f114";
}
.folder_icon:before.pull-left {
  margin-right: .3em;
}
.folder_icon:before.pull-right {
  margin-left: .3em;
}
.notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
}
.notebook_icon:before.pull-left {
  margin-right: .3em;
}
.notebook_icon:before.pull-right {
  margin-left: .3em;
}
.running_notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
  color: #5cb85c;
}
.running_notebook_icon:before.pull-left {
  margin-right: .3em;
}
.running_notebook_icon:before.pull-right {
  margin-left: .3em;
}
.file_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f016";
  position: relative;
  top: -2px;
}
.file_icon:before.pull-left {
  margin-right: .3em;
}
.file_icon:before.pull-right {
  margin-left: .3em;
}
#notebook_toolbar .pull-right {
  padding-top: 0px;
  margin-right: -1px;
}
ul#new-menu {
  left: auto;
  right: 0;
}
[dir="rtl"] #new-menu {
  text-align: right;
}
.kernel-menu-icon {
  padding-right: 12px;
  width: 24px;
  content: "\f096";
}
.kernel-menu-icon:before {
  content: "\f096";
}
.kernel-menu-icon-current:before {
  content: "\f00c";
}
#tab_content {
  padding-top: 20px;
}
#running .panel-group .panel {
  margin-top: 3px;
  margin-bottom: 1em;
}
#running .panel-group .panel .panel-heading {
  background-color: #EEE;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
#running .panel-group .panel .panel-heading a:focus,
#running .panel-group .panel .panel-heading a:hover {
  text-decoration: none;
}
#running .panel-group .panel .panel-body {
  padding: 0px;
}
#running .panel-group .panel .panel-body .list_container {
  margin-top: 0px;
  margin-bottom: 0px;
  border: 0px;
  border-radius: 0px;
}
#running .panel-group .panel .panel-body .list_container .list_item {
  border-bottom: 1px solid #ddd;
}
#running .panel-group .panel .panel-body .list_container .list_item:last-child {
  border-bottom: 0px;
}
[dir="rtl"] #running .col-sm-8 {
  float: right !important;
}
.delete-button {
  display: none;
}
.duplicate-button {
  display: none;
}
.rename-button {
  display: none;
}
.shutdown-button {
  display: none;
}
.dynamic-instructions {
  display: inline-block;
  padding-top: 4px;
}
/*!
*
* IPython text editor webapp
*
*/
.selected-keymap i.fa {
  padding: 0px 5px;
}
.selected-keymap i.fa:before {
  content: "\f00c";
}
#mode-menu {
  overflow: auto;
  max-height: 20em;
}
.edit_app #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.edit_app #menubar .navbar {
  /* Use a negative 1 bottom margin, so the border overlaps the border of the
    header */
  margin-bottom: -1px;
}
.dirty-indicator {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator.pull-left {
  margin-right: .3em;
}
.dirty-indicator.pull-right {
  margin-left: .3em;
}
.dirty-indicator-dirty {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-dirty.pull-left {
  margin-right: .3em;
}
.dirty-indicator-dirty.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-clean.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f00c";
}
.dirty-indicator-clean:before.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean:before.pull-right {
  margin-left: .3em;
}
#filename {
  font-size: 16pt;
  display: table;
  padding: 0px 5px;
}
#current-mode {
  padding-left: 5px;
  padding-right: 5px;
}
#texteditor-backdrop {
  padding-top: 20px;
  padding-bottom: 20px;
}
@media not print {
  #texteditor-backdrop {
    background-color: #EEE;
  }
}
@media print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container {
    padding: 0px;
    background-color: #fff;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
/*!
*
* IPython notebook
*
*/
/* CSS font colors for translated ANSI colors. */
.ansibold {
  font-weight: bold;
}
/* use dark versions for foreground, to improve visibility */
.ansiblack {
  color: black;
}
.ansired {
  color: darkred;
}
.ansigreen {
  color: darkgreen;
}
.ansiyellow {
  color: #c4a000;
}
.ansiblue {
  color: darkblue;
}
.ansipurple {
  color: darkviolet;
}
.ansicyan {
  color: steelblue;
}
.ansigray {
  color: gray;
}
/* and light for background, for the same reason */
.ansibgblack {
  background-color: black;
}
.ansibgred {
  background-color: red;
}
.ansibggreen {
  background-color: green;
}
.ansibgyellow {
  background-color: yellow;
}
.ansibgblue {
  background-color: blue;
}
.ansibgpurple {
  background-color: magenta;
}
.ansibgcyan {
  background-color: cyan;
}
.ansibggray {
  background-color: gray;
}
div.cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  border-radius: 2px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  border-width: 1px;
  border-style: solid;
  border-color: transparent;
  width: 100%;
  padding: 5px;
  /* This acts as a spacer between cells, that is outside the border */
  margin: 0px;
  outline: none;
  border-left-width: 1px;
  padding-left: 5px;
  background: linear-gradient(to right, transparent -40px, transparent 1px, transparent 1px, transparent 100%);
}
div.cell.jupyter-soft-selected {
  border-left-color: #90CAF9;
  border-left-color: #E3F2FD;
  border-left-width: 1px;
  padding-left: 5px;
  border-right-color: #E3F2FD;
  border-right-width: 1px;
  background: #E3F2FD;
}
@media print {
  div.cell.jupyter-soft-selected {
    border-color: transparent;
  }
}
div.cell.selected {
  border-color: #ababab;
  border-left-width: 0px;
  padding-left: 6px;
  background: linear-gradient(to right, #42A5F5 -40px, #42A5F5 5px, transparent 5px, transparent 100%);
}
@media print {
  div.cell.selected {
    border-color: transparent;
  }
}
div.cell.selected.jupyter-soft-selected {
  border-left-width: 0;
  padding-left: 6px;
  background: linear-gradient(to right, #42A5F5 -40px, #42A5F5 7px, #E3F2FD 7px, #E3F2FD 100%);
}
.edit_mode div.cell.selected {
  border-color: #66BB6A;
  border-left-width: 0px;
  padding-left: 6px;
  background: linear-gradient(to right, #66BB6A -40px, #66BB6A 5px, transparent 5px, transparent 100%);
}
@media print {
  .edit_mode div.cell.selected {
    border-color: transparent;
  }
}
.prompt {
  /* This needs to be wide enough for 3 digit prompt numbers: In[100]: */
  min-width: 14ex;
  /* This padding is tuned to match the padding on the CodeMirror editor. */
  padding: 0.4em;
  margin: 0px;
  font-family: monospace;
  text-align: right;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
  /* Don't highlight prompt number selection */
  -webkit-touch-callout: none;
  -webkit-user-select: none;
  -khtml-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  /* Use default cursor */
  cursor: default;
}
@media (max-width: 540px) {
  .prompt {
    text-align: left;
  }
}
div.inner_cell {
  min-width: 0;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_area {
  border: 1px solid #cfcfcf;
  border-radius: 2px;
  background: #f7f7f7;
  line-height: 1.21429em;
}
/* This is needed so that empty prompt areas can collapse to zero height when there
   is no content in the output_subarea and the prompt. The main purpose of this is
   to make sure that empty JavaScript output_subareas have no height. */
div.prompt:empty {
  padding-top: 0;
  padding-bottom: 0;
}
div.unrecognized_cell {
  padding: 5px 5px 5px 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.unrecognized_cell .inner_cell {
  border-radius: 2px;
  padding: 5px;
  font-weight: bold;
  color: red;
  border: 1px solid #cfcfcf;
  background: #eaeaea;
}
div.unrecognized_cell .inner_cell a {
  color: inherit;
  text-decoration: none;
}
div.unrecognized_cell .inner_cell a:hover {
  color: inherit;
  text-decoration: none;
}
@media (max-width: 540px) {
  div.unrecognized_cell > div.prompt {
    display: none;
  }
}
div.code_cell {
  /* avoid page breaking on code cells when printing */
}
@media print {
  div.code_cell {
    page-break-inside: avoid;
  }
}
/* any special styling for code cells that are currently running goes here */
div.input {
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.input {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_prompt {
  color: #303F9F;
  border-top: 1px solid transparent;
}
div.input_area > div.highlight {
  margin: 0.4em;
  border: none;
  padding: 0px;
  background-color: transparent;
}
div.input_area > div.highlight > pre {
  margin: 0px;
  border: none;
  padding: 0px;
  background-color: transparent;
}
/* The following gets added to the <head> if it is detected that the user has a
 * monospace font with inconsistent normal/bold/italic height.  See
 * notebookmain.js.  Such fonts will have keywords vertically offset with
 * respect to the rest of the text.  The user should select a better font.
 * See: https://github.com/ipython/ipython/issues/1503
 *
 * .CodeMirror span {
 *      vertical-align: bottom;
 * }
 */
.CodeMirror {
  line-height: 1.21429em;
  /* Changed from 1em to our global default */
  font-size: 14px;
  height: auto;
  /* Changed to auto to autogrow */
  background: none;
  /* Changed from white to allow our bg to show through */
}
.CodeMirror-scroll {
  /*  The CodeMirror docs are a bit fuzzy on if overflow-y should be hidden or visible.*/
  /*  We have found that if it is visible, vertical scrollbars appear with font size changes.*/
  overflow-y: hidden;
  overflow-x: auto;
}
.CodeMirror-lines {
  /* In CM2, this used to be 0.4em, but in CM3 it went to 4px. We need the em value because */
  /* we have set a different line-height and want this to scale with that. */
  padding: 0.4em;
}
.CodeMirror-linenumber {
  padding: 0 8px 0 4px;
}
.CodeMirror-gutters {
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.CodeMirror pre {
  /* In CM3 this went to 4px from 0 in CM2. We need the 0 value because of how we size */
  /* .CodeMirror-lines */
  padding: 0;
  border: 0;
  border-radius: 0;
}
/*

Original style from softwaremaniacs.org (c) Ivan Sagalaev <Maniac@SoftwareManiacs.Org>
Adapted from GitHub theme

*/
.highlight-base {
  color: #000;
}
.highlight-variable {
  color: #000;
}
.highlight-variable-2 {
  color: #1a1a1a;
}
.highlight-variable-3 {
  color: #333333;
}
.highlight-string {
  color: #BA2121;
}
.highlight-comment {
  color: #408080;
  font-style: italic;
}
.highlight-number {
  color: #080;
}
.highlight-atom {
  color: #88F;
}
.highlight-keyword {
  color: #008000;
  font-weight: bold;
}
.highlight-builtin {
  color: #008000;
}
.highlight-error {
  color: #f00;
}
.highlight-operator {
  color: #AA22FF;
  font-weight: bold;
}
.highlight-meta {
  color: #AA22FF;
}
/* previously not defined, copying from default codemirror */
.highlight-def {
  color: #00f;
}
.highlight-string-2 {
  color: #f50;
}
.highlight-qualifier {
  color: #555;
}
.highlight-bracket {
  color: #997;
}
.highlight-tag {
  color: #170;
}
.highlight-attribute {
  color: #00c;
}
.highlight-header {
  color: blue;
}
.highlight-quote {
  color: #090;
}
.highlight-link {
  color: #00c;
}
/* apply the same style to codemirror */
.cm-s-ipython span.cm-keyword {
  color: #008000;
  font-weight: bold;
}
.cm-s-ipython span.cm-atom {
  color: #88F;
}
.cm-s-ipython span.cm-number {
  color: #080;
}
.cm-s-ipython span.cm-def {
  color: #00f;
}
.cm-s-ipython span.cm-variable {
  color: #000;
}
.cm-s-ipython span.cm-operator {
  color: #AA22FF;
  font-weight: bold;
}
.cm-s-ipython span.cm-variable-2 {
  color: #1a1a1a;
}
.cm-s-ipython span.cm-variable-3 {
  color: #333333;
}
.cm-s-ipython span.cm-comment {
  color: #408080;
  font-style: italic;
}
.cm-s-ipython span.cm-string {
  color: #BA2121;
}
.cm-s-ipython span.cm-string-2 {
  color: #f50;
}
.cm-s-ipython span.cm-meta {
  color: #AA22FF;
}
.cm-s-ipython span.cm-qualifier {
  color: #555;
}
.cm-s-ipython span.cm-builtin {
  color: #008000;
}
.cm-s-ipython span.cm-bracket {
  color: #997;
}
.cm-s-ipython span.cm-tag {
  color: #170;
}
.cm-s-ipython span.cm-attribute {
  color: #00c;
}
.cm-s-ipython span.cm-header {
  color: blue;
}
.cm-s-ipython span.cm-quote {
  color: #090;
}
.cm-s-ipython span.cm-link {
  color: #00c;
}
.cm-s-ipython span.cm-error {
  color: #f00;
}
.cm-s-ipython span.cm-tab {
  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAMCAYAAAAkuj5RAAAAAXNSR0IArs4c6QAAAGFJREFUSMft1LsRQFAQheHPowAKoACx3IgEKtaEHujDjORSgWTH/ZOdnZOcM/sgk/kFFWY0qV8foQwS4MKBCS3qR6ixBJvElOobYAtivseIE120FaowJPN75GMu8j/LfMwNjh4HUpwg4LUAAAAASUVORK5CYII=);
  background-position: right;
  background-repeat: no-repeat;
}
div.output_wrapper {
  /* this position must be relative to enable descendents to be absolute within it */
  position: relative;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  z-index: 1;
}
/* class for the output area when it should be height-limited */
div.output_scroll {
  /* ideally, this would be max-height, but FF barfs all over that */
  height: 24em;
  /* FF needs this *and the wrapper* to specify full width, or it will shrinkwrap */
  width: 100%;
  overflow: auto;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  display: block;
}
/* output div while it is collapsed */
div.output_collapsed {
  margin: 0px;
  padding: 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
div.out_prompt_overlay {
  height: 100%;
  padding: 0px 0.4em;
  position: absolute;
  border-radius: 2px;
}
div.out_prompt_overlay:hover {
  /* use inner shadow to get border that is computed the same on WebKit/FF */
  -webkit-box-shadow: inset 0 0 1px #000;
  box-shadow: inset 0 0 1px #000;
  background: rgba(240, 240, 240, 0.5);
}
div.output_prompt {
  color: #D84315;
}
/* This class is the outer container of all output sections. */
div.output_area {
  padding: 0px;
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.output_area .MathJax_Display {
  text-align: left !important;
}
div.output_area .rendered_html table {
  margin-left: 0;
  margin-right: 0;
}
div.output_area .rendered_html img {
  margin-left: 0;
  margin-right: 0;
}
div.output_area img,
div.output_area svg {
  max-width: 100%;
  height: auto;
}
div.output_area img.unconfined,
div.output_area svg.unconfined {
  max-width: none;
}
/* This is needed to protect the pre formating from global settings such
   as that of bootstrap */
.output {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.output_area {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
div.output_area pre {
  margin: 0;
  padding: 0;
  border: 0;
  vertical-align: baseline;
  color: black;
  background-color: transparent;
  border-radius: 0;
}
/* This class is for the output subarea inside the output_area and after
   the prompt div. */
div.output_subarea {
  overflow-x: auto;
  padding: 0.4em;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
  max-width: calc(100% - 14ex);
}
div.output_scroll div.output_subarea {
  overflow-x: visible;
}
/* The rest of the output_* classes are for special styling of the different
   output types */
/* all text output has this class: */
div.output_text {
  text-align: left;
  color: #000;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
}
/* stdout/stderr are 'text' as well as 'stream', but execute_result/error are *not* streams */
div.output_stderr {
  background: #fdd;
  /* very light red background for stderr */
}
div.output_latex {
  text-align: left;
}
/* Empty output_javascript divs should have no height */
div.output_javascript:empty {
  padding: 0;
}
.js-error {
  color: darkred;
}
/* raw_input styles */
div.raw_input_container {
  line-height: 1.21429em;
  padding-top: 5px;
}
pre.raw_input_prompt {
  /* nothing needed here. */
}
input.raw_input {
  font-family: monospace;
  font-size: inherit;
  color: inherit;
  width: auto;
  /* make sure input baseline aligns with prompt */
  vertical-align: baseline;
  /* padding + margin = 0.5em between prompt and cursor */
  padding: 0em 0.25em;
  margin: 0em 0.25em;
}
input.raw_input:focus {
  box-shadow: none;
}
p.p-space {
  margin-bottom: 10px;
}
div.output_unrecognized {
  padding: 5px;
  font-weight: bold;
  color: red;
}
div.output_unrecognized a {
  color: inherit;
  text-decoration: none;
}
div.output_unrecognized a:hover {
  color: inherit;
  text-decoration: none;
}
.rendered_html {
  color: #000;
  /* any extras will just be numbers: */
}
.rendered_html em {
  font-style: italic;
}
.rendered_html strong {
  font-weight: bold;
}
.rendered_html u {
  text-decoration: underline;
}
.rendered_html :link {
  text-decoration: underline;
}
.rendered_html :visited {
  text-decoration: underline;
}
.rendered_html h1 {
  font-size: 185.7%;
  margin: 1.08em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h2 {
  font-size: 157.1%;
  margin: 1.27em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h3 {
  font-size: 128.6%;
  margin: 1.55em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h4 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h5 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h6 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h1:first-child {
  margin-top: 0.538em;
}
.rendered_html h2:first-child {
  margin-top: 0.636em;
}
.rendered_html h3:first-child {
  margin-top: 0.777em;
}
.rendered_html h4:first-child {
  margin-top: 1em;
}
.rendered_html h5:first-child {
  margin-top: 1em;
}
.rendered_html h6:first-child {
  margin-top: 1em;
}
.rendered_html ul {
  list-style: disc;
  margin: 0em 2em;
  padding-left: 0px;
}
.rendered_html ul ul {
  list-style: square;
  margin: 0em 2em;
}
.rendered_html ul ul ul {
  list-style: circle;
  margin: 0em 2em;
}
.rendered_html ol {
  list-style: decimal;
  margin: 0em 2em;
  padding-left: 0px;
}
.rendered_html ol ol {
  list-style: upper-alpha;
  margin: 0em 2em;
}
.rendered_html ol ol ol {
  list-style: lower-alpha;
  margin: 0em 2em;
}
.rendered_html ol ol ol ol {
  list-style: lower-roman;
  margin: 0em 2em;
}
.rendered_html ol ol ol ol ol {
  list-style: decimal;
  margin: 0em 2em;
}
.rendered_html * + ul {
  margin-top: 1em;
}
.rendered_html * + ol {
  margin-top: 1em;
}
.rendered_html hr {
  color: black;
  background-color: black;
}
.rendered_html pre {
  margin: 1em 2em;
}
.rendered_html pre,
.rendered_html code {
  border: 0;
  background-color: #fff;
  color: #000;
  font-size: 100%;
  padding: 0px;
}
.rendered_html blockquote {
  margin: 1em 2em;
}
.rendered_html table {
  margin-left: auto;
  margin-right: auto;
  border: 1px solid black;
  border-collapse: collapse;
}
.rendered_html tr,
.rendered_html th,
.rendered_html td {
  border: 1px solid black;
  border-collapse: collapse;
  margin: 1em 2em;
}
.rendered_html td,
.rendered_html th {
  text-align: left;
  vertical-align: middle;
  padding: 4px;
}
.rendered_html th {
  font-weight: bold;
}
.rendered_html * + table {
  margin-top: 1em;
}
.rendered_html p {
  text-align: left;
}
.rendered_html * + p {
  margin-top: 1em;
}
.rendered_html img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.rendered_html * + img {
  margin-top: 1em;
}
.rendered_html img,
.rendered_html svg {
  max-width: 100%;
  height: auto;
}
.rendered_html img.unconfined,
.rendered_html svg.unconfined {
  max-width: none;
}
div.text_cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.text_cell > div.prompt {
    display: none;
  }
}
div.text_cell_render {
  /*font-family: "Helvetica Neue", Arial, Helvetica, Geneva, sans-serif;*/
  outline: none;
  resize: none;
  width: inherit;
  border-style: none;
  padding: 0.5em 0.5em 0.5em 0.4em;
  color: #000;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
a.anchor-link:link {
  text-decoration: none;
  padding: 0px 20px;
  visibility: hidden;
}
h1:hover .anchor-link,
h2:hover .anchor-link,
h3:hover .anchor-link,
h4:hover .anchor-link,
h5:hover .anchor-link,
h6:hover .anchor-link {
  visibility: visible;
}
.text_cell.rendered .input_area {
  display: none;
}
.text_cell.rendered .rendered_html {
  overflow-x: auto;
  overflow-y: hidden;
}
.text_cell.unrendered .text_cell_render {
  display: none;
}
.cm-header-1,
.cm-header-2,
.cm-header-3,
.cm-header-4,
.cm-header-5,
.cm-header-6 {
  font-weight: bold;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
}
.cm-header-1 {
  font-size: 185.7%;
}
.cm-header-2 {
  font-size: 157.1%;
}
.cm-header-3 {
  font-size: 128.6%;
}
.cm-header-4 {
  font-size: 110%;
}
.cm-header-5 {
  font-size: 100%;
  font-style: italic;
}
.cm-header-6 {
  font-size: 100%;
  font-style: italic;
}
/*!
*
* IPython notebook webapp
*
*/
@media (max-width: 767px) {
  .notebook_app {
    padding-left: 0px;
    padding-right: 0px;
  }
}
#ipython-main-app {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook_panel {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook {
  font-size: 14px;
  line-height: 20px;
  overflow-y: hidden;
  overflow-x: auto;
  width: 100%;
  /* This spaces the page away from the edge of the notebook area */
  padding-top: 20px;
  margin: 0px;
  outline: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  min-height: 100%;
}
@media not print {
  #notebook-container {
    padding: 15px;
    background-color: #fff;
    min-height: 0;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
@media print {
  #notebook-container {
    width: 100%;
  }
}
div.ui-widget-content {
  border: 1px solid #ababab;
  outline: none;
}
pre.dialog {
  background-color: #f7f7f7;
  border: 1px solid #ddd;
  border-radius: 2px;
  padding: 0.4em;
  padding-left: 2em;
}
p.dialog {
  padding: 0.2em;
}
/* Word-wrap output correctly.  This is the CSS3 spelling, though Firefox seems
   to not honor it correctly.  Webkit browsers (Chrome, rekonq, Safari) do.
 */
pre,
code,
kbd,
samp {
  white-space: pre-wrap;
}
#fonttest {
  font-family: monospace;
}
p {
  margin-bottom: 0;
}
.end_space {
  min-height: 100px;
  transition: height .2s ease;
}
.notebook_app > #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
@media not print {
  .notebook_app {
    background-color: #EEE;
  }
}
kbd {
  border-style: solid;
  border-width: 1px;
  box-shadow: none;
  margin: 2px;
  padding-left: 2px;
  padding-right: 2px;
  padding-top: 1px;
  padding-bottom: 1px;
}
/* CSS for the cell toolbar */
.celltoolbar {
  border: thin solid #CFCFCF;
  border-bottom: none;
  background: #EEE;
  border-radius: 2px 2px 0px 0px;
  width: 100%;
  height: 29px;
  padding-right: 4px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
  display: -webkit-flex;
}
@media print {
  .celltoolbar {
    display: none;
  }
}
.ctb_hideshow {
  display: none;
  vertical-align: bottom;
}
/* ctb_show is added to the ctb_hideshow div to show the cell toolbar.
   Cell toolbars are only shown when the ctb_global_show class is also set.
*/
.ctb_global_show .ctb_show.ctb_hideshow {
  display: block;
}
.ctb_global_show .ctb_show + .input_area,
.ctb_global_show .ctb_show + div.text_cell_input,
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border-top-right-radius: 0px;
  border-top-left-radius: 0px;
}
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border: 1px solid #cfcfcf;
}
.celltoolbar {
  font-size: 87%;
  padding-top: 3px;
}
.celltoolbar select {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
  width: inherit;
  font-size: inherit;
  height: 22px;
  padding: 0px;
  display: inline-block;
}
.celltoolbar select:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.celltoolbar select::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.celltoolbar select:-ms-input-placeholder {
  color: #999;
}
.celltoolbar select::-webkit-input-placeholder {
  color: #999;
}
.celltoolbar select::-ms-expand {
  border: 0;
  background-color: transparent;
}
.celltoolbar select[disabled],
.celltoolbar select[readonly],
fieldset[disabled] .celltoolbar select {
  background-color: #eeeeee;
  opacity: 1;
}
.celltoolbar select[disabled],
fieldset[disabled] .celltoolbar select {
  cursor: not-allowed;
}
textarea.celltoolbar select {
  height: auto;
}
select.celltoolbar select {
  height: 30px;
  line-height: 30px;
}
textarea.celltoolbar select,
select[multiple].celltoolbar select {
  height: auto;
}
.celltoolbar label {
  margin-left: 5px;
  margin-right: 5px;
}
.completions {
  position: absolute;
  z-index: 110;
  overflow: hidden;
  border: 1px solid #ababab;
  border-radius: 2px;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  line-height: 1;
}
.completions select {
  background: white;
  outline: none;
  border: none;
  padding: 0px;
  margin: 0px;
  overflow: auto;
  font-family: monospace;
  font-size: 110%;
  color: #000;
  width: auto;
}
.completions select option.context {
  color: #286090;
}
#kernel_logo_widget {
  float: right !important;
  float: right;
}
#kernel_logo_widget .current_kernel_logo {
  display: none;
  margin-top: -1px;
  margin-bottom: -1px;
  width: 32px;
  height: 32px;
}
#menubar {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  margin-top: 1px;
}
#menubar .navbar {
  border-top: 1px;
  border-radius: 0px 0px 2px 2px;
  margin-bottom: 0px;
}
#menubar .navbar-toggle {
  float: left;
  padding-top: 7px;
  padding-bottom: 7px;
  border: none;
}
#menubar .navbar-collapse {
  clear: left;
}
.nav-wrapper {
  border-bottom: 1px solid #e7e7e7;
}
i.menu-icon {
  padding-top: 4px;
}
ul#help_menu li a {
  overflow: hidden;
  padding-right: 2.2em;
}
ul#help_menu li a i {
  margin-right: -1.2em;
}
.dropdown-submenu {
  position: relative;
}
.dropdown-submenu > .dropdown-menu {
  top: 0;
  left: 100%;
  margin-top: -6px;
  margin-left: -1px;
}
.dropdown-submenu:hover > .dropdown-menu {
  display: block;
}
.dropdown-submenu > a:after {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: block;
  content: "\f0da";
  float: right;
  color: #333333;
  margin-top: 2px;
  margin-right: -10px;
}
.dropdown-submenu > a:after.pull-left {
  margin-right: .3em;
}
.dropdown-submenu > a:after.pull-right {
  margin-left: .3em;
}
.dropdown-submenu:hover > a:after {
  color: #262626;
}
.dropdown-submenu.pull-left {
  float: none;
}
.dropdown-submenu.pull-left > .dropdown-menu {
  left: -100%;
  margin-left: 10px;
}
#notification_area {
  float: right !important;
  float: right;
  z-index: 10;
}
.indicator_area {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
#kernel_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  border-left: 1px solid;
}
#kernel_indicator .kernel_indicator_name {
  padding-left: 5px;
  padding-right: 5px;
}
#modal_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
#readonly-indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  margin-top: 2px;
  margin-bottom: 0px;
  margin-left: 0px;
  margin-right: 0px;
  display: none;
}
.modal_indicator:before {
  width: 1.28571429em;
  text-align: center;
}
.edit_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f040";
}
.edit_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.edit_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.command_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: ' ';
}
.command_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.command_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.kernel_idle_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f10c";
}
.kernel_idle_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_idle_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_busy_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f111";
}
.kernel_busy_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_busy_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_dead_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f1e2";
}
.kernel_dead_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_dead_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_disconnected_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f127";
}
.kernel_disconnected_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_disconnected_icon:before.pull-right {
  margin-left: .3em;
}
.notification_widget {
  color: #777;
  z-index: 10;
  background: rgba(240, 240, 240, 0.5);
  margin-right: 4px;
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget:focus,
.notification_widget.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.notification_widget:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active:hover,
.notification_widget.active:hover,
.open > .dropdown-toggle.notification_widget:hover,
.notification_widget:active:focus,
.notification_widget.active:focus,
.open > .dropdown-toggle.notification_widget:focus,
.notification_widget:active.focus,
.notification_widget.active.focus,
.open > .dropdown-toggle.notification_widget.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  background-image: none;
}
.notification_widget.disabled:hover,
.notification_widget[disabled]:hover,
fieldset[disabled] .notification_widget:hover,
.notification_widget.disabled:focus,
.notification_widget[disabled]:focus,
fieldset[disabled] .notification_widget:focus,
.notification_widget.disabled.focus,
.notification_widget[disabled].focus,
fieldset[disabled] .notification_widget.focus {
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget .badge {
  color: #fff;
  background-color: #333;
}
.notification_widget.warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning:focus,
.notification_widget.warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.notification_widget.warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active:hover,
.notification_widget.warning.active:hover,
.open > .dropdown-toggle.notification_widget.warning:hover,
.notification_widget.warning:active:focus,
.notification_widget.warning.active:focus,
.open > .dropdown-toggle.notification_widget.warning:focus,
.notification_widget.warning:active.focus,
.notification_widget.warning.active.focus,
.open > .dropdown-toggle.notification_widget.warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  background-image: none;
}
.notification_widget.warning.disabled:hover,
.notification_widget.warning[disabled]:hover,
fieldset[disabled] .notification_widget.warning:hover,
.notification_widget.warning.disabled:focus,
.notification_widget.warning[disabled]:focus,
fieldset[disabled] .notification_widget.warning:focus,
.notification_widget.warning.disabled.focus,
.notification_widget.warning[disabled].focus,
fieldset[disabled] .notification_widget.warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.notification_widget.success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success:focus,
.notification_widget.success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.notification_widget.success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active:hover,
.notification_widget.success.active:hover,
.open > .dropdown-toggle.notification_widget.success:hover,
.notification_widget.success:active:focus,
.notification_widget.success.active:focus,
.open > .dropdown-toggle.notification_widget.success:focus,
.notification_widget.success:active.focus,
.notification_widget.success.active.focus,
.open > .dropdown-toggle.notification_widget.success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  background-image: none;
}
.notification_widget.success.disabled:hover,
.notification_widget.success[disabled]:hover,
fieldset[disabled] .notification_widget.success:hover,
.notification_widget.success.disabled:focus,
.notification_widget.success[disabled]:focus,
fieldset[disabled] .notification_widget.success:focus,
.notification_widget.success.disabled.focus,
.notification_widget.success[disabled].focus,
fieldset[disabled] .notification_widget.success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.notification_widget.info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info:focus,
.notification_widget.info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.notification_widget.info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active:hover,
.notification_widget.info.active:hover,
.open > .dropdown-toggle.notification_widget.info:hover,
.notification_widget.info:active:focus,
.notification_widget.info.active:focus,
.open > .dropdown-toggle.notification_widget.info:focus,
.notification_widget.info:active.focus,
.notification_widget.info.active.focus,
.open > .dropdown-toggle.notification_widget.info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  background-image: none;
}
.notification_widget.info.disabled:hover,
.notification_widget.info[disabled]:hover,
fieldset[disabled] .notification_widget.info:hover,
.notification_widget.info.disabled:focus,
.notification_widget.info[disabled]:focus,
fieldset[disabled] .notification_widget.info:focus,
.notification_widget.info.disabled.focus,
.notification_widget.info[disabled].focus,
fieldset[disabled] .notification_widget.info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.notification_widget.danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger:focus,
.notification_widget.danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.notification_widget.danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active:hover,
.notification_widget.danger.active:hover,
.open > .dropdown-toggle.notification_widget.danger:hover,
.notification_widget.danger:active:focus,
.notification_widget.danger.active:focus,
.open > .dropdown-toggle.notification_widget.danger:focus,
.notification_widget.danger:active.focus,
.notification_widget.danger.active.focus,
.open > .dropdown-toggle.notification_widget.danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  background-image: none;
}
.notification_widget.danger.disabled:hover,
.notification_widget.danger[disabled]:hover,
fieldset[disabled] .notification_widget.danger:hover,
.notification_widget.danger.disabled:focus,
.notification_widget.danger[disabled]:focus,
fieldset[disabled] .notification_widget.danger:focus,
.notification_widget.danger.disabled.focus,
.notification_widget.danger[disabled].focus,
fieldset[disabled] .notification_widget.danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger .badge {
  color: #d9534f;
  background-color: #fff;
}
div#pager {
  background-color: #fff;
  font-size: 14px;
  line-height: 20px;
  overflow: hidden;
  display: none;
  position: fixed;
  bottom: 0px;
  width: 100%;
  max-height: 50%;
  padding-top: 8px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  /* Display over codemirror */
  z-index: 100;
  /* Hack which prevents jquery ui resizable from changing top. */
  top: auto !important;
}
div#pager pre {
  line-height: 1.21429em;
  color: #000;
  background-color: #f7f7f7;
  padding: 0.4em;
}
div#pager #pager-button-area {
  position: absolute;
  top: 8px;
  right: 20px;
}
div#pager #pager-contents {
  position: relative;
  overflow: auto;
  width: 100%;
  height: 100%;
}
div#pager #pager-contents #pager-container {
  position: relative;
  padding: 15px 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
div#pager .ui-resizable-handle {
  top: 0px;
  height: 8px;
  background: #f7f7f7;
  border-top: 1px solid #cfcfcf;
  border-bottom: 1px solid #cfcfcf;
  /* This injects handle bars (a short, wide = symbol) for 
        the resize handle. */
}
div#pager .ui-resizable-handle::after {
  content: '';
  top: 2px;
  left: 50%;
  height: 3px;
  width: 30px;
  margin-left: -15px;
  position: absolute;
  border-top: 1px solid #cfcfcf;
}
.quickhelp {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  line-height: 1.8em;
}
.shortcut_key {
  display: inline-block;
  width: 21ex;
  text-align: right;
  font-family: monospace;
}
.shortcut_descr {
  display: inline-block;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
span.save_widget {
  margin-top: 6px;
}
span.save_widget span.filename {
  height: 1em;
  line-height: 1em;
  padding: 3px;
  margin-left: 16px;
  border: none;
  font-size: 146.5%;
  border-radius: 2px;
}
span.save_widget span.filename:hover {
  background-color: #e6e6e6;
}
span.checkpoint_status,
span.autosave_status {
  font-size: small;
}
@media (max-width: 767px) {
  span.save_widget {
    font-size: small;
  }
  span.checkpoint_status,
  span.autosave_status {
    display: none;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  span.checkpoint_status {
    display: none;
  }
  span.autosave_status {
    font-size: x-small;
  }
}
.toolbar {
  padding: 0px;
  margin-left: -5px;
  margin-top: 2px;
  margin-bottom: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.toolbar select,
.toolbar label {
  width: auto;
  vertical-align: middle;
  margin-right: 2px;
  margin-bottom: 0px;
  display: inline;
  font-size: 92%;
  margin-left: 0.3em;
  margin-right: 0.3em;
  padding: 0px;
  padding-top: 3px;
}
.toolbar .btn {
  padding: 2px 8px;
}
.toolbar .btn-group {
  margin-top: 0px;
  margin-left: 5px;
}
#maintoolbar {
  margin-bottom: -3px;
  margin-top: -8px;
  border: 0px;
  min-height: 27px;
  margin-left: 0px;
  padding-top: 11px;
  padding-bottom: 3px;
}
#maintoolbar .navbar-text {
  float: none;
  vertical-align: middle;
  text-align: right;
  margin-left: 5px;
  margin-right: 0px;
  margin-top: 0px;
}
.select-xs {
  height: 24px;
}
.pulse,
.dropdown-menu > li > a.pulse,
li.pulse > a.dropdown-toggle,
li.pulse.open > a.dropdown-toggle {
  background-color: #F37626;
  color: white;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
/** WARNING IF YOU ARE EDITTING THIS FILE, if this is a .css file, It has a lot
 * of chance of beeing generated from the ../less/[samename].less file, you can
 * try to get back the less file by reverting somme commit in history
 **/
/*
 * We'll try to get something pretty, so we
 * have some strange css to have the scroll bar on
 * the left with fix button on the top right of the tooltip
 */
@-moz-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-webkit-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-moz-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@-webkit-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
/*properties of tooltip after "expand"*/
.bigtooltip {
  overflow: auto;
  height: 200px;
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
}
/*properties of tooltip before "expand"*/
.smalltooltip {
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
  text-overflow: ellipsis;
  overflow: hidden;
  height: 80px;
}
.tooltipbuttons {
  position: absolute;
  padding-right: 15px;
  top: 0px;
  right: 0px;
}
.tooltiptext {
  /*avoid the button to overlap on some docstring*/
  padding-right: 30px;
}
.ipython_tooltip {
  max-width: 700px;
  /*fade-in animation when inserted*/
  -webkit-animation: fadeOut 400ms;
  -moz-animation: fadeOut 400ms;
  animation: fadeOut 400ms;
  -webkit-animation: fadeIn 400ms;
  -moz-animation: fadeIn 400ms;
  animation: fadeIn 400ms;
  vertical-align: middle;
  background-color: #f7f7f7;
  overflow: visible;
  border: #ababab 1px solid;
  outline: none;
  padding: 3px;
  margin: 0px;
  padding-left: 7px;
  font-family: monospace;
  min-height: 50px;
  -moz-box-shadow: 0px 6px 10px -1px #adadad;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  border-radius: 2px;
  position: absolute;
  z-index: 1000;
}
.ipython_tooltip a {
  float: right;
}
.ipython_tooltip .tooltiptext pre {
  border: 0;
  border-radius: 0;
  font-size: 100%;
  background-color: #f7f7f7;
}
.pretooltiparrow {
  left: 0px;
  margin: 0px;
  top: -16px;
  width: 40px;
  height: 16px;
  overflow: hidden;
  position: absolute;
}
.pretooltiparrow:before {
  background-color: #f7f7f7;
  border: 1px #ababab solid;
  z-index: 11;
  content: "";
  position: absolute;
  left: 15px;
  top: 10px;
  width: 25px;
  height: 25px;
  -webkit-transform: rotate(45deg);
  -moz-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  -o-transform: rotate(45deg);
}
ul.typeahead-list i {
  margin-left: -10px;
  width: 18px;
}
ul.typeahead-list {
  max-height: 80vh;
  overflow: auto;
}
ul.typeahead-list > li > a {
  /** Firefox bug **/
  /* see https://github.com/jupyter/notebook/issues/559 */
  white-space: normal;
}
.cmd-palette .modal-body {
  padding: 7px;
}
.cmd-palette form {
  background: white;
}
.cmd-palette input {
  outline: none;
}
.no-shortcut {
  display: none;
}
.command-shortcut:before {
  content: "(command)";
  padding-right: 3px;
  color: #777777;
}
.edit-shortcut:before {
  content: "(edit)";
  padding-right: 3px;
  color: #777777;
}
#find-and-replace #replace-preview .match,
#find-and-replace #replace-preview .insert {
  background-color: #BBDEFB;
  border-color: #90CAF9;
  border-style: solid;
  border-width: 1px;
  border-radius: 0px;
}
#find-and-replace #replace-preview .replace .match {
  background-color: #FFCDD2;
  border-color: #EF9A9A;
  border-radius: 0px;
}
#find-and-replace #replace-preview .replace .insert {
  background-color: #C8E6C9;
  border-color: #A5D6A7;
  border-radius: 0px;
}
#find-and-replace #replace-preview {
  max-height: 60vh;
  overflow: auto;
}
#find-and-replace #replace-preview pre {
  padding: 5px 10px;
}
.terminal-app {
  background: #EEE;
}
.terminal-app #header {
  background: #fff;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.terminal-app .terminal {
  width: 100%;
  float: left;
  font-family: monospace;
  color: white;
  background: black;
  padding: 0.4em;
  border-radius: 2px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
}
.terminal-app .terminal,
.terminal-app .terminal dummy-screen {
  line-height: 1em;
  font-size: 14px;
}
.terminal-app .terminal .xterm-rows {
  padding: 10px;
}
.terminal-app .terminal-cursor {
  color: black;
  background: white;
}
.terminal-app #terminado-container {
  margin-top: 20px;
}
/*# sourceMappingURL=style.min.css.map */
    </style>
<style type="text/css">
    .highlight .hll { background-color: #ffffcc }
.highlight  { background: #f8f8f8; }
.highlight .c { color: #408080; font-style: italic } /* Comment */
.highlight .err { border: 1px solid #FF0000 } /* Error */
.highlight .k { color: #008000; font-weight: bold } /* Keyword */
.highlight .o { color: #666666 } /* Operator */
.highlight .ch { color: #408080; font-style: italic } /* Comment.Hashbang */
.highlight .cm { color: #408080; font-style: italic } /* Comment.Multiline */
.highlight .cp { color: #BC7A00 } /* Comment.Preproc */
.highlight .cpf { color: #408080; font-style: italic } /* Comment.PreprocFile */
.highlight .c1 { color: #408080; font-style: italic } /* Comment.Single */
.highlight .cs { color: #408080; font-style: italic } /* Comment.Special */
.highlight .gd { color: #A00000 } /* Generic.Deleted */
.highlight .ge { font-style: italic } /* Generic.Emph */
.highlight .gr { color: #FF0000 } /* Generic.Error */
.highlight .gh { color: #000080; font-weight: bold } /* Generic.Heading */
.highlight .gi { color: #00A000 } /* Generic.Inserted */
.highlight .go { color: #888888 } /* Generic.Output */
.highlight .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
.highlight .gs { font-weight: bold } /* Generic.Strong */
.highlight .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
.highlight .gt { color: #0044DD } /* Generic.Traceback */
.highlight .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
.highlight .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
.highlight .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
.highlight .kp { color: #008000 } /* Keyword.Pseudo */
.highlight .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
.highlight .kt { color: #B00040 } /* Keyword.Type */
.highlight .m { color: #666666 } /* Literal.Number */
.highlight .s { color: #BA2121 } /* Literal.String */
.highlight .na { color: #7D9029 } /* Name.Attribute */
.highlight .nb { color: #008000 } /* Name.Builtin */
.highlight .nc { color: #0000FF; font-weight: bold } /* Name.Class */
.highlight .no { color: #880000 } /* Name.Constant */
.highlight .nd { color: #AA22FF } /* Name.Decorator */
.highlight .ni { color: #999999; font-weight: bold } /* Name.Entity */
.highlight .ne { color: #D2413A; font-weight: bold } /* Name.Exception */
.highlight .nf { color: #0000FF } /* Name.Function */
.highlight .nl { color: #A0A000 } /* Name.Label */
.highlight .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
.highlight .nt { color: #008000; font-weight: bold } /* Name.Tag */
.highlight .nv { color: #19177C } /* Name.Variable */
.highlight .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
.highlight .w { color: #bbbbbb } /* Text.Whitespace */
.highlight .mb { color: #666666 } /* Literal.Number.Bin */
.highlight .mf { color: #666666 } /* Literal.Number.Float */
.highlight .mh { color: #666666 } /* Literal.Number.Hex */
.highlight .mi { color: #666666 } /* Literal.Number.Integer */
.highlight .mo { color: #666666 } /* Literal.Number.Oct */
.highlight .sa { color: #BA2121 } /* Literal.String.Affix */
.highlight .sb { color: #BA2121 } /* Literal.String.Backtick */
.highlight .sc { color: #BA2121 } /* Literal.String.Char */
.highlight .dl { color: #BA2121 } /* Literal.String.Delimiter */
.highlight .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
.highlight .s2 { color: #BA2121 } /* Literal.String.Double */
.highlight .se { color: #BB6622; font-weight: bold } /* Literal.String.Escape */
.highlight .sh { color: #BA2121 } /* Literal.String.Heredoc */
.highlight .si { color: #BB6688; font-weight: bold } /* Literal.String.Interpol */
.highlight .sx { color: #008000 } /* Literal.String.Other */
.highlight .sr { color: #BB6688 } /* Literal.String.Regex */
.highlight .s1 { color: #BA2121 } /* Literal.String.Single */
.highlight .ss { color: #19177C } /* Literal.String.Symbol */
.highlight .bp { color: #008000 } /* Name.Builtin.Pseudo */
.highlight .fm { color: #0000FF } /* Name.Function.Magic */
.highlight .vc { color: #19177C } /* Name.Variable.Class */
.highlight .vg { color: #19177C } /* Name.Variable.Global */
.highlight .vi { color: #19177C } /* Name.Variable.Instance */
.highlight .vm { color: #19177C } /* Name.Variable.Magic */
.highlight .il { color: #666666 } /* Literal.Number.Integer.Long */
    </style>
<style type="text/css">
    
/* Temporary definitions which will become obsolete with Notebook release 5.0 */
.ansi-black-fg { color: #3E424D; }
.ansi-black-bg { background-color: #3E424D; }
.ansi-black-intense-fg { color: #282C36; }
.ansi-black-intense-bg { background-color: #282C36; }
.ansi-red-fg { color: #E75C58; }
.ansi-red-bg { background-color: #E75C58; }
.ansi-red-intense-fg { color: #B22B31; }
.ansi-red-intense-bg { background-color: #B22B31; }
.ansi-green-fg { color: #00A250; }
.ansi-green-bg { background-color: #00A250; }
.ansi-green-intense-fg { color: #007427; }
.ansi-green-intense-bg { background-color: #007427; }
.ansi-yellow-fg { color: #DDB62B; }
.ansi-yellow-bg { background-color: #DDB62B; }
.ansi-yellow-intense-fg { color: #B27D12; }
.ansi-yellow-intense-bg { background-color: #B27D12; }
.ansi-blue-fg { color: #208FFB; }
.ansi-blue-bg { background-color: #208FFB; }
.ansi-blue-intense-fg { color: #0065CA; }
.ansi-blue-intense-bg { background-color: #0065CA; }
.ansi-magenta-fg { color: #D160C4; }
.ansi-magenta-bg { background-color: #D160C4; }
.ansi-magenta-intense-fg { color: #A03196; }
.ansi-magenta-intense-bg { background-color: #A03196; }
.ansi-cyan-fg { color: #60C6C8; }
.ansi-cyan-bg { background-color: #60C6C8; }
.ansi-cyan-intense-fg { color: #258F8F; }
.ansi-cyan-intense-bg { background-color: #258F8F; }
.ansi-white-fg { color: #C5C1B4; }
.ansi-white-bg { background-color: #C5C1B4; }
.ansi-white-intense-fg { color: #A1A6B2; }
.ansi-white-intense-bg { background-color: #A1A6B2; }

.ansi-bold { font-weight: bold; }

    </style>


<style type="text/css">
/* Overrides of notebook CSS for static HTML export */
body {
  overflow: visible;
  padding: 8px;
}

div#notebook {
  overflow: visible;
  border-top: none;
}@media print {
  div.cell {
    display: block;
    page-break-inside: avoid;
  } 
  div.output_wrapper { 
    display: block;
    page-break-inside: avoid; 
  }
  div.output { 
    display: block;
    page-break-inside: avoid; 
  }
}
</style>

<!-- Custom stylesheet, it must be in the same directory as the html file -->
<link rel="stylesheet" href="custom.css">

<!-- Loading mathjax macro -->
<!-- Load mathjax -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-AMS_HTML"></script>
    <!-- MathJax configuration -->
    <script type="text/x-mathjax-config">
    MathJax.Hub.Config({
        tex2jax: {
            inlineMath: [ ['$','$'], ["\\(","\\)"] ],
            displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
            processEscapes: true,
            processEnvironments: true
        },
        // Center justify equations in code and markdown cells. Elsewhere
        // we use CSS to left justify single line equations in code cells.
        displayAlign: 'center',
        "HTML-CSS": {
            styles: {'.MathJax_Display': {"margin": 0}},
            linebreaks: { automatic: true }
        }
    });
    </script>
    <!-- End of mathjax configuration --></head>
<body>
  <div tabindex="-1" id="notebook" class="border-box-sizing">
    <div class="container" id="notebook-container">

<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><h1><center>Projeto de análise de sobrevivente do desastre do Titanic.</center></h1></p>
<h2>Uma competição que está disponível no site do <a href='https://www.kaggle.com/c/titanic'>Kaggle</a> para os iniciantes</h2><p><h2>Minha referência e inspiração é o &lt;a href= '<a href="https://paulovasconcellos.com.br/o-que-o-naufr%C3%A1gio-do-titanic-nos-ensina-at%C3%A9-hoje-data-science-project-2fea8ff1c9b5'&gt;Paulo">https://paulovasconcellos.com.br/o-que-o-naufr%C3%A1gio-do-titanic-nos-ensina-at%C3%A9-hoje-data-science-project-2fea8ff1c9b5'&gt;Paulo</a> Vasconcellos&lt;/a&gt;</p>

</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<center><img src="mid.jpg" alt="Titanic" height="640" width="480"></center>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><h2>Importando as bibliotecas necessárias para o projeto.&lt;/h1&gt;</p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[1]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#https://github.com/paulozip/naufragio-titanic/blob/master/Titanic.ipynb</span>

<span class="c1">#Biblioteca de maninupação de dados</span>
<span class="kn">import</span> <span class="nn">pandas</span> <span class="k">as</span> <span class="nn">pd</span> <span class="c1">#biblioteca para criação de DataFrames</span>
<span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span> <span class="c1">#algebra</span>


<span class="c1">#Biblioteca de visualização</span>

<span class="kn">import</span> <span class="nn">seaborn</span> <span class="k">as</span> <span class="nn">sns</span> <span class="c1">#graficos mais atraentes</span>
<span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span> <span class="c1">#plotagem</span>
<span class="kn">import</span> <span class="nn">random</span> <span class="c1">#seleção de valores aleatórios para plotagem</span>
<span class="o">%</span><span class="k">matplotlib</span> inline

<span class="c1">#Biblioteca de machine learning</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3>Importando os dados do dataset.</h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[2]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#lendo o arquivo</span>
<span class="n">df</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">read_csv</span><span class="p">(</span><span class="s2">&quot;data/train.csv&quot;</span><span class="p">)</span> 
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3>Contanto linhas e colunas </h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[3]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Este dataset possui </span><span class="si">%s</span><span class="s1"> linhas e </span><span class="si">%s</span><span class="s1"> colunas&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="n">df</span><span class="o">.</span><span class="n">shape</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">df</span><span class="o">.</span><span class="n">shape</span><span class="p">[</span><span class="mi">1</span><span class="p">]))</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>Este dataset possui 891 linhas e 12 colunas
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3> Imprimindo os dados </h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[4]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[4]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>PassengerId</th>
      <th>Survived</th>
      <th>Pclass</th>
      <th>Name</th>
      <th>Sex</th>
      <th>Age</th>
      <th>SibSp</th>
      <th>Parch</th>
      <th>Ticket</th>
      <th>Fare</th>
      <th>Cabin</th>
      <th>Embarked</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>0</td>
      <td>3</td>
      <td>Braund, Mr. Owen Harris</td>
      <td>male</td>
      <td>22.0</td>
      <td>1</td>
      <td>0</td>
      <td>A/5 21171</td>
      <td>7.2500</td>
      <td>NaN</td>
      <td>S</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>1</td>
      <td>1</td>
      <td>Cumings, Mrs. John Bradley (Florence Briggs Th...</td>
      <td>female</td>
      <td>38.0</td>
      <td>1</td>
      <td>0</td>
      <td>PC 17599</td>
      <td>71.2833</td>
      <td>C85</td>
      <td>C</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>1</td>
      <td>3</td>
      <td>Heikkinen, Miss. Laina</td>
      <td>female</td>
      <td>26.0</td>
      <td>0</td>
      <td>0</td>
      <td>STON/O2. 3101282</td>
      <td>7.9250</td>
      <td>NaN</td>
      <td>S</td>
    </tr>
    <tr>
      <th>3</th>
      <td>4</td>
      <td>1</td>
      <td>1</td>
      <td>Futrelle, Mrs. Jacques Heath (Lily May Peel)</td>
      <td>female</td>
      <td>35.0</td>
      <td>1</td>
      <td>0</td>
      <td>113803</td>
      <td>53.1000</td>
      <td>C123</td>
      <td>S</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5</td>
      <td>0</td>
      <td>3</td>
      <td>Allen, Mr. William Henry</td>
      <td>male</td>
      <td>35.0</td>
      <td>0</td>
      <td>0</td>
      <td>373450</td>
      <td>8.0500</td>
      <td>NaN</td>
      <td>S</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[&nbsp;]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#cores para serem usadas nos gráficos</span>
<span class="n">cores</span> <span class="o">=</span> <span class="p">[</span>
         <span class="p">[</span><span class="s1">&#39;#0D47A1&#39;</span><span class="p">,</span><span class="s1">&#39;#1565C0&#39;</span><span class="p">,</span><span class="s1">&#39;#1976D2&#39;</span><span class="p">,</span><span class="s1">&#39;#1E88E5&#39;</span><span class="p">,</span><span class="s1">&#39;#2196F3&#39;</span><span class="p">],</span>
         <span class="p">[</span><span class="s1">&#39;#311B92&#39;</span><span class="p">,</span><span class="s1">&#39;#512DA8&#39;</span><span class="p">,</span><span class="s1">&#39;#673AB7&#39;</span><span class="p">,</span><span class="s1">&#39;#9575CD&#39;</span><span class="p">,</span><span class="s1">&#39;#B39DDB&#39;</span><span class="p">],</span>
         <span class="p">[</span><span class="s1">&#39;#1B5E20&#39;</span><span class="p">,</span><span class="s1">&#39;#388E3C&#39;</span><span class="p">,</span><span class="s1">&#39;#4CAF50&#39;</span><span class="p">,</span><span class="s1">&#39;#81C784&#39;</span><span class="p">,</span><span class="s1">&#39;#66BB6A&#39;</span><span class="p">],</span>
         <span class="p">[</span><span class="s1">&#39;#E65100&#39;</span><span class="p">,</span><span class="s1">&#39;#EF6C00&#39;</span><span class="p">,</span><span class="s1">&#39;#F57C00&#39;</span><span class="p">,</span><span class="s1">&#39;#FB8C00&#39;</span><span class="p">,</span><span class="s1">&#39;#FF9800&#39;</span><span class="p">],</span>
         <span class="p">[</span><span class="s1">&#39;#3E2723&#39;</span><span class="p">,</span><span class="s1">&#39;#4E342E&#39;</span><span class="p">,</span><span class="s1">&#39;#5D4037&#39;</span><span class="p">,</span><span class="s1">&#39;#6D4C41&#39;</span><span class="p">,</span><span class="s1">&#39;#795548&#39;</span><span class="p">],</span>
         <span class="p">[</span><span class="s1">&#39;#BF360C&#39;</span><span class="p">,</span><span class="s1">&#39;#D84315&#39;</span><span class="p">,</span><span class="s1">&#39;#E64A19&#39;</span><span class="p">,</span><span class="s1">&#39;#F4511E&#39;</span><span class="p">,</span><span class="s1">&#39;#FF5722&#39;</span><span class="p">],</span>
         <span class="p">[</span><span class="s1">&#39;#880E4F&#39;</span><span class="p">,</span><span class="s1">&#39;#AD1457&#39;</span><span class="p">,</span><span class="s1">&#39;#C2185B&#39;</span><span class="p">,</span><span class="s1">&#39;#D81B60&#39;</span><span class="p">,</span><span class="s1">&#39;#E91E63&#39;</span><span class="p">]</span>
        <span class="p">]</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3> Precisamos retiar as colunas que não são importantes para a análise.</h3>
<h3>Para isso vamos usar o comando drop, para retirar como um todo a coluna.</h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[5]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">drop</span><span class="p">([</span><span class="s1">&#39;Ticket&#39;</span><span class="p">,</span><span class="s1">&#39;Cabin&#39;</span><span class="p">,</span><span class="s1">&#39;PassengerId&#39;</span><span class="p">],</span> <span class="n">axis</span><span class="o">=</span><span class="mi">1</span><span class="p">,</span> <span class="n">inplace</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3>Para deixar as informações mais claras a qualquer leitor, irei renomear as colunas remanescentes.</h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[6]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="p">[</span><span class="s1">&#39;Sobreviveu&#39;</span><span class="p">,</span><span class="s1">&#39;Classe&#39;</span><span class="p">,</span><span class="s1">&#39;Nome&#39;</span><span class="p">,</span><span class="s1">&#39;Sexo&#39;</span><span class="p">,</span><span class="s1">&#39;Idade&#39;</span><span class="p">,</span><span class="s1">&#39;Irmãos/Cônjuge&#39;</span><span class="p">,</span><span class="s1">&#39;Pais/Crianças&#39;</span><span class="p">,</span><span class="s1">&#39;Tarifa&#39;</span><span class="p">,</span><span class="s1">&#39;Embarque&#39;</span><span class="p">]</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[7]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[7]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Sobreviveu</th>
      <th>Classe</th>
      <th>Nome</th>
      <th>Sexo</th>
      <th>Idade</th>
      <th>Irmãos/Cônjuge</th>
      <th>Pais/Crianças</th>
      <th>Tarifa</th>
      <th>Embarque</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>3</td>
      <td>Braund, Mr. Owen Harris</td>
      <td>male</td>
      <td>22.0</td>
      <td>1</td>
      <td>0</td>
      <td>7.2500</td>
      <td>S</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>1</td>
      <td>Cumings, Mrs. John Bradley (Florence Briggs Th...</td>
      <td>female</td>
      <td>38.0</td>
      <td>1</td>
      <td>0</td>
      <td>71.2833</td>
      <td>C</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1</td>
      <td>3</td>
      <td>Heikkinen, Miss. Laina</td>
      <td>female</td>
      <td>26.0</td>
      <td>0</td>
      <td>0</td>
      <td>7.9250</td>
      <td>S</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1</td>
      <td>1</td>
      <td>Futrelle, Mrs. Jacques Heath (Lily May Peel)</td>
      <td>female</td>
      <td>35.0</td>
      <td>1</td>
      <td>0</td>
      <td>53.1000</td>
      <td>S</td>
    </tr>
    <tr>
      <th>4</th>
      <td>0</td>
      <td>3</td>
      <td>Allen, Mr. William Henry</td>
      <td>male</td>
      <td>35.0</td>
      <td>0</td>
      <td>0</td>
      <td>8.0500</td>
      <td>S</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3>Começando a manipular os dados, para que fiquem mais simples para a avaliação</h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[8]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#trocando os valores numéricos para valores literais na coluna de Sobreviveu sim ou não.</span>
<span class="n">df</span><span class="p">[</span><span class="s1">&#39;Sobreviveu&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">df</span><span class="p">[</span><span class="s1">&#39;Sobreviveu&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">replace</span><span class="p">([</span><span class="mi">0</span><span class="p">,</span><span class="mi">1</span><span class="p">],[</span><span class="s1">&#39;Não&#39;</span><span class="p">,</span><span class="s1">&#39;Sim&#39;</span><span class="p">])</span>
<span class="c1">#Trocando os dados de inglês para portguês</span>
<span class="n">df</span><span class="p">[</span><span class="s1">&#39;Sexo&#39;</span><span class="p">]</span><span class="o">=</span> <span class="n">df</span><span class="p">[</span><span class="s1">&#39;Sexo&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">replace</span><span class="p">([</span><span class="s1">&#39;male&#39;</span><span class="p">,</span> <span class="s1">&#39;female&#39;</span><span class="p">],[</span><span class="s1">&#39;Masculino&#39;</span><span class="p">,</span> <span class="s1">&#39;Feminino&#39;</span><span class="p">])</span>
<span class="c1">#trocando as letras, pelos seus nomes correspondentes -&gt; Southampton,Queenstown,Cherbourg</span>
<span class="n">df</span><span class="p">[</span><span class="s1">&#39;Embarque&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">df</span><span class="p">[</span><span class="s1">&#39;Embarque&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">replace</span><span class="p">([</span><span class="s1">&#39;S&#39;</span><span class="p">,</span><span class="s1">&#39;Q&#39;</span><span class="p">,</span><span class="s1">&#39;C&#39;</span><span class="p">],[</span><span class="s1">&#39;Southampton&#39;</span><span class="p">,</span><span class="s1">&#39;Queenstown&#39;</span><span class="p">,</span><span class="s1">&#39;Cherbourg&#39;</span><span class="p">])</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[9]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[9]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Sobreviveu</th>
      <th>Classe</th>
      <th>Nome</th>
      <th>Sexo</th>
      <th>Idade</th>
      <th>Irmãos/Cônjuge</th>
      <th>Pais/Crianças</th>
      <th>Tarifa</th>
      <th>Embarque</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Não</td>
      <td>3</td>
      <td>Braund, Mr. Owen Harris</td>
      <td>Masculino</td>
      <td>22.0</td>
      <td>1</td>
      <td>0</td>
      <td>7.2500</td>
      <td>Southampton</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Sim</td>
      <td>1</td>
      <td>Cumings, Mrs. John Bradley (Florence Briggs Th...</td>
      <td>Feminino</td>
      <td>38.0</td>
      <td>1</td>
      <td>0</td>
      <td>71.2833</td>
      <td>Cherbourg</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Sim</td>
      <td>3</td>
      <td>Heikkinen, Miss. Laina</td>
      <td>Feminino</td>
      <td>26.0</td>
      <td>0</td>
      <td>0</td>
      <td>7.9250</td>
      <td>Southampton</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Sim</td>
      <td>1</td>
      <td>Futrelle, Mrs. Jacques Heath (Lily May Peel)</td>
      <td>Feminino</td>
      <td>35.0</td>
      <td>1</td>
      <td>0</td>
      <td>53.1000</td>
      <td>Southampton</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Não</td>
      <td>3</td>
      <td>Allen, Mr. William Henry</td>
      <td>Masculino</td>
      <td>35.0</td>
      <td>0</td>
      <td>0</td>
      <td>8.0500</td>
      <td>Southampton</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3>Verificando os tipos de dados que estamos trabalhando.</h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[10]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">dtypes</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[10]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>Sobreviveu         object
Classe              int64
Nome               object
Sexo               object
Idade             float64
Irmãos/Cônjuge      int64
Pais/Crianças       int64
Tarifa            float64
Embarque           object
dtype: object</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3>Fazendo a descrição dos dados.</h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[11]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">describe</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[11]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Classe</th>
      <th>Idade</th>
      <th>Irmãos/Cônjuge</th>
      <th>Pais/Crianças</th>
      <th>Tarifa</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>891.000000</td>
      <td>714.000000</td>
      <td>891.000000</td>
      <td>891.000000</td>
      <td>891.000000</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>2.308642</td>
      <td>29.699118</td>
      <td>0.523008</td>
      <td>0.381594</td>
      <td>32.204208</td>
    </tr>
    <tr>
      <th>std</th>
      <td>0.836071</td>
      <td>14.526497</td>
      <td>1.102743</td>
      <td>0.806057</td>
      <td>49.693429</td>
    </tr>
    <tr>
      <th>min</th>
      <td>1.000000</td>
      <td>0.420000</td>
      <td>0.000000</td>
      <td>0.000000</td>
      <td>0.000000</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>2.000000</td>
      <td>20.125000</td>
      <td>0.000000</td>
      <td>0.000000</td>
      <td>7.910400</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>3.000000</td>
      <td>28.000000</td>
      <td>0.000000</td>
      <td>0.000000</td>
      <td>14.454200</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>3.000000</td>
      <td>38.000000</td>
      <td>1.000000</td>
      <td>0.000000</td>
      <td>31.000000</td>
    </tr>
    <tr>
      <th>max</th>
      <td>3.000000</td>
      <td>80.000000</td>
      <td>8.000000</td>
      <td>6.000000</td>
      <td>512.329200</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3>Iremos criar um gráfico para analisar a quantidade de pessoas que sobreviveram ou não</h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[12]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#contando a quantidade de passageiros</span>
<span class="n">passageiros</span> <span class="o">=</span> <span class="n">sns</span><span class="o">.</span><span class="n">countplot</span><span class="p">(</span><span class="n">data</span><span class="o">=</span><span class="n">df</span><span class="p">,</span> <span class="n">x</span><span class="o">=</span><span class="s1">&#39;Sobreviveu&#39;</span><span class="p">,</span> <span class="n">hue</span><span class="o">=</span><span class="s1">&#39;Sexo&#39;</span><span class="p">,</span> <span class="n">palette</span><span class="o">=</span><span class="s1">&#39;Reds_d&#39;</span><span class="p">)</span>

<span class="c1">#posicionando valores acima das barras</span>
<span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">passageiros</span><span class="o">.</span><span class="n">patches</span><span class="p">:</span>
    <span class="n">b</span><span class="o">=</span><span class="n">p</span><span class="o">.</span><span class="n">get_bbox</span><span class="p">()</span>
    <span class="n">passageiros</span><span class="o">.</span><span class="n">annotate</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">{:.0f}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">b</span><span class="o">.</span><span class="n">y1</span> <span class="o">+</span> <span class="n">b</span><span class="o">.</span><span class="n">y0</span><span class="p">),</span> <span class="p">((</span><span class="n">b</span><span class="o">.</span><span class="n">x0</span> <span class="o">+</span> <span class="n">b</span><span class="o">.</span><span class="n">x1</span><span class="p">)</span><span class="o">/</span><span class="mi">2</span> <span class="o">-</span> <span class="mf">0.05</span><span class="p">,</span> <span class="n">b</span><span class="o">.</span><span class="n">y1</span> <span class="o">+</span> <span class="mi">20</span><span class="p">))</span>
    
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;QUANTIDADE DE SOBREVIVENTES/MORTOS</span><span class="se">\n</span><span class="s1"> Total: </span><span class="si">%s</span><span class="s1"> passageiros&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="n">df</span><span class="o">.</span><span class="n">shape</span><span class="p">[</span><span class="mi">0</span><span class="p">]))</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Sobreviveu (Sim ou Não)&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Número de sobreviventes&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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JeevC1zFZGbrvVdffZXXXntt6fTzzz/PzjvvzAcffLA0QSxcuJAXX3wRgLvvvpsPP/yQRx99lB/84AfMmTOHnXbaialTp/L6668DcOONN9KvX7+G35l65DMIM1vvzZs3b+kPfdOmTdl+++259tprOfnkkxk+fDhz585l0aJF/PCHP2SLLbZgxIgRjB07lq233prvf//7nHbaaYwaNYrrr7+eo48+emlD9imnnFLtXVsjThBmtt7bY489eOKJJ1Yob9euHY8++ugK5VOmTFn6fPjw4UufH3jggTz33HOVCbIKXMVkZmYlOUGYmVlJThBmZlaSE4SZmZXkBGFmZiU5QZiZWUm+zNXMGqX67mm5nN6KJTFkyBBuuukmABYtWkSHDh3Ya6+9uP/+++s1nmJTp05lwIABTJ48mQkTJjB69Gguv/zyim6zLk4QZmbZRhttxOTJk/n0009p1aoVf//73+nYsWODx9GnTx/69OnT4Nst5iomM7MChx9+OH/6058AuOWWWzjuuOOWznv66afZe++96dWrF/vssw+vvvoqAC+++CJ9+/alZ8+e9OjRY2m3HaNHj6ZHjx7svvvuHH/88QAMGzaMO++8c+k6N9544xViGDduHAMGDADgvPPO44QTTqB///5su+22y51V/OpXv2K33XZjt91249JLL63nd8JnEGZmyzn22GO54IILGDBgAJMmTeKEE05g/PjxAHTr1o3x48fTtGlTHnzwQc466yzuuusurr76ak477TSGDBnC559/zuLFi3nxxRcZOXIkTzzxBO3atePDDz9c7ZheeeUVHn74YT7++GN22mknTj31VCZNmsT111/PU089RUSw11570a9fP3r16lVfb4UThJlZoR49ejB16lRuueUWDj/88OXmzZ07l6FDh/Laa68hiYULFwKw9957c+GFFzJt2jQGDRrEDjvswEMPPcTRRx9Nu3btAGjbtu1qx/SVr3yFFi1a0KJFCzbffHPee+89HnvsMY488kg22mgjAAYNGsT48ePrNUG4isnMrMgRRxzBj370o+WqlwDOOeccDjjgACZPnswf//hHFixYAMA3vvEN7rvvPlq1asXhhx/OQw89VOu6mzZtypIlSwBYsmRJWUOb1ox0B6lb8kWLFq3Obq0yJwgzsyInnHAC5557Lt27d1+ufO7cuUsbrW+44Yal5W+88Qbb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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3>Por esse gráfico podemos deduzir que sobreviveram mais mulheres do que homens, sendo que a proporção de homens é maior</h3>
<h3>Vamos medir o quanto isso é apresentado em proporções, levando em consideração que a lei de maioridade da Inglaterra é de 10 anos. <a href ='https://super.abril.com.br/historia/qual-a-idade-da-maioridade/'> Artigo da revista Super Interessante.</a></h3><h3>Mas para esse caso, vamos levar em consideração a maioridade a partir dos 15 anos de idade.</h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[13]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">prioritarios</span> <span class="o">=</span> <span class="p">(</span><span class="n">df</span><span class="p">[</span><span class="s1">&#39;Idade&#39;</span><span class="p">]</span> <span class="o">&lt;=</span> <span class="mi">15</span><span class="p">)</span> <span class="o">&amp;</span> <span class="p">(</span><span class="n">df</span><span class="p">[</span><span class="s1">&#39;Idade&#39;</span><span class="p">]</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">)</span> <span class="o">|</span> <span class="p">(</span><span class="n">df</span><span class="p">[</span><span class="s1">&#39;Sexo&#39;</span><span class="p">]</span> <span class="o">==</span><span class="s1">&#39;Feminino&#39;</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[14]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">prioritarios</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[14]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>0    False
1     True
2     True
3     True
4    False
dtype: bool</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[15]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">prioritarios</span> <span class="o">=</span> <span class="n">df</span><span class="p">[</span><span class="n">prioritarios</span><span class="p">]</span>
</pre></div>

</div>
</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3>Iremos plotar um gráfico que mostra a proporção de pessoas que sobreviveram.</h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[16]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#contando a quantidade de passageiros</span>
<span class="n">passageiros</span> <span class="o">=</span> <span class="n">sns</span><span class="o">.</span><span class="n">countplot</span><span class="p">(</span><span class="n">data</span><span class="o">=</span><span class="n">df</span><span class="p">,</span> <span class="n">x</span><span class="o">=</span><span class="s1">&#39;Sobreviveu&#39;</span><span class="p">,</span> <span class="n">hue</span><span class="o">=</span><span class="s1">&#39;Sexo&#39;</span><span class="p">,</span> <span class="n">palette</span><span class="o">=</span><span class="s1">&#39;Reds_d&#39;</span><span class="p">)</span>

<span class="c1">#posicionando valores acima das barras</span>
<span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">passageiros</span><span class="o">.</span><span class="n">patches</span><span class="p">:</span>
    <span class="n">b</span><span class="o">=</span><span class="n">p</span><span class="o">.</span><span class="n">get_bbox</span><span class="p">()</span>
    <span class="n">passageiros</span><span class="o">.</span><span class="n">annotate</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">{:.0f}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">b</span><span class="o">.</span><span class="n">y1</span> <span class="o">+</span> <span class="n">b</span><span class="o">.</span><span class="n">y0</span><span class="p">),</span> <span class="p">((</span><span class="n">b</span><span class="o">.</span><span class="n">x0</span> <span class="o">+</span> <span class="n">b</span><span class="o">.</span><span class="n">x1</span><span class="p">)</span><span class="o">/</span><span class="mi">2</span> <span class="o">-</span> <span class="mf">0.05</span><span class="p">,</span> <span class="n">b</span><span class="o">.</span><span class="n">y1</span> <span class="o">+</span> <span class="mi">20</span><span class="p">))</span>
    
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;QUANTIDADE DE SOBREVIVENTES/MORTOS</span><span class="se">\n</span><span class="s1"> Total: </span><span class="si">%s</span><span class="s1"> passageiros&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="n">df</span><span class="o">.</span><span class="n">shape</span><span class="p">[</span><span class="mi">0</span><span class="p">]))</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Sobreviveu (Sim ou Não)&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Número de sobreviventes&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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JeevC1zFZGbrvVdffZXXXntt6fTzzz/PzjvvzAcffLA0QSxcuJAXX3wRgLvvvpsPP/yQRx99lB/84AfMmTOHnXbaialTp/L6668DcOONN9KvX7+G35l65DMIM1vvzZs3b+kPfdOmTdl+++259tprOfnkkxk+fDhz585l0aJF/PCHP2SLLbZgxIgRjB07lq233prvf//7nHbaaYwaNYrrr7+eo48+emlD9imnnFLtXVsjThBmtt7bY489eOKJJ1Yob9euHY8++ugK5VOmTFn6fPjw4UufH3jggTz33HOVCbIKXMVkZmYlOUGYmVlJThBmZlaSE4SZmZXkBGFmZiU5QZiZWUm+zNXMGqX67mm5nN6KJTFkyBBuuukmABYtWkSHDh3Ya6+9uP/+++s1nmJTp05lwIABTJ48mQkTJjB69Gguv/zyim6zLk4QZmbZRhttxOTJk/n0009p1aoVf//73+nYsWODx9GnTx/69OnT4Nst5iomM7MChx9+OH/6058AuOWWWzjuuOOWznv66afZe++96dWrF/vssw+vvvoqAC+++CJ9+/alZ8+e9OjRY2m3HaNHj6ZHjx7svvvuHH/88QAMGzaMO++8c+k6N9544xViGDduHAMGDADgvPPO44QTTqB///5su+22y51V/OpXv2K33XZjt91249JLL63nd8JnEGZmyzn22GO54IILGDBgAJMmTeKEE05g/PjxAHTr1o3x48fTtGlTHnzwQc466yzuuusurr76ak477TSGDBnC559/zuLFi3nxxRcZOXIkTzzxBO3atePDDz9c7ZheeeUVHn74YT7++GN22mknTj31VCZNmsT111/PU089RUSw11570a9fP3r16lVfb4UThJlZoR49ejB16lRuueUWDj/88OXmzZ07l6FDh/Laa68hiYULFwKw9957c+GFFzJt2jQGDRrEDjvswEMPPcTRRx9Nu3btAGjbtu1qx/SVr3yFFi1a0KJFCzbffHPee+89HnvsMY488kg22mgjAAYNGsT48ePrNUG4isnMrMgRRxzBj370o+WqlwDOOeccDjjgACZPnswf//hHFixYAMA3vvEN7rvvPlq1asXhhx/OQw89VOu6mzZtypIlSwBYsmRJWUOb1ox0B6lb8kWLFq3Obq0yJwgzsyInnHAC5557Lt27d1+ufO7cuUsbrW+44Yal5W+88Qbb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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3>

Através do gráfico acima, podemos ver que mais de 70% das mulheres (incluindo adultos e crianças) sobreviveram a tragédia. Já quando olhamos para os tripulantes masculinos, o número muda um pouco, onde apenas 52% das crianças do sexo masculino sobreviveram, ou seja, quase metade deles morreram no naufrágio.

Esses dados me deixaram curioso: será que o número de sobreviventes meninas foi muito maior que os sobreviventes meninos?
</h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[17]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#proporção de sobreviventes meninos e meninas no Titanic</span>

<span class="n">prioritarios</span><span class="p">[</span><span class="n">prioritarios</span><span class="p">[</span><span class="s1">&#39;Idade&#39;</span><span class="p">]</span> <span class="o">&lt;=</span> <span class="mi">15</span><span class="p">]</span><span class="o">.</span><span class="n">groupby</span><span class="p">(</span><span class="s1">&#39;Sexo&#39;</span><span class="p">)[</span><span class="s1">&#39;Sobreviveu&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">np</span><span class="o">.</span><span class="n">mean</span><span class="p">(</span><span class="n">x</span> <span class="o">==</span> <span class="s1">&#39;Sim&#39;</span><span class="p">))</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[17]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>Sexo
Feminino     0.651163
Masculino    0.525000
Name: Sobreviveu, dtype: float64</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3>A sobrevivência do que paga mais ?</h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[18]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#contando a quantidade de pessoas por classe do návio</span>
<span class="n">classePlot</span> <span class="o">=</span>  <span class="n">sns</span><span class="o">.</span><span class="n">countplot</span><span class="p">(</span><span class="n">data</span> <span class="o">=</span> <span class="n">df</span><span class="p">,</span><span class="n">x</span> <span class="o">=</span> <span class="s1">&#39;Classe&#39;</span><span class="p">,</span> <span class="n">hue</span><span class="o">=</span><span class="s1">&#39;Classe&#39;</span><span class="p">)</span>

<span class="c1">#posicionando valores acima das barras</span>
<span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">passageiros</span><span class="o">.</span><span class="n">patches</span><span class="p">:</span>
    <span class="n">b</span><span class="o">=</span><span class="n">p</span><span class="o">.</span><span class="n">get_bbox</span><span class="p">()</span>
    <span class="n">passageiros</span><span class="o">.</span><span class="n">annotate</span><span class="p">(</span><span class="s2">&quot;</span><span class="si">{:.0f}</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">b</span><span class="o">.</span><span class="n">y1</span> <span class="o">+</span> <span class="n">b</span><span class="o">.</span><span class="n">y0</span><span class="p">),</span> <span class="p">((</span><span class="n">b</span><span class="o">.</span><span class="n">x0</span> <span class="o">+</span> <span class="n">b</span><span class="o">.</span><span class="n">x1</span><span class="p">)</span><span class="o">/</span><span class="mi">2</span> <span class="o">-</span> <span class="mf">0.05</span><span class="p">,</span> <span class="n">b</span><span class="o">.</span><span class="n">y1</span> <span class="o">+</span> <span class="mi">20</span><span class="p">))</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3>Do gráfico acima tiramos a informação que há mais pessoas na 3ª classe</h3>
</div>
</div>
</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3>Vamos ver a proporção de pessoas por sexo nas devidas classes </h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[19]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#ax =  sns.countplot(data = df, hue =&#39;Classe&#39;, y=&#39;Classe&#39;)</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">sns</span><span class="o">.</span><span class="n">factorplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s2">&quot;Classe&quot;</span><span class="p">,</span> <span class="n">hue</span><span class="o">=</span><span class="s2">&quot;Classe&quot;</span><span class="p">,</span> <span class="n">col</span><span class="o">=</span><span class="s2">&quot;Sexo&quot;</span><span class="p">,</span><span class="n">data</span><span class="o">=</span><span class="n">df</span><span class="p">,</span> <span class="n">kind</span><span class="o">=</span><span class="s2">&quot;count&quot;</span><span class="p">,</span><span class="n">size</span><span class="o">=</span><span class="mi">4</span><span class="p">,</span> <span class="n">aspect</span><span class="o">=.</span><span class="mi">7</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<H3>Verificando a quantidade de sobreviventes na relação Sexo por Classe</H3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[20]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">g</span> <span class="o">=</span> <span class="n">sns</span><span class="o">.</span><span class="n">factorplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="s2">&quot;Classe&quot;</span><span class="p">,</span> <span class="n">hue</span><span class="o">=</span><span class="s2">&quot;Classe&quot;</span><span class="p">,</span> <span class="n">col</span><span class="o">=</span><span class="s2">&quot;Sobreviveu&quot;</span><span class="p">,</span><span class="n">data</span><span class="o">=</span><span class="n">df</span><span class="p">,</span> <span class="n">kind</span><span class="o">=</span><span class="s2">&quot;count&quot;</span><span class="p">,</span><span class="n">size</span><span class="o">=</span><span class="mi">4</span><span class="p">,</span> <span class="n">aspect</span><span class="o">=.</span><span class="mi">7</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[21]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#agrupando a proporção de sobreviventes por classe e gerando um gráfico a partir do resultado</span>
<span class="n">sobreviventes_classe</span> <span class="o">=</span> <span class="n">df</span><span class="o">.</span><span class="n">copy</span><span class="p">()</span>
<span class="n">sobreviventes_classe</span><span class="p">[</span><span class="s1">&#39;Sobreviveu&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">df</span><span class="p">[</span><span class="s1">&#39;Sobreviveu&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;Sim&#39;</span>

<span class="n">sns</span><span class="o">.</span><span class="n">barplot</span><span class="p">(</span><span class="n">data</span><span class="o">=</span><span class="n">sobreviventes_classe</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="s1">&#39;Sobreviveu&#39;</span><span class="p">,</span> <span class="n">x</span><span class="o">=</span><span class="s1">&#39;Classe&#39;</span><span class="p">)</span>

<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;PROPORÇÃO DE SOBREVIVENTES POR CLASSE&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Proporção&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3>Proporção de sobreviventes por classe</h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[23]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#filtrando o dataset para conter dados apenas de pessoas que sobreviveram</span>
<span class="n">classe_sobrevivente</span> <span class="o">=</span> <span class="n">df</span><span class="p">[</span><span class="n">df</span><span class="p">[</span><span class="s1">&#39;Sobreviveu&#39;</span><span class="p">]</span> <span class="o">==</span> <span class="s1">&#39;Sim&#39;</span><span class="p">][</span><span class="s1">&#39;Classe&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">value_counts</span><span class="p">()</span><span class="o">.</span><span class="n">sort_values</span><span class="p">(</span><span class="n">ascending</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">classe_sobrevivente</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">kind</span><span class="o">=</span><span class="s1">&#39;barh&#39;</span><span class="p">,</span> <span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">11</span><span class="p">,</span><span class="mi">5</span><span class="p">),</span> <span class="n">color</span><span class="o">=</span><span class="n">random</span><span class="o">.</span><span class="n">choice</span><span class="p">(</span><span class="n">cores</span><span class="p">),</span> <span class="n">rot</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">grid</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>

<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;QUANTIDADE DE SOBREVIVENTES POR CLASSE</span><span class="se">\n</span><span class="s1"> Total: </span><span class="si">%s</span><span class="s1"> sobreviventes&#39;</span> <span class="o">%</span> <span class="p">(</span><span class="n">classe_sobrevivente</span><span class="o">.</span><span class="n">sum</span><span class="p">()))</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;QUANTIDADE DE SOBREVIVENTES&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Classe&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>


<div class="output_subarea output_text output_error">
<pre>
<span class="ansi-red-fg">---------------------------------------------------------------------------</span>
<span class="ansi-red-fg">NameError</span>                                 Traceback (most recent call last)
<span class="ansi-green-fg">&lt;ipython-input-23-8085cedfb3c1&gt;</span> in <span class="ansi-cyan-fg">&lt;module&gt;</span><span class="ansi-blue-fg">()</span>
<span class="ansi-green-intense-fg ansi-bold">      1</span> <span class="ansi-red-fg">#filtrando o dataset para conter dados apenas de pessoas que sobreviveram</span>
<span class="ansi-green-intense-fg ansi-bold">      2</span> classe_sobrevivente <span class="ansi-blue-fg">=</span> df<span class="ansi-blue-fg">[</span>df<span class="ansi-blue-fg">[</span><span class="ansi-blue-fg">&#39;Sobreviveu&#39;</span><span class="ansi-blue-fg">]</span> <span class="ansi-blue-fg">==</span> <span class="ansi-blue-fg">&#39;Sim&#39;</span><span class="ansi-blue-fg">]</span><span class="ansi-blue-fg">[</span><span class="ansi-blue-fg">&#39;Classe&#39;</span><span class="ansi-blue-fg">]</span><span class="ansi-blue-fg">.</span>value_counts<span class="ansi-blue-fg">(</span><span class="ansi-blue-fg">)</span><span class="ansi-blue-fg">.</span>sort_values<span class="ansi-blue-fg">(</span>ascending<span class="ansi-blue-fg">=</span><span class="ansi-green-fg">True</span><span class="ansi-blue-fg">)</span>
<span class="ansi-green-fg">----&gt; 3</span><span class="ansi-red-fg"> </span>classe_sobrevivente<span class="ansi-blue-fg">.</span>plot<span class="ansi-blue-fg">(</span>kind<span class="ansi-blue-fg">=</span><span class="ansi-blue-fg">&#39;barh&#39;</span><span class="ansi-blue-fg">,</span> figsize<span class="ansi-blue-fg">=</span><span class="ansi-blue-fg">(</span><span class="ansi-cyan-fg">11</span><span class="ansi-blue-fg">,</span><span class="ansi-cyan-fg">5</span><span class="ansi-blue-fg">)</span><span class="ansi-blue-fg">,</span> color<span class="ansi-blue-fg">=</span>random<span class="ansi-blue-fg">.</span>choice<span class="ansi-blue-fg">(</span>cores<span class="ansi-blue-fg">)</span><span class="ansi-blue-fg">,</span> rot<span class="ansi-blue-fg">=</span><span class="ansi-cyan-fg">0</span><span class="ansi-blue-fg">,</span> grid<span class="ansi-blue-fg">=</span><span class="ansi-green-fg">True</span><span class="ansi-blue-fg">)</span>
<span class="ansi-green-intense-fg ansi-bold">      4</span> 
<span class="ansi-green-intense-fg ansi-bold">      5</span> plt<span class="ansi-blue-fg">.</span>title<span class="ansi-blue-fg">(</span><span class="ansi-blue-fg">&#39;QUANTIDADE DE SOBREVIVENTES POR CLASSE\n Total: %s sobreviventes&#39;</span> <span class="ansi-blue-fg">%</span> <span class="ansi-blue-fg">(</span>classe_sobrevivente<span class="ansi-blue-fg">.</span>sum<span class="ansi-blue-fg">(</span><span class="ansi-blue-fg">)</span><span class="ansi-blue-fg">)</span><span class="ansi-blue-fg">)</span>

<span class="ansi-red-fg">NameError</span>: name &#39;cores&#39; is not defined</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[23]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#quantidade de passageiros (sobreviventes ou não) por classe</span>
<span class="n">df</span><span class="p">[</span><span class="s1">&#39;Classe&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">value_counts</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[23]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>3    491
1    216
2    184
Name: Classe, dtype: int64</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h3>Verificando a faixa etária das pessoas do návio.</h3>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[24]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">idades</span> <span class="o">=</span> <span class="n">df</span><span class="p">[</span><span class="n">df</span><span class="p">[</span><span class="s1">&#39;Idade&#39;</span><span class="p">]</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">][</span><span class="s1">&#39;Idade&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">astype</span><span class="p">(</span><span class="nb">int</span><span class="p">)</span><span class="o">.</span><span class="n">hist</span><span class="p">(</span><span class="n">bins</span><span class="o">=</span><span class="mi">10</span><span class="p">,</span> <span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">15</span><span class="p">,</span><span class="mi">5</span><span class="p">),</span> <span class="n">color</span><span class="o">=</span><span class="s1">&#39;red&#39;</span><span class="p">,</span> <span class="n">alpha</span><span class="o">=.</span><span class="mi">7</span><span class="p">)</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAA3EAAAEyCAYAAABUJ1mnAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAADl0RVh0U29mdHdhcmUAbWF0cGxvdGxpYiB2ZXJzaW9uIDIuMi4yLCBodHRwOi8vbWF0cGxvdGxpYi5vcmcvhp/UCwAAGVtJREFUeJzt3X+wpXddH/D3p1mhmut0wdAlJbQLkxQHMhrNHYqj0rugNlLXqx0HyVgLil2dwVbbOBZtp1gdZmzriu1osRFScNQslB9ulqFWhnJFZ4qyKykGkLpgkKSYGMiCFx0U+PSPewLX5Sa57D1nn/vd83rNnLnn+T7P/Z7PfubMc/Z9nx+nujsAAACM4a9NXQAAAAC7J8QBAAAMRIgDAAAYiBAHAAAwECEOAABgIEIcAADAQIQ4AACAgQhxAAAAAxHiAAAABnJg6gKS5IorrujDhw9PXcbn+PjHP57LL7986jKWkt5PS/+no/fT0fvp6P109H46ej+d/dr7M2fO3Nfdj9nNtvsixB0+fDinT5+euozPsbGxkbW1tanLWEp6Py39n47eT0fvp6P309H76ej9dPZr76vqA7vd1umUAAAAAxHiAAAABiLEAQAADESIAwAAGIgQBwAAMBAhDgAAYCBCHAAAwECEOAAAgIEIcQAAAAMR4gAAAAYixAEAAAzkwNQFAOza0aNTV7B46+vJ8ePzmevUqfnMAwDsK47EAQAADESIAwAAGIgQBwAAMBAhDgAAYCAPG+Kq6paqureq7tg29qqqun32uLOqbp+NH66qP9+27ucXWTwAAMCy2c3dKV+R5GeT/OIDA9397Q88r6rjST66bfv3dfd18yoQAACAz3rYENfdb62qwzutq6pK8uwkz5hvWQAAAOxkr9fEfW2Se7r7D7aNPaGq3lFVv1FVX7vH+QEAANimuvvhN9o6EveG7r72vPGXJjnb3cdny49MstLdH66q65P8apKndPfHdpjzWJJjSXLo0KHrT5w4scd/yvxtbm5mZWVl6jKWkt5Pa9/2/+zZqStYuM2DB7Ny7tx8Jrv66vnMsyT27ft+Cej9dPR+Ono/nf3a+yNHjpzp7tXdbHvBIa6qDiS5O8n13X3Xg/zeRpIf6u7TDzX/6upqnz79kJtMYmNjI2tra1OXsZT0flr7tv9Hj05dwcJtrK9n7eTJ+Ux26tR85lkS+/Z9vwT0fjp6Px29n85+7X1V7TrE7eV0yq9L8vvbA1xVPaaqLps9f2KSa5K8fw+vAQAAwDa7+YqBW5P87yRPqqq7qur5s1XPSXLreZs/Pck7Z1858Jok39fdH5lnwQAAAMtsN3envPFBxp+3w9hrk7x272UBAACwk73enRIAAICLSIgDAAAYiBAHAAAwECEOAABgIEIcAADAQIQ4AACAgQhxAAAAAxHiAAAABiLEAQAADESIAwAAGMiBqQuApXb06NQV7Gx9PTl+fOoqAADYgSNxAAAAAxHiAAAABiLEAQAADESIAwAAGIgQBwAAMBAhDgAAYCBCHAAAwECEOAAAgIEIcQAAAAMR4gAAAAYixAEAAAxEiAMAABiIEAcAADAQIQ4AAGAgQhwAAMBAhDgAAICBPGyIq6pbqureqrpj29iPVdXdVXX77PGsbet+pKrOVtV7q+ofLKpwAACAZbSbI3GvSHLDDuMv6e7rZo83JklVPTnJc5I8ZfY7/6WqLptXsQAAAMvuYUNcd781yUd2Od96khPd/Ynu/sMkZ5M8dQ/1AQAAsE1198NvVHU4yRu6+9rZ8o8leV6SjyU5neSm7r6/qn42ydu6+5dm2708yf/o7tfsMOexJMeS5NChQ9efOHFiDv+c+drc3MzKysrUZSylpen92bNTV7CjzYMHs3Lu3NRlLKW59v7qq+czz5JYmv3OPqT309H76ej9dPZr748cOXKmu1d3s+2BC3yNlyb5iSQ9+3k8yXd/PhN0981Jbk6S1dXVXltbu8BSFmdjYyP7sa5lsDS9P3586gp2tLG+nrWTJ6cuYynNtfenTs1nniWxNPudfUjvp6P309H76VwKvb+gu1N29z3d/anu/nSSX8hnT5m8O8njt2161WwMAACAObigEFdVV25b/NYkD9y58rYkz6mqR1bVE5Jck+R39lYiAAAAD3jY0ymr6tYka0muqKq7krwoyVpVXZet0ynvTPK9SdLd76qqVyd5d5JPJnlBd39qMaUDAAAsn4cNcd194w7DL3+I7V+c5MV7KQoAAICdXdDplAAAAExDiAMAABiIEAcAADAQIQ4AAGAgQhwAAMBAhDgAAICBCHEAAAADEeIAAAAGIsQBAAAMRIgDAAAYiBAHAAAwECEOAABgIEIcAADAQIQ4AACAgQhxAAAAAxHiAAAABiLEAQAADESIAwAAGIgQBwAAMBAhDgAAYCBCHAAAwECEOAAAgIEIcQAAAAMR4gAAAAYixAEAAAxEiAMAABiIEAcAADCQhw1xVXVLVd1bVXdsG/uPVfX7VfXOqnp9VR2cjR+uqj+vqttnj59fZPEAAADLZjdH4l6R5Ibzxt6U5Nru/rIk/zfJj2xb977uvm72+L75lAkAAECyixDX3W9N8pHzxn69uz85W3xbkqsWUBsAAADnqe5++I2qDid5Q3dfu8O6U0le1d2/NNvuXdk6OvexJP+mu3/zQeY8luRYkhw6dOj6EydOXNi/YIE2NzezsrIydRlLaWl6f/bs1BXsaPPgwaycOzd1GUtprr2/+ur5zLMklma/sw/p/XT0fjp6P5392vsjR46c6e7V3Wy7pxBXVf86yWqSf9TdXVWPTLLS3R+uquuT/GqSp3T3xx5q/tXV1T59+vRu6r2oNjY2sra2NnUZS2lpen/06NQV7GhjfT1rJ09OXcZSmmvvT52azzxLYmn2O/uQ3k9H76ej99PZr72vql2HuAu+O2VVPS/JNyX5jp4lwe7+RHd/ePb8TJL3Jfm7F/oaAAAA/FUHLuSXquqGJD+c5O93959tG39Mko9096eq6olJrkny/rlUCsDnZ58e6d23brpp6goAYFceNsRV1a1J1pJcUVV3JXlRtu5G+cgkb6qqJHnb7E6UT0/y41X1l0k+neT7uvsjO04MAADA5+1hQ1x337jD8MsfZNvXJnntXosCAABgZxd8TRwAAAAXnxAHAAAwECEOAABgIEIcAADAQIQ4AACAgQhxAAAAAxHiAAAABiLEAQAADESIAwAAGIgQBwAAMBAhDgAAYCBCHAAAwECEOAAAgIEIcQAAAAMR4gAAAAYixAEAAAxEiAMAABiIEAcAADAQIQ4AAGAgQhwAAMBAhDgAAICBCHEAAAADEeIAAAAGIsQBAAAMRIgDAAAYiBAHAAAwkF2FuKq6parurao7to09uqreVFV/MPv5qNl4VdV/rqqzVfXOqvrKRRUPAACwbHZ7JO4VSW44b+yFSd7c3dckefNsOUm+Mck1s8exJC/de5kAAAAkuwxx3f3WJB85b3g9yStnz1+Z5Fu2jf9ib3lbkoNVdeU8igUAAFh2e7km7lB3f2j2/I+THJo9f1ySD27b7q7ZGAAAAHtU3b27DasOJ3lDd187Wz7X3Qe3rb+/ux9VVW9I8pPd/Vuz8Tcn+Vfdffq8+Y5l63TLHDp06PoTJ07M4Z8zX5ubm1lZWZm6jKW0NL0/e3bqCna0efBgVs6dm7qMpaT309l87GOXY7+zDy3NPn8f0vvp6P109mvvjxw5cqa7V3ez7YE9vM49VXVld39odrrkvbPxu5M8ftt2V83G/oruvjnJzUmyurraa2treyhlMTY2NrIf61oGS9P748enrmBHG+vrWTt5cuoylpLeT2fjppuWY7+zDy3NPn8f0vvp6P10LoXe7+V0ytuSPHf2/LlJTm4b/yezu1Q+LclHt512CQAAwB7s6khcVd2aZC3JFVV1V5IXJfnJJK+uqucn+UCSZ882f2OSZyU5m+TPknzXnGsGAABYWrsKcd1944OseuYO23aSF+ylKAAAAHa2l9MpAQAAuMiEOAAAgIEIcQAAAAMR4gAAAAYixAEAAAxEiAMAABiIEAcAADAQIQ4AAGAgQhwAAMBAhDgAAICBCHEAAAADEeIAAAAGIsQBAAAMRIgDAAAYiBAHAAAwECEOAABgIEIcAADAQIQ4AACAgQhxAAAAAxHiAAAABiLEAQAADESIAwAAGIgQBwAAMBAhDgAAYCBCHAAAwECEOAAAgIEIcQAAAAM5cKG/WFVPSvKqbUNPTPJvkxxM8k+T/Mls/Ee7+40XXCEAAACfccEhrrvfm+S6JKmqy5LcneT1Sb4ryUu6+6fmUiEAAACfMa/TKZ+Z5H3d/YE5zQcAAMAO5hXinpPk1m3L319V76yqW6rqUXN6DQAAgKVX3b23CaoekeT/JXlKd99TVYeS3Jekk/xEkiu7+7t3+L1jSY4lyaFDh64/ceLEnupYhM3NzaysrExdxlJamt6fPTt1BTvaPHgwK+fOTV3GUtL76Ww+9rHLsd/Zh5Zmn78P6f109H46+7X3R44cOdPdq7vZdh4hbj3JC7r7G3ZYdzjJG7r72oeaY3V1tU+fPr2nOhZhY2Mja2trU5exlJam90ePTl3BjjbW17N28uTUZSwlvZ+O3n+eTp2a21RLs8/fh/R+Ono/nf3a+6radYibx+mUN2bbqZRVdeW2dd+a5I45vAYAAADZw90pk6SqLk/y9Um+d9vwf6iq67J1OuWd560DAABgD/YU4rr740m+5Lyx79xTRQAAADyoed2dEgAAgItAiAMAABiIEAcAADAQIQ4AAGAgQhwAAMBAhDgAAICBCHEAAAADEeIAAAAGIsQBAAAMRIgDAAAYiBAHAAAwECEOAABgIEIcAADAQIQ4AACAgQhxAAAAAxHiAAAABiLEAQAADESIAwAAGIgQBwAAMBAhDgAAYCBCHAAAwECEOAAAgIEIcQAAAAMR4gAAAAYixAEAAAxEiAMAABiIEAcAADCQA3udoKruTPKnST6V5JPdvVpVj07yqiSHk9yZ5Nndff9eXwsAAGDZzetI3JHuvq67V2fLL0zy5u6+JsmbZ8sAAADs0aJOp1xP8srZ81cm+ZYFvQ4AAMBSqe7e2wRVf5jk/iSd5L92981Vda67D87WV5L7H1je9nvHkhxLkkOHDl1/4sSJPdWxCJv33ZeVc+emLmMcV189t6k2NzezsrIyt/n2rbNnp65gR5sHD3rvT0Tvp6P301mK3s/xM3Kelubzdh/S++ns194fOXLkzLYzGx/SPELc47r77qr6m0nelOSfJblte2irqvu7+1EPNsfq6mqfPn16T3UswsbLXpa1kyenLmMcp07NbaqNjY2sra3Nbb596+jRqSvY0cb6uvf+RPR+Ono/naXo/Rw/I+dpaT5v9yG9n85+7X1V7TrE7fl0yu6+e/bz3iSvT/LUJPdU1ZWzYq5Mcu9eXwcAAIA9hriquryqvviB50m+IckdSW5L8tzZZs9Ncon/eQ0AAODi2OtXDBxK8vqty95yIMmvdPevVdXbk7y6qp6f5ANJnr3H1wEAACB7DHHd/f4kX77D+IeTPHMvcwMAAPC5FvUVAwAAACyAEAcAADAQIQ4AAGAgQhwAAMBAhDgAAICBCHEAAAADEeIAAAAGIsQBAAAMRIgDAAAYiBAHAAAwECEOAABgIEIcAADAQIQ4AACAgQhxAAAAAxHiAAAABiLEAQAADESIAwAAGIgQBwAAMBAhDgAAYCAHpi6AS8jRo/Oba309OX58fvMBAMAlwpE4AACAgQhxAAAAAxHiAAAABiLEAQAADESIAwAAGIgQBwAAMBAhDgAAYCAXHOKq6vFV9ZaqendVvauqfmA2/mNVdXdV3T57PGt+5QIAACy3vXzZ9yeT3NTdv1tVX5zkTFW9abbuJd39U3svDwAAgO0uOMR194eSfGj2/E+r6j1JHjevwgAALhlHj05dwc7W15Pjx6eu4nOdOjV1BbCvVXfvfZKqw0nemuTaJP8yyfOSfCzJ6Wwdrbt/h985luRYkhw6dOj6EydO7LmOedu8776snDs3dRlLafPgQb2fkP5PR++no/fT0fvp7NveX3311BUs3ObmZlZWVqYuYynt194fOXLkTHev7mbbPYe4qlpJ8htJXtzdr6uqQ0nuS9JJfiLJld393Q81x+rqap8+fXpPdSzCxstelrWTJ6cuYyltrK/r/YT0fzp6Px29n47eT2ff9n4JjsRtbGxkbW1t6jKW0n7tfVXtOsTt6e6UVfUFSV6b5Je7+3VJ0t33dPenuvvTSX4hyVP38hoAAAB81l7uTllJXp7kPd3909vGr9y22bcmuePCywMAAGC7vdyd8quTfGeS36uq22djP5rkxqq6LlunU96Z5Hv3VCEAAACfsZe7U/5Wktph1RsvvBwAAAAeyp6uiQMAAODiEuIAAAAGIsQBAAAMRIgDAAAYiBAHAAAwECEOAABgIEIcAADAQIQ4AACAgQhxAAAAAxHiAAAABiLEAQAADESIAwAAGIgQBwAAMBAhDgAAYCAHpi4AAAD+iqNHp65g8dbXk+PH5zPXqVPzmYdhOBIHAAAwECEOAABgIEIcAADAQIQ4AACAgQhxAAAAAxHiAAAABiLEAQAADESIAwAAGIgQBwAAMBAhDgAAYCBCHAAAwEAWFuKq6oaqem9Vna2qFy7qdQAAAJbJgUVMWlWXJfm5JF+f5K4kb6+q27r73Yt4PQAAWFpHj05dwVhuumnqCvZsUUfinprkbHe/v7v/IsmJJOsLei0AAIClsagQ97gkH9y2fNdsDAAAgD2o7p7/pFXfluSG7v6e2fJ3Jvl73f3927Y5luTYbPFJSd4790L27ook901dxJLS+2np/3T0fjp6Px29n47eT0fvp7Nfe/93uvsxu9lwIdfEJbk7yeO3LV81G/uM7r45yc0Lev25qKrT3b06dR3LSO+npf/T0fvp6P109H46ej8dvZ/OpdD7RZ1O+fYk11TVE6rqEUmek+S2Bb0WAADA0ljIkbju/mRVfX+S/5nksiS3dPe7FvFaAAAAy2RRp1Omu9+Y5I2Lmv8i2dene17i9H5a+j8dvZ+O3k9H76ej99PR++kM3/uF3NgEAACAxVjUNXEAAAAsgBAHAAAwECHuQVTVDVX13qo6W1UvnLqeS1lV3VJV91bVHdvGHl1Vb6qqP5j9fNSUNV6qqurxVfWWqnp3Vb2rqn5gNq7/C1ZVf72qfqeq/s+s9/9uNv6Eqvrt2b7nVbM7/LIAVXVZVb2jqt4wW9b7i6Cq7qyq36uq26vq9GzMPuciqKqDVfWaqvr9qnpPVX2V3l8cVfWk2Xv+gcfHquoH9f/iqKp/MfusvaOqbp19Bg+9zxfidlBVlyX5uSTfmOTJSW6sqidPW9Ul7RVJbjhv7IVJ3tzd1yR582yZ+ftkkpu6+8lJnpbkBbP3uv4v3ieSPKO7vzzJdUluqKqnJfn3SV7S3VcnuT/J8yes8VL3A0nes21Z7y+eI9193bbvabLPuTj+U5Jf6+4vTfLl2Xr/6/1F0N3vnb3nr0tyfZI/S/L66P/CVdXjkvzzJKvdfW227pz/nAy+zxfidvbUJGe7+/3d/RdJTiRZn7imS1Z3vzXJR84bXk/yytnzVyb5lota1JLo7g919+/Onv9ptj7QHxf9X7jesjlb/ILZo5M8I8lrZuN6vyBVdVWSf5jkZbPlit5PyT5nwarqbyR5epKXJ0l3/0V3n4veT+GZSd7X3R+I/l8sB5J8YVUdSPJFST6Uwff5QtzOHpfkg9uW75qNcfEc6u4PzZ7/cZJDUxazDKrqcJKvSPLb0f+LYnY63+1J7k3ypiTvS3Kuuz8528S+Z3F+JskPJ/n0bPlLovcXSyf59ao6U1XHZmP2OYv3hCR/kuS/zU4jfllVXR69n8Jzktw6e67/C9bddyf5qSR/lK3w9tEkZzL4Pl+IY9/rre/B8F0YC1RVK0lem+QHu/tj29fp/+J096dmp9Zcla0zAL504pKWQlV9U5J7u/vM1LUsqa/p7q/M1iULL6iqp29faZ+zMAeSfGWSl3b3VyT5eM47dU/vF2923dU3J/nv56/T/8WYXWe4nq0/ZPytJJfncy/jGY4Qt7O7kzx+2/JVszEunnuq6sokmf28d+J6LllV9QXZCnC/3N2vmw3r/0U0O6XpLUm+KsnB2ekeiX3Ponx1km+uqjuzdbr8M7J1rZDeXwSzv4qnu+/N1jVBT419zsVwV5K7uvu3Z8uvyVao0/uL6xuT/G533zNb1v/F+7okf9jdf9Ldf5nkddn6HBh6ny/E7eztSa6Z3bXmEdk67H3bxDUtm9uSPHf2/LlJTk5YyyVrdh3Qy5O8p7t/etsq/V+wqnpMVR2cPf/CJF+frWsS35Lk22ab6f0CdPePdPdV3X04W/v3/9Xd3xG9X7iquryqvviB50m+Ickdsc9ZuO7+4yQfrKonzYaemeTd0fuL7cZ89lTKRP8vhj9K8rSq+qLZ/3seeO8Pvc+vrSO3nK+qnpWtayYuS3JLd7944pIuWVV1a5K1JFckuSfJi5L8apJXJ/nbST6Q5Nndff7NT9ijqvqaJL+Z5Pfy2WuDfjRb18Xp/wJV1Zdl60Lqy7L1B7VXd/ePV9UTs3V06NFJ3pHkH3f3J6ar9NJWVWtJfqi7v0nvF2/W49fPFg8k+ZXufnFVfUnscxauqq7L1s18HpHk/Um+K7P9T/R+4WZ/uPijJE/s7o/Oxrz3L4LZ1/h8e7buyv2OJN+TrWvght3nC3EAAAADcTolAADAQIQ4AACAgQhxAAAAAxHiAAAABiLEAQAADESIAwAAGIgQBwAAMJD/D7EoctkrXrqwAAAAAElFTkSuQmCC
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div>
<div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<p><h3> Contando as pessoas que não pagaram o ticket de entrada no návio.<h3></p>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[25]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#tarifaZero = df[df[&#39;Tarifa&#39;] == 0]</span>
<span class="n">df</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

</div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

<div class="prompt output_prompt">Out[25]:</div>



<div class="output_html rendered_html output_subarea output_execute_result">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Sobreviveu</th>
      <th>Classe</th>
      <th>Nome</th>
      <th>Sexo</th>
      <th>Idade</th>
      <th>Irmãos/Cônjuge</th>
      <th>Pais/Crianças</th>
      <th>Tarifa</th>
      <th>Embarque</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Não</td>
      <td>3</td>
      <td>Braund, Mr. Owen Harris</td>
      <td>Masculino</td>
      <td>22.0</td>
      <td>1</td>
      <td>0</td>
      <td>7.2500</td>
      <td>Southampton</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Sim</td>
      <td>1</td>
      <td>Cumings, Mrs. John Bradley (Florence Briggs Th...</td>
      <td>Feminino</td>
      <td>38.0</td>
      <td>1</td>
      <td>0</td>
      <td>71.2833</td>
      <td>Cherbourg</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Sim</td>
      <td>3</td>
      <td>Heikkinen, Miss. Laina</td>
      <td>Feminino</td>
      <td>26.0</td>
      <td>0</td>
      <td>0</td>
      <td>7.9250</td>
      <td>Southampton</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Sim</td>
      <td>1</td>
      <td>Futrelle, Mrs. Jacques Heath (Lily May Peel)</td>
      <td>Feminino</td>
      <td>35.0</td>
      <td>1</td>
      <td>0</td>
      <td>53.1000</td>
      <td>Southampton</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Não</td>
      <td>3</td>
      <td>Allen, Mr. William Henry</td>
      <td>Masculino</td>
      <td>35.0</td>
      <td>0</td>
      <td>0</td>
      <td>8.0500</td>
      <td>Southampton</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>
</div>

</div>
    </div>
  </div>
</body>

 


</html>

