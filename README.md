[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/molp11/library_selection_demo/master)
# library_selection_demo

<!DOCTYPE html>
<html>
<head><meta charset="utf-8" />

<title>main</title>

<script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
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
 *  Font Awesome 4.7.0 by @davegandy - http://fontawesome.io - @fontawesome
 *  License - http://fontawesome.io/license (Font: SIL OFL 1.1, CSS: MIT License)
 */
/* FONT PATH
 * -------------------------- */
@font-face {
  font-family: 'FontAwesome';
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?v=4.7.0');
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?#iefix&v=4.7.0') format('embedded-opentype'), url('../components/font-awesome/fonts/fontawesome-webfont.woff2?v=4.7.0') format('woff2'), url('../components/font-awesome/fonts/fontawesome-webfont.woff?v=4.7.0') format('woff'), url('../components/font-awesome/fonts/fontawesome-webfont.ttf?v=4.7.0') format('truetype'), url('../components/font-awesome/fonts/fontawesome-webfont.svg?v=4.7.0#fontawesomeregular') format('svg');
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
.fa-pull-left {
  float: left;
}
.fa-pull-right {
  float: right;
}
.fa.fa-pull-left {
  margin-right: .3em;
}
.fa.fa-pull-right {
  margin-left: .3em;
}
/* Deprecated as of 4.4.0 */
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
.fa-pulse {
  -webkit-animation: fa-spin 1s infinite steps(8);
  animation: fa-spin 1s infinite steps(8);
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
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=1)";
  -webkit-transform: rotate(90deg);
  -ms-transform: rotate(90deg);
  transform: rotate(90deg);
}
.fa-rotate-180 {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=2)";
  -webkit-transform: rotate(180deg);
  -ms-transform: rotate(180deg);
  transform: rotate(180deg);
}
.fa-rotate-270 {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=3)";
  -webkit-transform: rotate(270deg);
  -ms-transform: rotate(270deg);
  transform: rotate(270deg);
}
.fa-flip-horizontal {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=0, mirror=1)";
  -webkit-transform: scale(-1, 1);
  -ms-transform: scale(-1, 1);
  transform: scale(-1, 1);
}
.fa-flip-vertical {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=2, mirror=1)";
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
.fa-facebook-f:before,
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
.fa-feed:before,
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
.fa-gittip:before,
.fa-gratipay:before {
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
.fa-pied-piper-pp:before {
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
.fa-resistance:before,
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
.fa-y-combinator-square:before,
.fa-yc-square:before,
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
.fa-buysellads:before {
  content: "\f20d";
}
.fa-connectdevelop:before {
  content: "\f20e";
}
.fa-dashcube:before {
  content: "\f210";
}
.fa-forumbee:before {
  content: "\f211";
}
.fa-leanpub:before {
  content: "\f212";
}
.fa-sellsy:before {
  content: "\f213";
}
.fa-shirtsinbulk:before {
  content: "\f214";
}
.fa-simplybuilt:before {
  content: "\f215";
}
.fa-skyatlas:before {
  content: "\f216";
}
.fa-cart-plus:before {
  content: "\f217";
}
.fa-cart-arrow-down:before {
  content: "\f218";
}
.fa-diamond:before {
  content: "\f219";
}
.fa-ship:before {
  content: "\f21a";
}
.fa-user-secret:before {
  content: "\f21b";
}
.fa-motorcycle:before {
  content: "\f21c";
}
.fa-street-view:before {
  content: "\f21d";
}
.fa-heartbeat:before {
  content: "\f21e";
}
.fa-venus:before {
  content: "\f221";
}
.fa-mars:before {
  content: "\f222";
}
.fa-mercury:before {
  content: "\f223";
}
.fa-intersex:before,
.fa-transgender:before {
  content: "\f224";
}
.fa-transgender-alt:before {
  content: "\f225";
}
.fa-venus-double:before {
  content: "\f226";
}
.fa-mars-double:before {
  content: "\f227";
}
.fa-venus-mars:before {
  content: "\f228";
}
.fa-mars-stroke:before {
  content: "\f229";
}
.fa-mars-stroke-v:before {
  content: "\f22a";
}
.fa-mars-stroke-h:before {
  content: "\f22b";
}
.fa-neuter:before {
  content: "\f22c";
}
.fa-genderless:before {
  content: "\f22d";
}
.fa-facebook-official:before {
  content: "\f230";
}
.fa-pinterest-p:before {
  content: "\f231";
}
.fa-whatsapp:before {
  content: "\f232";
}
.fa-server:before {
  content: "\f233";
}
.fa-user-plus:before {
  content: "\f234";
}
.fa-user-times:before {
  content: "\f235";
}
.fa-hotel:before,
.fa-bed:before {
  content: "\f236";
}
.fa-viacoin:before {
  content: "\f237";
}
.fa-train:before {
  content: "\f238";
}
.fa-subway:before {
  content: "\f239";
}
.fa-medium:before {
  content: "\f23a";
}
.fa-yc:before,
.fa-y-combinator:before {
  content: "\f23b";
}
.fa-optin-monster:before {
  content: "\f23c";
}
.fa-opencart:before {
  content: "\f23d";
}
.fa-expeditedssl:before {
  content: "\f23e";
}
.fa-battery-4:before,
.fa-battery:before,
.fa-battery-full:before {
  content: "\f240";
}
.fa-battery-3:before,
.fa-battery-three-quarters:before {
  content: "\f241";
}
.fa-battery-2:before,
.fa-battery-half:before {
  content: "\f242";
}
.fa-battery-1:before,
.fa-battery-quarter:before {
  content: "\f243";
}
.fa-battery-0:before,
.fa-battery-empty:before {
  content: "\f244";
}
.fa-mouse-pointer:before {
  content: "\f245";
}
.fa-i-cursor:before {
  content: "\f246";
}
.fa-object-group:before {
  content: "\f247";
}
.fa-object-ungroup:before {
  content: "\f248";
}
.fa-sticky-note:before {
  content: "\f249";
}
.fa-sticky-note-o:before {
  content: "\f24a";
}
.fa-cc-jcb:before {
  content: "\f24b";
}
.fa-cc-diners-club:before {
  content: "\f24c";
}
.fa-clone:before {
  content: "\f24d";
}
.fa-balance-scale:before {
  content: "\f24e";
}
.fa-hourglass-o:before {
  content: "\f250";
}
.fa-hourglass-1:before,
.fa-hourglass-start:before {
  content: "\f251";
}
.fa-hourglass-2:before,
.fa-hourglass-half:before {
  content: "\f252";
}
.fa-hourglass-3:before,
.fa-hourglass-end:before {
  content: "\f253";
}
.fa-hourglass:before {
  content: "\f254";
}
.fa-hand-grab-o:before,
.fa-hand-rock-o:before {
  content: "\f255";
}
.fa-hand-stop-o:before,
.fa-hand-paper-o:before {
  content: "\f256";
}
.fa-hand-scissors-o:before {
  content: "\f257";
}
.fa-hand-lizard-o:before {
  content: "\f258";
}
.fa-hand-spock-o:before {
  content: "\f259";
}
.fa-hand-pointer-o:before {
  content: "\f25a";
}
.fa-hand-peace-o:before {
  content: "\f25b";
}
.fa-trademark:before {
  content: "\f25c";
}
.fa-registered:before {
  content: "\f25d";
}
.fa-creative-commons:before {
  content: "\f25e";
}
.fa-gg:before {
  content: "\f260";
}
.fa-gg-circle:before {
  content: "\f261";
}
.fa-tripadvisor:before {
  content: "\f262";
}
.fa-odnoklassniki:before {
  content: "\f263";
}
.fa-odnoklassniki-square:before {
  content: "\f264";
}
.fa-get-pocket:before {
  content: "\f265";
}
.fa-wikipedia-w:before {
  content: "\f266";
}
.fa-safari:before {
  content: "\f267";
}
.fa-chrome:before {
  content: "\f268";
}
.fa-firefox:before {
  content: "\f269";
}
.fa-opera:before {
  content: "\f26a";
}
.fa-internet-explorer:before {
  content: "\f26b";
}
.fa-tv:before,
.fa-television:before {
  content: "\f26c";
}
.fa-contao:before {
  content: "\f26d";
}
.fa-500px:before {
  content: "\f26e";
}
.fa-amazon:before {
  content: "\f270";
}
.fa-calendar-plus-o:before {
  content: "\f271";
}
.fa-calendar-minus-o:before {
  content: "\f272";
}
.fa-calendar-times-o:before {
  content: "\f273";
}
.fa-calendar-check-o:before {
  content: "\f274";
}
.fa-industry:before {
  content: "\f275";
}
.fa-map-pin:before {
  content: "\f276";
}
.fa-map-signs:before {
  content: "\f277";
}
.fa-map-o:before {
  content: "\f278";
}
.fa-map:before {
  content: "\f279";
}
.fa-commenting:before {
  content: "\f27a";
}
.fa-commenting-o:before {
  content: "\f27b";
}
.fa-houzz:before {
  content: "\f27c";
}
.fa-vimeo:before {
  content: "\f27d";
}
.fa-black-tie:before {
  content: "\f27e";
}
.fa-fonticons:before {
  content: "\f280";
}
.fa-reddit-alien:before {
  content: "\f281";
}
.fa-edge:before {
  content: "\f282";
}
.fa-credit-card-alt:before {
  content: "\f283";
}
.fa-codiepie:before {
  content: "\f284";
}
.fa-modx:before {
  content: "\f285";
}
.fa-fort-awesome:before {
  content: "\f286";
}
.fa-usb:before {
  content: "\f287";
}
.fa-product-hunt:before {
  content: "\f288";
}
.fa-mixcloud:before {
  content: "\f289";
}
.fa-scribd:before {
  content: "\f28a";
}
.fa-pause-circle:before {
  content: "\f28b";
}
.fa-pause-circle-o:before {
  content: "\f28c";
}
.fa-stop-circle:before {
  content: "\f28d";
}
.fa-stop-circle-o:before {
  content: "\f28e";
}
.fa-shopping-bag:before {
  content: "\f290";
}
.fa-shopping-basket:before {
  content: "\f291";
}
.fa-hashtag:before {
  content: "\f292";
}
.fa-bluetooth:before {
  content: "\f293";
}
.fa-bluetooth-b:before {
  content: "\f294";
}
.fa-percent:before {
  content: "\f295";
}
.fa-gitlab:before {
  content: "\f296";
}
.fa-wpbeginner:before {
  content: "\f297";
}
.fa-wpforms:before {
  content: "\f298";
}
.fa-envira:before {
  content: "\f299";
}
.fa-universal-access:before {
  content: "\f29a";
}
.fa-wheelchair-alt:before {
  content: "\f29b";
}
.fa-question-circle-o:before {
  content: "\f29c";
}
.fa-blind:before {
  content: "\f29d";
}
.fa-audio-description:before {
  content: "\f29e";
}
.fa-volume-control-phone:before {
  content: "\f2a0";
}
.fa-braille:before {
  content: "\f2a1";
}
.fa-assistive-listening-systems:before {
  content: "\f2a2";
}
.fa-asl-interpreting:before,
.fa-american-sign-language-interpreting:before {
  content: "\f2a3";
}
.fa-deafness:before,
.fa-hard-of-hearing:before,
.fa-deaf:before {
  content: "\f2a4";
}
.fa-glide:before {
  content: "\f2a5";
}
.fa-glide-g:before {
  content: "\f2a6";
}
.fa-signing:before,
.fa-sign-language:before {
  content: "\f2a7";
}
.fa-low-vision:before {
  content: "\f2a8";
}
.fa-viadeo:before {
  content: "\f2a9";
}
.fa-viadeo-square:before {
  content: "\f2aa";
}
.fa-snapchat:before {
  content: "\f2ab";
}
.fa-snapchat-ghost:before {
  content: "\f2ac";
}
.fa-snapchat-square:before {
  content: "\f2ad";
}
.fa-pied-piper:before {
  content: "\f2ae";
}
.fa-first-order:before {
  content: "\f2b0";
}
.fa-yoast:before {
  content: "\f2b1";
}
.fa-themeisle:before {
  content: "\f2b2";
}
.fa-google-plus-circle:before,
.fa-google-plus-official:before {
  content: "\f2b3";
}
.fa-fa:before,
.fa-font-awesome:before {
  content: "\f2b4";
}
.fa-handshake-o:before {
  content: "\f2b5";
}
.fa-envelope-open:before {
  content: "\f2b6";
}
.fa-envelope-open-o:before {
  content: "\f2b7";
}
.fa-linode:before {
  content: "\f2b8";
}
.fa-address-book:before {
  content: "\f2b9";
}
.fa-address-book-o:before {
  content: "\f2ba";
}
.fa-vcard:before,
.fa-address-card:before {
  content: "\f2bb";
}
.fa-vcard-o:before,
.fa-address-card-o:before {
  content: "\f2bc";
}
.fa-user-circle:before {
  content: "\f2bd";
}
.fa-user-circle-o:before {
  content: "\f2be";
}
.fa-user-o:before {
  content: "\f2c0";
}
.fa-id-badge:before {
  content: "\f2c1";
}
.fa-drivers-license:before,
.fa-id-card:before {
  content: "\f2c2";
}
.fa-drivers-license-o:before,
.fa-id-card-o:before {
  content: "\f2c3";
}
.fa-quora:before {
  content: "\f2c4";
}
.fa-free-code-camp:before {
  content: "\f2c5";
}
.fa-telegram:before {
  content: "\f2c6";
}
.fa-thermometer-4:before,
.fa-thermometer:before,
.fa-thermometer-full:before {
  content: "\f2c7";
}
.fa-thermometer-3:before,
.fa-thermometer-three-quarters:before {
  content: "\f2c8";
}
.fa-thermometer-2:before,
.fa-thermometer-half:before {
  content: "\f2c9";
}
.fa-thermometer-1:before,
.fa-thermometer-quarter:before {
  content: "\f2ca";
}
.fa-thermometer-0:before,
.fa-thermometer-empty:before {
  content: "\f2cb";
}
.fa-shower:before {
  content: "\f2cc";
}
.fa-bathtub:before,
.fa-s15:before,
.fa-bath:before {
  content: "\f2cd";
}
.fa-podcast:before {
  content: "\f2ce";
}
.fa-window-maximize:before {
  content: "\f2d0";
}
.fa-window-minimize:before {
  content: "\f2d1";
}
.fa-window-restore:before {
  content: "\f2d2";
}
.fa-times-rectangle:before,
.fa-window-close:before {
  content: "\f2d3";
}
.fa-times-rectangle-o:before,
.fa-window-close-o:before {
  content: "\f2d4";
}
.fa-bandcamp:before {
  content: "\f2d5";
}
.fa-grav:before {
  content: "\f2d6";
}
.fa-etsy:before {
  content: "\f2d7";
}
.fa-imdb:before {
  content: "\f2d8";
}
.fa-ravelry:before {
  content: "\f2d9";
}
.fa-eercast:before {
  content: "\f2da";
}
.fa-microchip:before {
  content: "\f2db";
}
.fa-snowflake-o:before {
  content: "\f2dc";
}
.fa-superpowers:before {
  content: "\f2dd";
}
.fa-wpexplorer:before {
  content: "\f2de";
}
.fa-meetup:before {
  content: "\f2e0";
}
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
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
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
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
div.traceback-wrapper pre.traceback {
  max-height: 600px;
  overflow: auto;
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
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 5px;
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
[dir="rtl"] #ipython_notebook {
  margin-right: 10px;
  margin-left: 0;
}
[dir="rtl"] #ipython_notebook.pull-left {
  float: right !important;
  float: right;
}
.flex-spacer {
  flex: 1;
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
span#kernel_logo_widget {
  margin: 0 10px;
}
span#login_widget {
  float: right;
}
[dir="rtl"] span#login_widget {
  float: left;
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
.modal-header {
  cursor: move;
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
[dir="rtl"] .center-nav form.pull-left {
  float: right !important;
  float: right;
}
[dir="rtl"] .center-nav .navbar-text {
  float: right;
}
[dir="rtl"] .navbar-inner {
  text-align: right;
}
[dir="rtl"] div.text-left {
  text-align: right;
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
  position: absolute;
  display: block;
  width: 100%;
  height: 100%;
  overflow: hidden;
  cursor: pointer;
  opacity: 0;
  z-index: 2;
}
.alternate_upload .btn-xs > input.fileinput {
  margin: -1px -5px;
}
.alternate_upload .btn-upload {
  position: relative;
  height: 22px;
}
::-webkit-file-upload-button {
  cursor: pointer;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
ul#tabs {
  margin-bottom: 4px;
}
ul#tabs a {
  padding-top: 6px;
  padding-bottom: 4px;
}
[dir="rtl"] ul#tabs.nav-tabs > li {
  float: right;
}
[dir="rtl"] ul#tabs.nav.nav-tabs {
  padding-right: 0;
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
[dir="rtl"] .list_toolbar .tree-buttons .pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .list_toolbar .col-sm-4,
[dir="rtl"] .list_toolbar .col-sm-8 {
  float: right;
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
  vertical-align: text-bottom;
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
[dir="rtl"] .list_item > div input {
  margin-right: 0;
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
.item_modified {
  margin-right: 7px;
  margin-left: 7px;
}
[dir="rtl"] .item_modified.pull-right {
  float: left !important;
  float: left;
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
[dir="rtl"] .item_buttons.pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .item_buttons .kernel-name {
  margin-left: 7px;
  float: right;
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
.sort_button {
  display: inline-block;
  padding-left: 7px;
}
[dir="rtl"] .sort_button.pull-right {
  float: left !important;
  float: left;
}
#tree-selector {
  padding-right: 0px;
}
#button-select-all {
  min-width: 50px;
}
[dir="rtl"] #button-select-all.btn {
  float: right ;
}
#select-all {
  margin-left: 7px;
  margin-right: 2px;
  margin-top: 2px;
  height: 16px;
}
[dir="rtl"] #select-all.pull-left {
  float: right !important;
  float: right;
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
.folder_icon:before.fa-pull-left {
  margin-right: .3em;
}
.folder_icon:before.fa-pull-right {
  margin-left: .3em;
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
.notebook_icon:before.fa-pull-left {
  margin-right: .3em;
}
.notebook_icon:before.fa-pull-right {
  margin-left: .3em;
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
.running_notebook_icon:before.fa-pull-left {
  margin-right: .3em;
}
.running_notebook_icon:before.fa-pull-right {
  margin-left: .3em;
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
.file_icon:before.fa-pull-left {
  margin-right: .3em;
}
.file_icon:before.fa-pull-right {
  margin-left: .3em;
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
#new-menu .dropdown-header {
  font-size: 10px;
  border-bottom: 1px solid #e5e5e5;
  padding: 0 0 3px;
  margin: -3px 20px 0;
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
.delete-button {
  display: none;
}
.duplicate-button {
  display: none;
}
.rename-button {
  display: none;
}
.move-button {
  display: none;
}
.download-button {
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
.dirty-indicator.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator.fa-pull-right {
  margin-left: .3em;
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
.dirty-indicator-dirty.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator-dirty.fa-pull-right {
  margin-left: .3em;
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
.dirty-indicator-clean.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean.fa-pull-right {
  margin-left: .3em;
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
.dirty-indicator-clean:before.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean:before.fa-pull-right {
  margin-left: .3em;
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
.CodeMirror-dialog {
  background-color: #fff;
}
/*!
*
* IPython notebook
*
*/
/* CSS font colors for translated ANSI escape sequences */
/* The color values are a mix of
   http://www.xcolors.net/dl/baskerville-ivorylight and
   http://www.xcolors.net/dl/euphrasia */
.ansi-black-fg {
  color: #3E424D;
}
.ansi-black-bg {
  background-color: #3E424D;
}
.ansi-black-intense-fg {
  color: #282C36;
}
.ansi-black-intense-bg {
  background-color: #282C36;
}
.ansi-red-fg {
  color: #E75C58;
}
.ansi-red-bg {
  background-color: #E75C58;
}
.ansi-red-intense-fg {
  color: #B22B31;
}
.ansi-red-intense-bg {
  background-color: #B22B31;
}
.ansi-green-fg {
  color: #00A250;
}
.ansi-green-bg {
  background-color: #00A250;
}
.ansi-green-intense-fg {
  color: #007427;
}
.ansi-green-intense-bg {
  background-color: #007427;
}
.ansi-yellow-fg {
  color: #DDB62B;
}
.ansi-yellow-bg {
  background-color: #DDB62B;
}
.ansi-yellow-intense-fg {
  color: #B27D12;
}
.ansi-yellow-intense-bg {
  background-color: #B27D12;
}
.ansi-blue-fg {
  color: #208FFB;
}
.ansi-blue-bg {
  background-color: #208FFB;
}
.ansi-blue-intense-fg {
  color: #0065CA;
}
.ansi-blue-intense-bg {
  background-color: #0065CA;
}
.ansi-magenta-fg {
  color: #D160C4;
}
.ansi-magenta-bg {
  background-color: #D160C4;
}
.ansi-magenta-intense-fg {
  color: #A03196;
}
.ansi-magenta-intense-bg {
  background-color: #A03196;
}
.ansi-cyan-fg {
  color: #60C6C8;
}
.ansi-cyan-bg {
  background-color: #60C6C8;
}
.ansi-cyan-intense-fg {
  color: #258F8F;
}
.ansi-cyan-intense-bg {
  background-color: #258F8F;
}
.ansi-white-fg {
  color: #C5C1B4;
}
.ansi-white-bg {
  background-color: #C5C1B4;
}
.ansi-white-intense-fg {
  color: #A1A6B2;
}
.ansi-white-intense-bg {
  background-color: #A1A6B2;
}
.ansi-default-inverse-fg {
  color: #FFFFFF;
}
.ansi-default-inverse-bg {
  background-color: #000000;
}
.ansi-bold {
  font-weight: bold;
}
.ansi-underline {
  text-decoration: underline;
}
/* The following styles are deprecated an will be removed in a future version */
.ansibold {
  font-weight: bold;
}
.ansi-inverse {
  outline: 0.5px dotted;
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
  position: relative;
  overflow: visible;
}
div.cell:before {
  position: absolute;
  display: block;
  top: -1px;
  left: -1px;
  width: 5px;
  height: calc(100% +  2px);
  content: '';
  background: transparent;
}
div.cell.jupyter-soft-selected {
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
div.cell.selected,
div.cell.selected.jupyter-soft-selected {
  border-color: #ababab;
}
div.cell.selected:before,
div.cell.selected.jupyter-soft-selected:before {
  position: absolute;
  display: block;
  top: -1px;
  left: -1px;
  width: 5px;
  height: calc(100% +  2px);
  content: '';
  background: #42A5F5;
}
@media print {
  div.cell.selected,
  div.cell.selected.jupyter-soft-selected {
    border-color: transparent;
  }
}
.edit_mode div.cell.selected {
  border-color: #66BB6A;
}
.edit_mode div.cell.selected:before {
  position: absolute;
  display: block;
  top: -1px;
  left: -1px;
  width: 5px;
  height: calc(100% +  2px);
  content: '';
  background: #66BB6A;
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
  /* Note that this should set vertical padding only, since CodeMirror assumes
       that horizontal padding will be set on CodeMirror pre */
  padding: 0.4em 0;
}
.CodeMirror-linenumber {
  padding: 0 8px 0 4px;
}
.CodeMirror-gutters {
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.CodeMirror pre {
  /* In CM3 this went to 4px from 0 in CM2. This sets horizontal padding only,
    use .CodeMirror-lines for vertical */
  padding: 0 0.4em;
  border: 0;
  border-radius: 0;
}
.CodeMirror-cursor {
  border-left: 1.4px solid black;
}
@media screen and (min-width: 2138px) and (max-width: 4319px) {
  .CodeMirror-cursor {
    border-left: 2px solid black;
  }
}
@media screen and (min-width: 4320px) {
  .CodeMirror-cursor {
    border-left: 4px solid black;
  }
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
div.output_area .mglyph > img {
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
  padding: 1px 0 1px 0;
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
.rendered_html ul:not(.list-inline),
.rendered_html ol:not(.list-inline) {
  padding-left: 2em;
}
.rendered_html ul {
  list-style: disc;
}
.rendered_html ul ul {
  list-style: square;
  margin-top: 0;
}
.rendered_html ul ul ul {
  list-style: circle;
}
.rendered_html ol {
  list-style: decimal;
}
.rendered_html ol ol {
  list-style: upper-alpha;
  margin-top: 0;
}
.rendered_html ol ol ol {
  list-style: lower-alpha;
}
.rendered_html ol ol ol ol {
  list-style: lower-roman;
}
.rendered_html ol ol ol ol ol {
  list-style: decimal;
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
  padding: 0px;
  background-color: #fff;
}
.rendered_html code {
  background-color: #eff0f1;
}
.rendered_html p code {
  padding: 1px 5px;
}
.rendered_html pre code {
  background-color: #fff;
}
.rendered_html pre,
.rendered_html code {
  border: 0;
  color: #000;
  font-size: 100%;
}
.rendered_html blockquote {
  margin: 1em 2em;
}
.rendered_html table {
  margin-left: auto;
  margin-right: auto;
  border: none;
  border-collapse: collapse;
  border-spacing: 0;
  color: black;
  font-size: 12px;
  table-layout: fixed;
}
.rendered_html thead {
  border-bottom: 1px solid black;
  vertical-align: bottom;
}
.rendered_html tr,
.rendered_html th,
.rendered_html td {
  text-align: right;
  vertical-align: middle;
  padding: 0.5em 0.5em;
  line-height: normal;
  white-space: normal;
  max-width: none;
  border: none;
}
.rendered_html th {
  font-weight: bold;
}
.rendered_html tbody tr:nth-child(odd) {
  background: #f5f5f5;
}
.rendered_html tbody tr:hover {
  background: rgba(66, 165, 245, 0.2);
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
.rendered_html .alert {
  margin-bottom: initial;
}
.rendered_html * + .alert {
  margin-top: 1em;
}
[dir="rtl"] .rendered_html p {
  text-align: right;
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
.text_cell.rendered .rendered_html tr,
.text_cell.rendered .rendered_html th,
.text_cell.rendered .rendered_html td {
  max-width: none;
}
.text_cell.unrendered .text_cell_render {
  display: none;
}
.text_cell .dropzone .input_area {
  border: 2px dashed #bababa;
  margin: -1px;
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
.jupyter-keybindings {
  padding: 1px;
  line-height: 24px;
  border-bottom: 1px solid gray;
}
.jupyter-keybindings input {
  margin: 0;
  padding: 0;
  border: none;
}
.jupyter-keybindings i {
  padding: 6px;
}
.well code {
  background-color: #ffffff;
  border-color: #ababab;
  border-width: 1px;
  border-style: solid;
  padding: 2px;
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
.tags_button_container {
  width: 100%;
  display: flex;
}
.tag-container {
  display: flex;
  flex-direction: row;
  flex-grow: 1;
  overflow: hidden;
  position: relative;
}
.tag-container > * {
  margin: 0 4px;
}
.remove-tag-btn {
  margin-left: 4px;
}
.tags-input {
  display: flex;
}
.cell-tag:last-child:after {
  content: "";
  position: absolute;
  right: 0;
  width: 40px;
  height: 100%;
  /* Fade to background color of cell toolbar */
  background: linear-gradient(to right, rgba(0, 0, 0, 0), #EEE);
}
.tags-input > * {
  margin-left: 4px;
}
.cell-tag,
.tags-input input,
.tags-input button {
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
  box-shadow: none;
  width: inherit;
  font-size: inherit;
  height: 22px;
  line-height: 22px;
  padding: 0px 4px;
  display: inline-block;
}
.cell-tag:focus,
.tags-input input:focus,
.tags-input button:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.cell-tag::-moz-placeholder,
.tags-input input::-moz-placeholder,
.tags-input button::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.cell-tag:-ms-input-placeholder,
.tags-input input:-ms-input-placeholder,
.tags-input button:-ms-input-placeholder {
  color: #999;
}
.cell-tag::-webkit-input-placeholder,
.tags-input input::-webkit-input-placeholder,
.tags-input button::-webkit-input-placeholder {
  color: #999;
}
.cell-tag::-ms-expand,
.tags-input input::-ms-expand,
.tags-input button::-ms-expand {
  border: 0;
  background-color: transparent;
}
.cell-tag[disabled],
.tags-input input[disabled],
.tags-input button[disabled],
.cell-tag[readonly],
.tags-input input[readonly],
.tags-input button[readonly],
fieldset[disabled] .cell-tag,
fieldset[disabled] .tags-input input,
fieldset[disabled] .tags-input button {
  background-color: #eeeeee;
  opacity: 1;
}
.cell-tag[disabled],
.tags-input input[disabled],
.tags-input button[disabled],
fieldset[disabled] .cell-tag,
fieldset[disabled] .tags-input input,
fieldset[disabled] .tags-input button {
  cursor: not-allowed;
}
textarea.cell-tag,
textarea.tags-input input,
textarea.tags-input button {
  height: auto;
}
select.cell-tag,
select.tags-input input,
select.tags-input button {
  height: 30px;
  line-height: 30px;
}
textarea.cell-tag,
textarea.tags-input input,
textarea.tags-input button,
select[multiple].cell-tag,
select[multiple].tags-input input,
select[multiple].tags-input button {
  height: auto;
}
.cell-tag,
.tags-input button {
  padding: 0px 4px;
}
.cell-tag {
  background-color: #fff;
  white-space: nowrap;
}
.tags-input input[type=text]:focus {
  outline: none;
  box-shadow: none;
  border-color: #ccc;
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
#kernel_logo_widget .current_kernel_logo {
  display: none;
  margin-top: -1px;
  margin-bottom: -1px;
  width: 32px;
  height: 32px;
}
[dir="rtl"] #kernel_logo_widget {
  float: left !important;
  float: left;
}
.modal .modal-body .move-path {
  display: flex;
  flex-direction: row;
  justify-content: space;
  align-items: center;
}
.modal .modal-body .move-path .server-root {
  padding-right: 20px;
}
.modal .modal-body .move-path .path-input {
  flex: 1;
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
[dir="rtl"] #menubar .navbar-toggle {
  float: right;
}
[dir="rtl"] #menubar .navbar-collapse {
  clear: right;
}
[dir="rtl"] #menubar .navbar-nav {
  float: right;
}
[dir="rtl"] #menubar .nav {
  padding-right: 0px;
}
[dir="rtl"] #menubar .navbar-nav > li {
  float: right;
}
[dir="rtl"] #menubar .navbar-right {
  float: left !important;
}
[dir="rtl"] ul.dropdown-menu {
  text-align: right;
  left: auto;
}
[dir="rtl"] ul#new-menu.dropdown-menu {
  right: auto;
  left: 0;
}
.nav-wrapper {
  border-bottom: 1px solid #e7e7e7;
}
i.menu-icon {
  padding-top: 4px;
}
[dir="rtl"] i.menu-icon.pull-right {
  float: left !important;
  float: left;
}
ul#help_menu li a {
  overflow: hidden;
  padding-right: 2.2em;
}
ul#help_menu li a i {
  margin-right: -1.2em;
}
[dir="rtl"] ul#help_menu li a {
  padding-left: 2.2em;
}
[dir="rtl"] ul#help_menu li a i {
  margin-right: 0;
  margin-left: -1.2em;
}
[dir="rtl"] ul#help_menu li a i.pull-right {
  float: left !important;
  float: left;
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
[dir="rtl"] .dropdown-submenu > .dropdown-menu {
  right: 100%;
  margin-right: -1px;
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
.dropdown-submenu > a:after.fa-pull-left {
  margin-right: .3em;
}
.dropdown-submenu > a:after.fa-pull-right {
  margin-left: .3em;
}
.dropdown-submenu > a:after.pull-left {
  margin-right: .3em;
}
.dropdown-submenu > a:after.pull-right {
  margin-left: .3em;
}
[dir="rtl"] .dropdown-submenu > a:after {
  float: left;
  content: "\f0d9";
  margin-right: 0;
  margin-left: -10px;
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
[dir="rtl"] #notification_area {
  float: left !important;
  float: left;
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
[dir="rtl"] .indicator_area {
  float: left !important;
  float: left;
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
[dir="rtl"] #kernel_indicator {
  float: left !important;
  float: left;
  border-left: 0;
  border-right: 1px solid;
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
[dir="rtl"] #modal_indicator {
  float: left !important;
  float: left;
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
.edit_mode .modal_indicator:before.fa-pull-left {
  margin-right: .3em;
}
.edit_mode .modal_indicator:before.fa-pull-right {
  margin-left: .3em;
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
.command_mode .modal_indicator:before.fa-pull-left {
  margin-right: .3em;
}
.command_mode .modal_indicator:before.fa-pull-right {
  margin-left: .3em;
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
.kernel_idle_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_idle_icon:before.fa-pull-right {
  margin-left: .3em;
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
.kernel_busy_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_busy_icon:before.fa-pull-right {
  margin-left: .3em;
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
.kernel_dead_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_dead_icon:before.fa-pull-right {
  margin-left: .3em;
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
.kernel_disconnected_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_disconnected_icon:before.fa-pull-right {
  margin-left: .3em;
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
  height: 30px;
  margin-top: 4px;
  display: flex;
  justify-content: flex-start;
  align-items: baseline;
  width: 50%;
  flex: 1;
}
span.save_widget span.filename {
  height: 100%;
  line-height: 1em;
  margin-left: 16px;
  border: none;
  font-size: 146.5%;
  text-overflow: ellipsis;
  overflow: hidden;
  white-space: nowrap;
  border-radius: 2px;
}
span.save_widget span.filename:hover {
  background-color: #e6e6e6;
}
[dir="rtl"] span.save_widget.pull-left {
  float: right !important;
  float: right;
}
[dir="rtl"] span.save_widget span.filename {
  margin-left: 0;
  margin-right: 16px;
}
span.checkpoint_status,
span.autosave_status {
  font-size: small;
  white-space: nowrap;
  padding: 0 5px;
}
@media (max-width: 767px) {
  span.save_widget {
    font-size: small;
    padding: 0 0 0 5px;
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
.toolbar-btn-label {
  margin-left: 6px;
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
[dir="rtl"] .btn-group > .btn,
.btn-group-vertical > .btn {
  float: right;
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
[dir="rtl"] ul.typeahead-list i {
  margin-left: 0;
  margin-right: -10px;
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
ul.typeahead-list  > li > a.pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .typeahead-list {
  text-align: right;
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
  min-width: 20px;
  color: transparent;
}
[dir="rtl"] .no-shortcut.pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .command-shortcut.pull-right {
  float: left !important;
  float: left;
}
.command-shortcut:before {
  content: "(command mode)";
  padding-right: 3px;
  color: #777777;
}
.edit-shortcut:before {
  content: "(edit)";
  padding-right: 3px;
  color: #777777;
}
[dir="rtl"] .edit-shortcut.pull-right {
  float: left !important;
  float: left;
}
#find-and-replace #replace-preview .match,
#find-and-replace #replace-preview .insert {
  background-color: #BBDEFB;
  border-color: #90CAF9;
  border-style: solid;
  border-width: 1px;
  border-radius: 0px;
}
[dir="ltr"] #find-and-replace .input-group-btn + .form-control {
  border-left: none;
}
[dir="rtl"] #find-and-replace .input-group-btn + .form-control {
  border-right: none;
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

<div class="cell border-box-sizing code_cell rendered">

</div>
<div class="cell border-box-sizing code_cell rendered">

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Simplified-Molecular-Input-Line-Entry-System-(SMILES)"><a href="https://www.daylight.com/dayhtml/doc/theory/theory.smiles.html">Simplified Molecular Input Line Entry System (SMILES)</a><a class="anchor-link" href="#Simplified-Molecular-Input-Line-Entry-System-(SMILES)">&#182;</a></h1><h2 id="Advantages:">Advantages:<a class="anchor-link" href="#Advantages:">&#182;</a></h2><ul>
<li>Efficient: smaller data files</li>
</ul>
<h2 id="Disadvantages:">Disadvantages:<a class="anchor-link" href="#Disadvantages:">&#182;</a></h2><ul>
<li>Only capable of encoding 2D structure information</li>
<li>Can only include one identifier for each compound (i.e. no other molecule attributes)</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>CC(=O)NC1CCSC1=O
</pre>
</div>
</div>

<div class="output_area">



<div class="output_png output_subarea output_execute_result">
<img src="data:image/png;base64,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Wlqq7du3a/bs2Y1eJPpNI0aMUGFhocrLy5WYmKiSkpIWnt49PvjgA33xxRe6++67nR6lRYWEhHBNVhMIVgspLi7W4sWL1aNHD02fPl1hYWHauHGjDh48qKeeekp9+/b9Vr+3R48eys/PV2JiokaOHKlt27Y18+TulJubq8TERHVu7ClCrchDDz2kHTt26JNPPnF6FNchWM3o1KlTyszMVEJCgoYOHao9e/bo6aef1pEjR5SVlaVx48Y1y9NdwsLClJWVpYULF2rSpEl64YUXmmF6d2std2e4Gv3791dSUhLXZAXi9DGp7aqrq8369etNamqqCQ0NNQMHDjRPPPGEOXjwYFDePzs720RERJjZs2ebCxcuBOU9g62ystJ4vV6za9cup0cJmj//+c8mLi7O+Hw+p0dxlbZ7j5LrtGfPHmVlZemVV15RbW2t0tLStG3bNo0aNSqoc0yfPl39+vXT1KlTNXnyZL366nrdeGN4UGdoaW+99ZY6duyoO+64w+lRguLkyZNau3athg4dqpAQDoIuxX+Na3D06FEtXbpUt99+u5KSkrRv3z49++yzOnr0qDIyMoIeqwbDhw/X7t27FRv7EyUlhau1fR2t4WGpbeEK/w8++ECJiYny+Xxavny50+O4DsG6gurqamVnZ+uee+5Rr169lJmZqfvvv19HjhxRXl6eZs6cqfBw51c0MTExysxMUXKylJgobdjg9ETX79y5c1q5cqXy8/PbxMn2NWvWKDk5WePHj9e2bdsUExPj9Eju4/QxqVsVFhaa+fPnmy5dupjOnTub2bNnm8LCQqfHuirPP29Mhw7GPPWU05NcO5/PZ9566y0zc+ZMExERYXr06GFmzJhhOnbsaFJSUszx48edHrHZ1dbWmkWLFpmwsDCzYsUKp8dxNYL1DatXrzbx8fHG6/WalJQUs379eitPZm/ebExUlDEPPGBMVZXT01zZZ599Zp566inTt29fExYWZlJTU8369etNbW2tMcaYTz/91Nx1110mOjraZGRkODxt8/niiy/MXXfdZeLi4szu3budHsf1CNY3bNy40bz44oumvLzc6VGuW0mJMQMGGDNypDFuXJhUVJw2mZmZJjk52Xg8HpOcnGyWLVvW6FX89fX1JiMjw0RGRpopU6aYw4cPB3ni5lVQUGB69uxpxowZY06cOOH0OFYgWK1cebkxY8cac8stxrjhiNbnMyYvz5gZM4xJSso3t9xyi1m0aJHZv3//Vf+OTz/91IwdO9bq1VZGRobxer1m/vz5F1eRuDKC1QbU1hozf74xERHG5OQ4M0NxsTELFxoTG2tMZKQxM2ca89Zb9d/6OqOG1VanTp3M5MmTzeeff97ME7eM6upq8/DDD5vIyMhW/73IlkCw2pCMDP/J+EWLjGnkphDNqqLC/57JycaEhPj/zMgw5uzZ5nuPAwcOmLvvvtuK1dbhw4dNUlKSiY+PN3v37nV6HCsRrDYmP9+Ym24yJi3NmC+/bJn3+OwzY1JSjPF6jYmPN+Y3vzHmwIGWeS9jvr7amjRpkitXW/n5+SYmJsZMnjyZW8dcB67DamPuvFN6911p715p9eqWeY/oaKlrV2nrVmn/funxx6WWvA29x+PR7NmztXfvXtXW1mrw4MHKzMyUccnNdDMzMzVu3Dilp6drw4YNio6Odnoka3GL5DaqslKKiJCa4bvYrmKM0bJly7RgwQKNHDlSmZmZiouLc2SW6upqzZ07Vzk5OVq5cqXuu+8+R+ZoTVhhtVGRkZfEqkxK9khzvvm09P+8vvmbf29sHxdoWG199NFHCg0N1ZAhQxxZbR06dEh33nmndu7cqV27dhGrZkKwcFHmZPeE53rFxsZq/fr1WrZsmRYvXqxJkybp0KFDQXnvLVu2aPjw4YqNjdW//vUvDRo0KCjv2xYQLFy0aZM0eY7TUzSv1NRUFRcXy+v1tvhqyxijJUuWaOrUqVq4cKHWrVunqKioFnmvtopg4SuTpE0KcGhoue7du+uNN97Q8uXL9ctf/lITJ05s9tVWZWWl0tLS9Mwzz2jDhg1atGhRs9ysEV9HsPA1kzIkPSmVNbJ9ssd/7uviT3/p3WAOeB1SU1NVVFSk8PBwDRkyREuXLlV9ff11/97S0lKNGDFCZWVlKigo0IQJE5phWgRCsHCZBWlS+tLA2zYZyVz6UyqNDO5416V79+5at26dli9frt/+9rcaM2aMysoay/OVbdy4UYmJiRo2bJh27NihPn36NOO0+CaChcvEPyqlvSotLXV6kpbTsNrq0qWLhg0bpiVLllzTaqvhfNW0adO0ePFirVmzRh07dmzBiSFJ3CIZAT26Skq26HDv24iJidHrr7+u7OxszZ07V2+++aZWrFih/v37N/nvzp49q/T0dO3YsUObN2/W2LFjgzQxWGEhsHhp1fNODxEcDZ8k3nTTTbr99tubXG19/PHHSkpK0qFDh1RQUECsgowr3YFLZGdna968eRowYIBWrFihW2+99eK2tWvXatasWZo2bZoyMjJccWvstoYVFnCJhnNb3bp1u7jaqq2t1eLFi5Wenq7nnntOWVlZxMohrLCARrz88suaP3++YmJidPr0af39739XUlKS02O1aQQLaMKJEydUVFSkwYMHq1u3bk6P0+YRLADW4BwWAGsQLADWIFgArEGwAFiDYAGwBsECYA2CBcAaBAuANQgWAGsQLADWIFgArEGwAFiDYAGwBsECYA2CBcAaBAuANQgWAGsQLADWIFgArEGwAFiDYAGwBsECYA2CBcAaBAuANQgWAGsQLADWIFgArEGwAFiDYAGwBsECYA2CBcAaBAuANQgWAGsQLADWIFgArEGwAFiDYAGwBsECYA2CBcAaBAuANQgWAGsQLADWIFgArEGwAFiDYAGwBsECYA2CBcAaBAuANQgWAGsQLADWIFgArEGwAFiDYAGwBsECYA2CBcAaBAuANQgWAGsQLADWIFgArEGwAFiDYAGwBsECYA2CBcAaBAuANQgWAGsQLADWIFgArEGwAFiDYAGwBsECYA2CBcAaBAuANQgWAGsQLADWIFgArEGwAFiDYAGwBsECYA2CBcAaBAuANQgWAGsQLADWIFgArEGwAFiDYAGwBsECYA2CBcAaBAuANQgWAGsQLADWIFgArEGwAFiDYAGwBsECYA2CBcAaBAuANQgWAGsQLADWIFgArEGwAFiDYAGwBsECYA2CBcAaBAuANf4fk5KZzqRgtH8AAAAASUVORK5CYII=
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Structure-Data-File-(SDF)"><a href="http://www.structuralchemistry.org/pcsb/capp_cdf.php">Structure Data File (SDF)</a><a class="anchor-link" href="#Structure-Data-File-(SDF)">&#182;</a></h1><h2 id="Advantages:">Advantages:<a class="anchor-link" href="#Advantages:">&#182;</a></h2><ul>
<li>Capable of encoding 3D coordinates</li>
<li>Can include as many properties for each molecule as desired</li>
</ul>
<h2 id="Disadvantages:">Disadvantages:<a class="anchor-link" href="#Disadvantages:">&#182;</a></h2><ul>
<li>Larger files (10 $-$ 100 $\times$ more memory)</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>
     RDKit          2D

 10 10  0  0  0  0  0  0  0  0999 V2000
    4.6250   -5.5000    0.0000 C   0  0  0  0  0  0  0  0  0  0  0  0
    5.3417   -4.2542    0.0000 N   0  0  0  0  0  0  0  0  0  0  0  0
    4.6292   -4.6750    0.0000 C   0  0  0  0  0  0  0  0  0  0  0  0
    3.9167   -5.9167    0.0000 S   0  0  0  0  0  0  0  0  0  0  0  0
    6.0542   -4.6625    0.0000 C   0  0  0  0  0  0  0  0  0  0  0  0
    5.3417   -5.9125    0.0000 O   0  0  0  0  0  0  0  0  0  0  0  0
    6.0667   -5.4875    0.0000 O   0  0  0  0  0  0  0  0  0  0  0  0
    3.2042   -4.6667    0.0000 C   0  0  0  0  0  0  0  0  0  0  0  0
    3.2042   -5.4917    0.0000 C   0  0  0  0  0  0  0  0  0  0  0  0
    6.7667   -4.2417    0.0000 C   0  0  0  0  0  0  0  0  0  0  0  0
  2  3  1  0
  3  1  1  0
  4  1  1  0
  5  2  1  0
  6  1  2  0
  7  5  2  0
  8  3  1  0
  9  4  1  0
 10  5  1  0
  8  9  1  0
M  END

</pre>
</div>
</div>

<div class="output_area">


<div class="output_html rendered_html output_subarea ">
<div id="3dmolviewer_15609895514740243"  style="position: relative; width: 400px; height: 400px">
        <p id="3dmolwarning_15609895514740243" style="background-color:#ffcccc;color:black">You appear to be running in JupyterLab (or JavaScript failed to load for some other reason).  You need to install the 3dmol extension: <br>
        <tt>jupyter labextension install jupyterlab_3dmol</tt></p>
        </div>
<script>

var loadScriptAsync = function(uri){
  return new Promise((resolve, reject) => {
    var tag = document.createElement('script');
    tag.src = uri;
    tag.async = true;
    tag.onload = () => {
      resolve();
    };
  var firstScriptTag = document.getElementsByTagName('script')[0];
  firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);
});
};

if(typeof $3Dmolpromise === 'undefined') {
$3Dmolpromise = null;
  $3Dmolpromise = loadScriptAsync('https://3dmol.csb.pitt.edu/build/3Dmol.js');
}

var viewer_15609895514740243 = null;
var warn = document.getElementById("3dmolwarning_15609895514740243");
if(warn) {
    warn.parentNode.removeChild(warn);
}
$3Dmolpromise.then(function() {
viewer_15609895514740243 = $3Dmol.createViewer($("#3dmolviewer_15609895514740243"),{backgroundColor:"white"});
	viewer_15609895514740243.removeAllModels();
	viewer_15609895514740243.addModel("\n     RDKit          2D\n\n 10 10  0  0  0  0  0  0  0  0999 V2000\n    4.6250   -5.5000    0.0000 C   0  0  0  0  0  0  0  0  0  0  0  0\n    5.3417   -4.2542    0.0000 N   0  0  0  0  0  0  0  0  0  0  0  0\n    4.6292   -4.6750    0.0000 C   0  0  0  0  0  0  0  0  0  0  0  0\n    3.9167   -5.9167    0.0000 S   0  0  0  0  0  0  0  0  0  0  0  0\n    6.0542   -4.6625    0.0000 C   0  0  0  0  0  0  0  0  0  0  0  0\n    5.3417   -5.9125    0.0000 O   0  0  0  0  0  0  0  0  0  0  0  0\n    6.0667   -5.4875    0.0000 O   0  0  0  0  0  0  0  0  0  0  0  0\n    3.2042   -4.6667    0.0000 C   0  0  0  0  0  0  0  0  0  0  0  0\n    3.2042   -5.4917    0.0000 C   0  0  0  0  0  0  0  0  0  0  0  0\n    6.7667   -4.2417    0.0000 C   0  0  0  0  0  0  0  0  0  0  0  0\n  2  3  1  0\n  3  1  1  0\n  4  1  1  0\n  5  2  1  0\n  6  1  2  0\n  7  5  2  0\n  8  3  1  0\n  9  4  1  0\n 10  5  1  0\n  8  9  1  0\nM  END\n","sdf");
	viewer_15609895514740243.setStyle({"stick": {}});
	viewer_15609895514740243.setBackgroundColor("0xeeeeee");
	viewer_15609895514740243.zoomTo();
viewer_15609895514740243.render();
});
</script>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="2D-molecules-can-be-converted-to-3D-using-RDKit">2D molecules can be converted to <a href="https://www.rdkit.org/docs/GettingStartedInPython.html#working-with-3d-molecules">3D using RDKit</a><a class="anchor-link" href="#2D-molecules-can-be-converted-to-3D-using-RDKit">&#182;</a></h2><ul>
<li>3D structure coordinates are needed to calculate 3D molecular descriptors (see normalized principle moment ratio and plane of best fit later on)</li>
<li>After 3D coordinates are generated, they can be saved in SDF format</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>
     RDKit          3D

 19 19  0  0  0  0  0  0  0  0999 V2000
   -1.3912   -0.7729    1.3471 C   0  0  0  0  0  0  0  0  0  0  0  0
    0.8149   -0.2635    0.4168 N   0  0  0  0  0  0  0  0  0  0  0  0
   -0.5829    0.1418    0.4393 C   0  0  0  0  0  0  0  0  0  0  0  0
   -3.0360   -0.9679    0.7518 S   0  0  0  0  0  0  0  0  0  0  0  0
    1.7695    0.5369   -0.1621 C   0  0  0  0  0  0  0  0  0  0  0  0
   -0.9751   -1.3091    2.3644 O   0  0  0  0  0  0  0  0  0  0  0  0
    1.5013    1.5607   -0.7817 O   0  0  0  0  0  0  0  0  0  0  0  0
   -1.2598    0.0308   -0.9249 C   0  0  0  0  0  0  0  0  0  0  0  0
   -2.7563    0.1070   -0.6829 C   0  0  0  0  0  0  0  0  0  0  0  0
    3.1829    0.0599    0.0334 C   0  0  0  0  0  0  0  0  0  0  0  0
    1.1099   -0.9218    1.1331 H   0  0  0  0  0  0  0  0  0  0  0  0
   -0.6496    1.1641    0.8313 H   0  0  0  0  0  0  0  0  0  0  0  0
   -0.9370    0.8272   -1.6038 H   0  0  0  0  0  0  0  0  0  0  0  0
   -1.0022   -0.9206   -1.4107 H   0  0  0  0  0  0  0  0  0  0  0  0
   -3.0643    1.1273   -0.4334 H   0  0  0  0  0  0  0  0  0  0  0  0
   -3.3289   -0.2370   -1.5482 H   0  0  0  0  0  0  0  0  0  0  0  0
    3.6838    0.7108    0.7545 H   0  0  0  0  0  0  0  0  0  0  0  0
    3.2128   -0.9696    0.4012 H   0  0  0  0  0  0  0  0  0  0  0  0
    3.7081    0.0959   -0.9251 H   0  0  0  0  0  0  0  0  0  0  0  0
  2  3  1  0
  3  1  1  0
  4  1  1  0
  5  2  1  0
  6  1  2  0
  7  5  2  0
  8  3  1  0
  9  4  1  0
 10  5  1  0
  8  9  1  0
  2 11  1  0
  3 12  1  0
  8 13  1  0
  8 14  1  0
  9 15  1  0
  9 16  1  0
 10 17  1  0
 10 18  1  0
 10 19  1  0
M  END

</pre>
</div>
</div>

<div class="output_area">


<div class="output_html rendered_html output_subarea ">
<div id="3dmolviewer_15609895515478272"  style="position: relative; width: 400px; height: 400px">
        <p id="3dmolwarning_15609895515478272" style="background-color:#ffcccc;color:black">You appear to be running in JupyterLab (or JavaScript failed to load for some other reason).  You need to install the 3dmol extension: <br>
        <tt>jupyter labextension install jupyterlab_3dmol</tt></p>
        </div>
<script>

var loadScriptAsync = function(uri){
  return new Promise((resolve, reject) => {
    var tag = document.createElement('script');
    tag.src = uri;
    tag.async = true;
    tag.onload = () => {
      resolve();
    };
  var firstScriptTag = document.getElementsByTagName('script')[0];
  firstScriptTag.parentNode.insertBefore(tag, firstScriptTag);
});
};

if(typeof $3Dmolpromise === 'undefined') {
$3Dmolpromise = null;
  $3Dmolpromise = loadScriptAsync('https://3dmol.csb.pitt.edu/build/3Dmol.js');
}

var viewer_15609895515478272 = null;
var warn = document.getElementById("3dmolwarning_15609895515478272");
if(warn) {
    warn.parentNode.removeChild(warn);
}
$3Dmolpromise.then(function() {
viewer_15609895515478272 = $3Dmol.createViewer($("#3dmolviewer_15609895515478272"),{backgroundColor:"white"});
	viewer_15609895515478272.removeAllModels();
	viewer_15609895515478272.addModel("\n     RDKit          3D\n\n 19 19  0  0  0  0  0  0  0  0999 V2000\n   -1.3912   -0.7729    1.3471 C   0  0  0  0  0  0  0  0  0  0  0  0\n    0.8149   -0.2635    0.4168 N   0  0  0  0  0  0  0  0  0  0  0  0\n   -0.5829    0.1418    0.4393 C   0  0  0  0  0  0  0  0  0  0  0  0\n   -3.0360   -0.9679    0.7518 S   0  0  0  0  0  0  0  0  0  0  0  0\n    1.7695    0.5369   -0.1621 C   0  0  0  0  0  0  0  0  0  0  0  0\n   -0.9751   -1.3091    2.3644 O   0  0  0  0  0  0  0  0  0  0  0  0\n    1.5013    1.5607   -0.7817 O   0  0  0  0  0  0  0  0  0  0  0  0\n   -1.2598    0.0308   -0.9249 C   0  0  0  0  0  0  0  0  0  0  0  0\n   -2.7563    0.1070   -0.6829 C   0  0  0  0  0  0  0  0  0  0  0  0\n    3.1829    0.0599    0.0334 C   0  0  0  0  0  0  0  0  0  0  0  0\n    1.1099   -0.9218    1.1331 H   0  0  0  0  0  0  0  0  0  0  0  0\n   -0.6496    1.1641    0.8313 H   0  0  0  0  0  0  0  0  0  0  0  0\n   -0.9370    0.8272   -1.6038 H   0  0  0  0  0  0  0  0  0  0  0  0\n   -1.0022   -0.9206   -1.4107 H   0  0  0  0  0  0  0  0  0  0  0  0\n   -3.0643    1.1273   -0.4334 H   0  0  0  0  0  0  0  0  0  0  0  0\n   -3.3289   -0.2370   -1.5482 H   0  0  0  0  0  0  0  0  0  0  0  0\n    3.6838    0.7108    0.7545 H   0  0  0  0  0  0  0  0  0  0  0  0\n    3.2128   -0.9696    0.4012 H   0  0  0  0  0  0  0  0  0  0  0  0\n    3.7081    0.0959   -0.9251 H   0  0  0  0  0  0  0  0  0  0  0  0\n  2  3  1  0\n  3  1  1  0\n  4  1  1  0\n  5  2  1  0\n  6  1  2  0\n  7  5  2  0\n  8  3  1  0\n  9  4  1  0\n 10  5  1  0\n  8  9  1  0\n  2 11  1  0\n  3 12  1  0\n  8 13  1  0\n  8 14  1  0\n  9 15  1  0\n  9 16  1  0\n 10 17  1  0\n 10 18  1  0\n 10 19  1  0\nM  END\n","sdf");
	viewer_15609895515478272.setStyle({"stick": {}});
	viewer_15609895515478272.setBackgroundColor("0xeeeeee");
	viewer_15609895515478272.zoomTo();
viewer_15609895515478272.render();
});
</script>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h2 id="Additional-molecular-properties-are-stored-for-each-molecule-after-the-end-of-the-compound-structure-coordinates-(M-END)-and-before-the-compound-delimiter-($\$\$\$\$$)">Additional molecular properties are stored for each molecule after the end of the compound structure coordinates (M END) and before the compound delimiter ($\$\$\$\$$)<a class="anchor-link" href="#Additional-molecular-properties-are-stored-for-each-molecule-after-the-end-of-the-compound-structure-coordinates-(M-END)-and-before-the-compound-delimiter-($\$\$\$\$$)">&#182;</a></h2>
</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">

<div class="output_area">



<div class="output_text output_subarea output_execute_result">
<pre>[&#39;Code&#39;,
 &#39;Structure_smiles&#39;,
 &#39;Appearance&#39;,
 &#39;casno&#39;,
 &#39;product_name&#39;,
 &#39;c_log_p&#39;,
 &#39;acd_code&#39;,
 &#39;Flexibility&#39;,
 &#39;PSA&#39;,
 &#39;h_bond_donors&#39;,
 &#39;h_bond_acceptors&#39;,
 &#39;parent_mw&#39;,
 &#39;Heavy_Atom_Count&#39;,
 &#39;PAINS_Free&#39;,
 &#39;Set&#39;]</pre>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="2D-descriptors:">2D descriptors:<a class="anchor-link" href="#2D-descriptors:">&#182;</a></h1><h2 id="a-common-school-of-thought-holds-that-fragment-libraries-should-contain-molecules-with-the-following-attributes:"><a href="http://practicalfragments.blogspot.com/2011/11/pushing-rule-of-3.html">a common school of thought</a> holds that fragment libraries should contain molecules with the following attributes:<a class="anchor-link" href="#a-common-school-of-thought-holds-that-fragment-libraries-should-contain-molecules-with-the-following-attributes:">&#182;</a></h2><ul>
<li>Molecular Weight $\lt$ 300 g/mol</li>
<li>ClogP $\le$ 3</li>
<li>Number of hydrogen bond donors $\le$ 3</li>
<li>Number of hydrogen bond acceptors $\le$ 3</li>
<li>Number of rotatable bonds $\le$ 3</li>
<li>Polar surface area $\le$ 60 Å</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">

<div class="output_area">




 
 
<div id="3ed5d9c2-d671-41cd-bba4-8610d6588348"></div>
<div class="output_subarea output_widget_view ">
<script type="text/javascript">
var element = $('#3ed5d9c2-d671-41cd-bba4-8610d6588348');
</script>
<script type="application/vnd.jupyter.widget-view+json">
{"model_id": "b48c84858f444a7fa206efbc49697400", "version_major": 2, "version_minor": 0}
</script>
</div>

</div>

<div class="output_area">

<div class="output_subarea output_stream output_stdout output_text">
<pre>
</pre>
</div>
</div>

<div class="output_area">



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
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="3-dimensionality-(vs.-flat-structures)-as-a-strategy-to-increase-library-diversity"><a href="https://blogs.sciencemag.org/pipeline/archives/2013/08/08/the_3d_fragment_consortium">3-dimensionality (vs. flat structures) as a strategy to increase library diversity</a><a class="anchor-link" href="#3-dimensionality-(vs.-flat-structures)-as-a-strategy-to-increase-library-diversity">&#182;</a></h1><h2 id="Plots-describing-molecule-3D-character-depicted-below">Plots describing molecule 3D character depicted below<a class="anchor-link" href="#Plots-describing-molecule-3D-character-depicted-below">&#182;</a></h2><ul>
<li><a href="https://pubs.acs.org/doi/full/10.1021/ci025599w">2-dimensional normalized ratios of principle moments of inertia</a></li>
<li><a href="https://pubs.acs.org/doi/pdfplus/10.1021/ci300293f">plane of best fit (PBF) score versus sum of NPRs</a></li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">

<div class="output_area">




 
 
<div id="fc99c256-a396-4b22-b870-34bfd0952ca6"></div>
<div class="output_subarea output_widget_view ">
<script type="text/javascript">
var element = $('#fc99c256-a396-4b22-b870-34bfd0952ca6');
</script>
<script type="application/vnd.jupyter.widget-view+json">
{"model_id": "ad319fca4a7e4c7aa3ea0ba553d09983", "version_major": 2, "version_minor": 0}
</script>
</div>

</div>

<div class="output_area">



<div class="output_png output_subarea ">
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAsgAAAEYCAYAAABBfQDEAAAABHNCSVQICAgIfAhkiAAAAAlwSFlzAAALEgAACxIB0t1+/AAAADl0RVh0U29mdHdhcmUAbWF0cGxvdGxpYiB2ZXJzaW9uIDMuMC4yLCBodHRwOi8vbWF0cGxvdGxpYi5vcmcvOIA7rQAAIABJREFUeJzs3Xd4FNX6wPHvmd1N7wmBhF6kk0SIVCFBimABpVjAgoJesYCCV0Gvgl6xgYIFFaX9RKR7EZHee1NCDz2QBimQvnXm/P5YWAkJIYQSynyeJ0+yU86end2dnDnznvcIKSU6nU6n0+l0Op3OSSnvCuh0Op1Op9PpdDcTvYGs0+l0Op1Op9NdQG8g63Q6nU6n0+l0F9AbyDqdTqfT6XQ63QX0BrJOp9PpdDqdTncBvYGs0+l0Op1Op9NdQG8g63Q6nU6n0+l0F9AbyDqdTqfT6XQ63QX0BrJOp9PpdDqdTncBY3lX4EqFhITIGjVqlHc1dDqd7or89ddfGVLKCuVdj2tFPxfryuLgwYMA1KtXr5xrortTlfZcfMs1kGvUqMGOHTvKuxo6nU53RYQQJ8q7DteSfi7WlcWsWbMAePzxx8u5Jro7VWnPxbdcA1mn0+l0Ot2tSW8Y624VegyyTqfT6XS6GyI7O5vs7OzyroZOd1l3ZAO5X79+zJ07F4ABAwawf//+K9rfx8fnkutat25dpjqNHDmSMWPGlGlfnU7ndOF3u6weeOABsrKyrni/qVOn8uqrr17Vc+t0t7vu3bvTvXv38q6GTndZd3yIxcSJE69JOaqqYjAY2LRp0zUpT6fT3VhSSqSULFq0qLyrcsuy2+0kJSVhsVjKuyq6m9QXX3wBwIEDB8q5JqXj4eFBlSpVMJlM5V0V3Q12WzWQf/75Z8aMGYMQglq1ahEXF8ehQ4cwmUzk5OQQERHB4cOHC+0TGxvLmDFjiI6OxsfHh8GDB7Nw4UI8PT35/fffqVixIsePH6dPnz44HA66dOni2nfNmjV88MEHhIWFERcXx/79+/Hx8SEvLw+Azz//nGnTpqEoCl27duXTTz/lp59+4scff8Rms1GnTh2mTZuGl5fXDT1OOt2tJD8/n8cee4ykpCRUVeW9997j7bff5vHHH2f16tUA/Prrr9SpUweAdevW8eWXX3Lq1Ck+//xzevXqBcDo0aOZPXs2VquVRx99lA8++ICEhAS6du1K+/bt2bx5M/PnzycmJoYdO3YQEhJS6JwSERHBtGnT+OOPP/joo4+w2WwEBwczffp0KlasWG7H52aSlJSEr68vNWrUQAhR3tXR6a6KlJLMzEySkpKoWbNmeVdHd4PdNiEW+/btY9SoUaxatYpdu3YxadIkYmNj+fPPPwGYOXMmPXv2LPEqMD8/n5YtW7Jr1y7atWvHTz/9BMDgwYMZOHAg27dvp1KlSoX22bZtG6NGjSoSprF48WLmz5/P1q1b2bVrF2+99RYAPXr0YPv27ezatYsGDRowadKka3kYdLrbzpIlSwgPD2fXrl3s3bvXdZHq5+fHtm3bePXVV3n99ddd26emprJhwwYWLlzIsGHDAFi2bBmHDx9m27ZtxMXF8ddff7Fu3TrAmXbqmWeeYefOnVSvXt1VzsXnlK+++gqAe++9ly1btrBz506eeOIJPv/88xt1KG56FouF4OBgvXGsuyS73Y7dbi/vapSKEILg4GD9jsgd6rZpIK9atYpevXoREhICQFBQEAMGDGDKlCkATJkyheeee67EMtzc3HjooYcAaNasGQkJCQBs3LiRJ598EoCnn3660D7Nmzcv9spyxYoVPPfcc67e4aCgIAD27t1L27ZtadKkCdOnT2ffvn1lfMU63Z2hSZMmrFixgrfffpv169fj7+8P4PpOPvnkk2zevNm1/SOPPIKiKDRs2JDTp08DzgbysmXLuPvuu2natCnx8fGuu0nVq1enZcuWRZ63uHMKOHtJ77//fpo0acLo0aP17/BF9MaxriTHjh3j2LFj5V2NUtM/z3eu2ybEQkpZ5IPcpk0bEhISWLt2Laqq0rhx4xLLMJlMrjIMBgMOh8O17lJfEm9v71LXB5yDiObPn09kZCRTp05lzZo1JdZJp7vT1a1bl7/++otFixYxfPhwOnfuDBT+Tl74t7u7u+tvKaXr9/Dhw/nXv/5VqOyEhIQr/g6/9tprDBkyhG7durFmzRpGjhxZ5tem091p9HAk3a3itulB7tChA7NnzyYzMxOAM2fOAPDMM8/w5JNPXrb3uCRt2rRh5syZAEyfPr1U+3Tu3JnJkydTUFBQqD65ubmEhYVht9tLXZZOdydLSUnBy8uLp556ijfffJO///4b+GfCgVmzZtGqVasSy7j//vuZPHmya3xAcnIyaWlpJe5zqXNKdnY2lStXBuD//u//yv7CdNecxWKhefPmREZG0qhRI0aMGOFaFxsbS7169YiIiKB+/fq8+uqrl8xW8vHHH7v+TkhIuGznSlmsWbPGdceytGJjY4udnOVSGVSsVisdO3YkKirK9X25UiNHjsTLy6vQ9+XCTE4Gg4GoqCgaN25M7969Xf/zLlz+8MMPu451QEAATzzxBAEBAVf8+qdOnYqiKOzevdu1rHHjxq67vTVq1KBJkyZERkbSuXNnTp06VWh5REQEMTExnDjhnCciMTGR9u3b06BBAxo1auQKo7odORwa8fEZFBTcGuEtN4PbpoHcqFEj3n33XWJiYoiMjGTIkCEA9O3bl7Nnz7pux5bFV199xfjx47nnnntKnb+xS5cudOvWjejoaKKiolwp3P773//SokULOnXqRP369ctcJ53uTrFnzx6aN29OVFQUo0aN4j//+Q/g/OffokULvvrqK8aOHVtiGZ07d6ZPnz60atWKJk2a0KtXL3Jzc0vc51LnlJEjR9K7d2/atm3rCr+4mQkhJgsh0oQQey+x/t9CiLhzP3uFEKoQIuhG1/NacHd3d8WMx8XFsWTJErZs2eJaP336dHbv3s3u3btxd3e/ZLqxCxvIpXXhHcebxc6dO7Hb7cTFxZV6gg5VVYssCwkJcWWfuJinpydxcXHs3bsXNzc3fvjhhyLLg4KCGD9+POCMQX7jjTeYNm1aifW41DTmVapUYdSoUZfcb/Xq1ezatYvo6OhC7+Pq1avZvXs3sbGxfPTRRwAYjUa++OILDhw4wJYtWxg/fvwVp329Vbz00iIefHAWXbvO0BvJpXU+tdGt8tOsWTN5JebMmSOfeuqpK9pHp9Pd3KpXry7T09PLuxpXBNghy+GcCbQDmgJ7S7Htw8Cq0pRb3Ll4//79hR7HxMTIKVOmSCmltNlsMiYmRk6bNk1KKWV+fr6MiYmRM2fOlFJKmZWVJWNiYuS8efOklFKmp6fLmJgYuWDBAimllKmpqaU/2OfKv/vuu+WWLVtcddm+fbtrvcPhkDVq1JBxcXGF9nv77beloigyMjJS9unTRx4/flzWr19fDhgwQDZs2FB26tRJFhQUuMocPny4bNeunRwzZoxMS0uTPXr0kNHR0TI6Olpu2LBBSinlmjVrZGRkpIyMjJRRUVEyJydHrl69WsbExMiePXvKevXqyT59+khN06SUUq5YsUJGRUXJxo0by+eee05aLJYir2Hy5Mnyrrvuku3atZMDBgyQr7zySqHXcfr0aVm7dm3p5+cnIyMj5ZEjRy5ZbvXq1eUHH3wg27RpI2fMmFGonBEjRsgRI0bI6tWry8zMTCmllN7e3q71F/79/fffy4EDB5a4PD4+XsbHx8vVq1fLBx988JLvX/Xq1YssmzJlihw4cKBs1KiRjI+Pl1JK2ahRI3n8+HHXPufPC4sXL5Zdu3YtcfnFunXrJpctW1Zk+cWf61uNpmmyZs1vZUTEBFm79ngZH5/hWp6TY3F97u4UpT0X3zY9yMV57bXXGDZsGO+99155V0Wn0+nKhZRyHXCmlJs/Ccy4jtW57lRVJSoqitDQUDp16kSLFi2K3c5gMBAZGUl8fHyh5Z9++qmr9/N8GNzhw4d55ZVX2LdvHwEBAcybN8+1fVZWFmvXrmXo0KEMHjyYN954g+3btzNv3jwGDBgAwJgxYxg/fjxxcXGsX78eT09PwNnDO27cOPbv38+xY8fYuHEjFouFfv36MWvWLPbs2YPD4eD7778vVMfU1FRGjBjBxo0bWb58ebG9nqGhoUycOJG2bdsSFxdH5cqVSyzXw8ODDRs28MQTTxQpy8fHh+eff77EEASHw8HixYtp0qRJkfdj5cqVdOvWDYBKlSoVyQZ1JRRF4a233rpsL//ChQuL1AWcWXEeeeSRIssTEhLYuXPnJT8vtzIhBIMH30Nenp327atTp04gAEOHrqBJk5945pkFaJos51refG6bQXrF+eabb8q7Cjqd7jo4H3Oou3aEEF5AF+CS0wEKIV4EXgSoVq3aZcu8cBCyyWQq9NjLy6vQY39//0KPQ0JCCj0ubaPKYDAQFxdHVlYWjz76KHv37r1kDLGUpWsU1KxZk6ioKKBwhiOgUOjCihUrCjVWc3JyyM3NpU2bNgwZMoS+ffvSo0cPqlSpAjizIJ3/OyoqioSEBHx9falZsyZ169YF4Nlnn2X8+PGFUhlu3bqV2NhYKlSo4KrDoUOHSnwNBw8eLLHcy4VgDBo0iKioKIYOHVpoudlsdh2btm3b0r9//0LLExISaNasGZ06dQJwZaEpziuvvMLGjRsB59iD8+X27t2bd99917Vdnz59GDVqFMePHy9SRvv27TEYDERERLhCKc4vP336NKGhoYWWA+Tl5dGzZ0/GjRuHn59ficfhVjV4cHMGDbrHNfDYYnEwb148wcGebNyYSHJyLlWr3p6vvaxu6wayTqfT6UrtYWCjlPKSvc1Syh+BHwGio6Nv6i6ngIAAYmNjWbJkSbENZFVV2bNnDw0aNLhsWRdmRjEYDJjNZtfjC7OgaJrG5s2bXT3E5w0bNowHH3yQRYsW0bJlS1asWFFsuQ6Ho9SN9itNP3a5ci+VzeW8gIAA+vTpw3fffVdo+fne9oudX56dnc1DDz3E+PHjGTRoEDab7ZLPcT5OGZwxyMWVC87Y4aFDh/LZZ58VWbd69epixwasXr0ab29v+vXrx/vvv8+XX34JOGOie/bs6bp4uZ0VzvZj4P77a7F8+XGaNq1EWJhPCXvema5biEUpBoYIIcTXQogjQojdQoim16suOp1Op7usJ7jFwyvS09Nd2RLMZjMrVqwodjC03W5n+PDhVK1alYiIiCLrTSZTmSaz6Ny5M99++63r8fkG3tGjR2nSpAlvv/020dHRRcI6LlS/fn0SEhI4cuQIANOmTSMmJqbQNi1atGDNmjVkZmZit9uZM2fOZetWmnIvZ8iQIUyYMOGKBiT6+/vz9ddfM2bMGOx2O8ePHy+25/dK9evXjxUrVpCenl7qfTw9PRk3bhw///wzZ86cQUpJ//79adCggWsQ7p1CCMEPPzzA5s39mD27B0bjbR1xWybX84hMxXm77lK6Aned+3kR+L6EbXU6nU53nQgh/IEY4PfyrsvVSE1NpX379kRERHDPPffQqVOnQqnE+vbtS0REBI0bNyY/P5/ffy/+5b744otERETQt2/fK3r+r7/+mh07dhAREUHDhg1dGR3GjRtH48aNiYyMxNPTk65du16yDA8PD6ZMmULv3r1p0qQJiqLw0ksvFdomLCyMkSNH0qpVKzp27EjTppfvXypNuZcTEhLCo48+itVqvaL97r77biIjI5k5cyZhYWE899xz9O7dm5UrV1KlShWWLl16ReWBc2KvQYMGXTZd48XCwsJ48sknGT9+PBs3bmTatGmsWrWKqKgooqKiWLRo0RXX5ValKIJKlXwwGPTGcXFEaW/nlKlwIWoAC6WURe5vCSEmAGuklDPOPT4IxEopU0sqMzo6WhaXB/JaateuHUKIQrcjHnvsMV5++WUKCgp44IEHiuzTr18/+vXrR0ZGBr169SqyfuDAgTz++OMkJiYWmY0PYOjQoTz88MMcPHiwyGQGAP/5z3/o2LEjcXFxhWLRzvv4449p3bo1mzZt4p133imyfty4cURFRbFixYoi8VcAEyZMoF69evzxxx/FpvOZNm0aVatWZdasWUUGjADMnTuXkJAQpk6dytSpU4usX7RoEV5eXnz33XfMnj27yPrzsYZjxoxh4cKFhdZ5enqyePFiwJkmb+XKlYXWBwcHuwbNDB8+vNCsauBMC/TLL78A8Prrrxe5bVe3bl1+/PFHwPmP8eJYPpOpGoryJP3712PBgvdJSkoqtL5Vq1Z88sknAPTs2dOVN/e8Dh06uAaKdu3atdDtWYCHHnqIN998E3DmOb3YlX720tLySUnJpUIFLypX9tM/e5f57J1ff70JIf6SUkZf9ycq+rwzgFggBDgNjABMAFLKH85t0w/oIqUsOkLrEoo7Fx84cKBUIQs63a1E/1zfXkp7Li7Py4bKQOIFj5POLStCCPGiEGKHEGLHldxOKYv09HR27NhBcnLydX2eG8UqQQLzM6DedhiT6Hx8LTlUWLIbTmaWvJ2Ukj//1Ni2TXLixE0dvuhit2ts25bByZN5DB++HVXVyrtKJdI0yfHjWdjtKklJOdhsRXOa6grbs2cPf/zxR3lX47qRUj4ppQyTUpqklFWklJOklD+cbxyf22bqlTSOdbqyslqtV9wDrdOVh/LsQf4T+ERKueHc45XAW1LKv0oq83r3IEspeeihh1izZg179uyhVq1a1+25rlRKNnyzEeoEw3P3gHLR5Y2U8Hki/HkGXguHzVb4PRtqukNSFpgEWDSY0xCiyhiPPycBvtwPHcPggygQQMcxkJABPu6wfjj4eRa/75kzkmbNHPj5QU4O/P23kcDA4geaSCnZuTMfHx8DdeteosAboKDAQbt2f3D2rI2wMC/WrXsIRbmywTE3kqZJOnT4PxITcwgM9GDt2ufw8jKVd7V0lF8P8vWi9yDryuLgwYMA1KtXr5xrUnr65/r2civ0ICcBVS94XAVIKae6uAghmDBhAgaDgRdffLHUI4qvBU2Do6mQZy5+/ZsLYfpO+HgVrD1WdP1xC/x0CjLs8Hayygy7GRmSzTHNQaQPmDUIMkJND+f2VjR+5TQzOY2N0vWMvhcH2XaYkQAb0uD5LfBXChgUyLfClK3w4lz4O6novv7+UL++ID8fGjQQlJRNZ9Kk0zz22EEeemg/mzbllKpu14OXl5EFCzozdmxL/ve/jjd14xicMWW//fY43377AAsX9tEbxyVYv349Q4YMcU2Nq9Pprr/w8HDCw8PLuxo63WWVZwN5AfDMuWwWLYHsy8Uf3yhVqlRh9OjRrFy5kkmTJt2w531vGtz/H+gwHM4UMwuuuxFXfISbofC6FE3jIy0fc8UCChQVtf5plGqnyAvKxlQ1k6l1YX4jWB4B/ueS+80mjamcYjKnmEMa+fxz2ysNC/8jiXj+aZxKJHXCbVgNKr5GmJ8EK0+DsR4YPKFva/hmC6w4DC/MLVp/g0Hw228G5s0zMm+egTm/CV4eDLv3FN12x448VFXDYtHYv79sDZgtWzJo2XIJjz++npycsk+tGR7uTbdu1alQ4cp7su12leTk3GuahH3lyuN8/PEGjh07W+z6wEBPunSpQ8WKetqeSzGbzfTv35/58+ff0Itgne5O5+vri6+vb3lXQ3edrF9/gm++2UZKSjGNmFvMdcuDfOHAECFEEkUHhiwCHgCOAAXAc9erLmXxwgsvMHPmTGbNmkX//v2vOOdkWSzeAR4myMyFg0nQ6qI7Ol88DNP+guqB0LrGP8uzUPnYWsBGTcUjELr4wxaPNBAFOKQBi8mXH0USr3k3ReGf1yE5396WLGM/28mgMw3pSiNeZyeJFGBA8C1RNCaIbznL2XtyqORQ+MERzsYkI0YBfuGS4Q9CBz/BzINgs0PAJdqSnp6CyEjY9je8MRKMGuz4G7atL7zdoEHhHDpkxt/fSPfuwWU6np99to+MDCtpaRZWrEilR4/LT2xwMbtd44MP9hIfn8sHHzSmUaNLJ7m/mNXq4NFH/0d8/BkefLAW33zT6Yqf/2LHj2fx0kuLsdlUliw5xrp1z1x1mXeiESNGcPjwYVasWHHZ/K86ne7asVgsgDOrhu72cuTIGfr3X4DF4mDx4sMsWnRlWWBuNtetgSylfPIy6yXwyvV6/qulKApz587F39//hjSOAV57GP47A+6uDVG1YOUp2HoGnqgGtXwgyAsGtwVNSledjmPjXyRxQnHDjDc+QuFBbyOHhZVsFBRhpx4Z7KKADMyE4hytL5G0JINjpCIIIIVkCrCyhJ2cZRfJVECi4ECykAM0ojXrKMAkBA6TRqbJyot1jIR6Sz51K2CUUSPV5MavfdyZcRiCq0KaDULdin+tQ7+ADAlCQq1iEgg0bOjFqlVFpwm9Eq1ahbBnTxbu7gbq1y99w/ZCq1enMWPGSaSEoUN3MmtWG/z9Sxe2cOJEDgcPnsHf342FC4/y1VdXH6JxvrdTCHHTDxi8WW3fvp0vvviCF154gQ4dOpR3dXS6O8qJEyeAWysGWVc6VqsDTZMoiiAv79ITwtwq9OR3JQgODsZoNJKRkcH69esvv8NVeq4zHJkE8/4Dpx0w8C+YcBT6bXWuL5CSvvazRNnTeUU9zVTS+BszFsxUcztBPY9MhnrmsN+4mPsooBJQHYEXBVTGB28c7GMhx9jISfazkp8I4jeCmUIoh3AgMZDCYRKpzEmM2PGkgEz2sICFtCEZDclduBGNJ4qAqqEaeUYNH2C23Y5nEMz1hw+zofF+OFrMYGVNg9NnILwS+AfC4NfhzU9h4mznQMNr5c03GzJr1r0sXXofDRuWrYFcqZIHUoLZrLFtWw7Nm69mw4aMUu1bs6Y/zZuHcfaslWefbXxN4pdr1Qpk3LjO9OnTiClTHr7q8u40UkpefvllwsLCGD16dHlXR3eNWSwWmjdvTmRkJI0aNWLEiBGudbGxsdSrV4+IiAjq16/Pq6++6ppU5GIff/yx6++EhIRLTlV9NdasWVMoR3NpxMbGUtwg9alTp/Lqq0VnCLdarXTs2JGoqChmzZpVpnqOHDmSypUrExUVRePGjVmwYEGR5fXr12fgwIFomvOivV+/fq7puaOiovj6669d5VWuXJnKlYtNWKUrgd2uMnfuQRYuPHJNQ/aupUaNQvnww/Z061aPCROu7LN9M9Knmi6F559/no0bN7J//34qVqx4XZ4jowD6/wnpBTD+fvD3cYY/CMBx7ruwR9rZLx040PhNcxBvyOIhgggiEYewEGTKYi8pCMCNHL7nISoSQBoFhODJX0whkb9QMFCZe9Gw4+xLltQgiUD8sFGAijvhZBKC85+HFzb2k4kbJt7nbjrSiVwKWMpefAy+1FCqckSTvOhmokCFHCmxAzkaTEiHz6sUbhgqCowbDt9OhwfawbQF8Pd+MBmhXk1oe8+1OaaKImjWrGzhGecdOpSH3S4oKJB4eRmx2TT++COVe+8tOpXpxUwmA7/++jBms+OaDpZ78ME6PPhgnWtW3p1ECMEvv/xCWloa/v5lu2jS3bzc3d1ZtWoVPj4+2O127r33Xrp27UrLli0BmD59OtHR0dhsNoYPH0737t1Zu3ZtkXI+/vjjYnN6l8ThcGA03lz/Unfu3Indbr/klM3FUVUVg6HwIJc33niDN998kwMHDtC2bVvX5Bznl2uaRrt27Vi7di3t27cHYPTo0cXOCeDjo4+NKIvx43cybtwOhACLxUGvXkVniLwZ9OnThD59ru7u783i5vo236Q+++wzoqKieO2114qdaOBqaBoknoWViRB3GgwCxm6Dn7vBuLthdYZG3xoACnWFkSAhOCnBXzhvX3ijUBc3MlFxYEPFjB1QEPjhiQFBRQzY2I+K5dyzSipRnaoIUrDhJ63Ux4tQUQl3OpJIEm7AQSZyFgcm8kihFhJ/Vwzz/1jHIU6iCANf+nYmTFbBpKhMlwepGGYi+3Q1VANs9rCgSW+Ui8JUHmjn/AHYuvOfnmPPmywsbeHCU7i7G/H0dA4y9PQ00LNn6Xs/hBB6JombRG5uLr6+vtSrV0+/vXuDXIuJby50fkKhSxFCuBpgdrsdu91ebIicm5sbn3/+OXXq1GHXrl1ERka61g0bNgyz2UxUVBSNGjVi1KhRqKrKCy+8wKZNm6hcuTK///47np6exMbG0rp1azZu3Ei3bt145plneOmllzh58iTgnCSnTZs2rF27lsGDB7vquG7dOgDy8vLo1asXe/fupVmzZvzyyy8IIVi5ciVvvvkmDoeDe+65h++//x53d/dCr2HKlCl88sknhIWFUbdu3SLr09LSeOqpp0hPTycqKop58+aRkJBQbLk1atTg+eefZ9myZbz66qs88UTxKbEbNGjguqt6IZvNhsViITAwsMT3B3BNlOTpWX7pO29F6ekFrp7jjAzLZbbWXQt6iEUpNGjQgBEjRjBnzhz+97//XdOyX/0V7hsDE5aAmwKKgNZVnOts4fksjUjhZb9U9mIjUChMM7rzg8nKuwZPniaUpwllEPfQjqp0IZDqFBCGlY5UwwcPJJIUXidZDiRULqS2bEUTHiVMtdA+ey698pbzoG0BteQcfLS38DXfx93mtdSWNQjCQnVOEkYGNUijIW60pDZwvndbxYNspLDhrwjmcoxF4iThYYepW28vNeokku1XQM4FU5Ok2ODkRWEX496Ft16A8SMhuowXnmazxvTpOSxZkn9NsxIMGFADk0lQo4YXa9e2Y+fO+2jePOialX8xVdU4dCgTs7nsWTd0RTkcDu677z4GDhxY3lXRXWeqqhIVFUVoaCidOnWiRYsWxW5nMBiIjIwkPj6+0PJPP/0UT09P4uLimD59OgCHDx/mlVdeYd++fQQEBLhm7gTIyspi7dq1DB06lMGDB/PGG2+wfft25s2bx4ABAwDnDKHjx48nLi6O9evXuxqHO3fuZNy4cezfv59jx46xceNGLBYL/fr1Y9asWezZsweHw1FkBsnU1FRGjBjBxo0bWb58Ofv37y/y+kJDQ5k4cSJt27YlLi6OypUrl1iuh4cHGzZsuGTjGGDr1q0oikKFChUAGDt2LFFRUa6/j6n/AAAgAElEQVRGelRUlGvbf//7364Qiz17/klVdPLkSdcFhK703ngjmkceuYs+fRrw1FMNy7s6dwS9B7mU/v3vfzN37lxefvllYmJiCAq6+kaSpsHiveDvCZk58GNPCPaDiFDIRmMomeQjyUCwjHxqoPGj+JN8CvBA5Qla4EkoVfDlWSJQcbATD1RUmnIPUjqQ6i4shl0ImY7AQX37bLz4Dpl6D25aGh5+YHHzwIFEyGw0qwVS3sdDmcfd1YdxzHMb+cRThVRqauvIYxyK+D86Cn9C+RM77qSSRz3exYhAQcOIlbs8D2KWfjSSdVAJ4KTU2J5rZNgxAyD4sjo8HAhHz8CotVCnGnRoXfZj+d//nmH69FyMRvjhh1A6dXJmJkhOtjFgwElsNskPP1TlrruurIv63ntD2LevE0JwQwZrDhjwJ+vWnaRGDX/+/PMJPDz0r+i18OWXX7Jjxw7eeuut8q7KHaWkHl8vL68S14eEhFy2x7g4BoOBuLg4srKyePTRR9m7d+8lY4hLezF9Pp4WoFmzZiQkJLjWPf74466/V6xYUaixmpOTQ25uLm3atGHIkCH07duXHj16UKWKsxekefPmrr+joqJISEjA19eXmjVrUrduXQCeffZZxo8fX2ia961btxIbG+tqqD7++OMcOnSoxNdw8ODBEsu98HVcbOzYsfzyyy/4+voya9Ys17nwfIiF3W6nV69ezJw509XAvlSIxfnXq7syISFefP11x/Kuxh1F70EuJZPJxOTJk7n33ntxOBxlKiM1FV74Fwx5E/LynLG47RrCwRwI8Ic6leGTbEmHYxrj821Yz528NSTVUDhLHlbsFJDPGSysYjFnOHlumwLsrCeKyrSgDSbcIKMjIrUtgXnJgANv1YRijUPui0XYToMEJR/cbL4YbQrGNAfuh7PAbIb8bQQcHU5TRtGMb6ir5hFkPYaPNRmrYwCJfIYHZ/AhkzyOs4/p2JmNH0cJF4nUEkepIlJJMyTwnIjnMeL5t5pCotSwScmqc+mVhy+HVcdg4t+w/Og/x0rTYOchSCndeDjOnFGRUqKqkJ39T3aHGTPOsm+fmaNHrUycWMrCLqIoAiFEkX+mKSkFfPrpPubPT7zEnldG0ySrV5/A19eNhIRskpNv/TySN4ODBw/y/vvv8+ijjxb7D1t3ewoICCA2NpYlS5YUu15VVfbs2VOqGdIuDF8wGAyF/gdcmCZQ0zQ2b95MXFwccXFxJCcn4+vry7Bhw5g4cSJms5mWLVu6eq2LK7e0jfYrvWC/XLklpTt84403XL3fbdu2LbLeZDLRpUsXV+jI5Z5HT62ouxXoDeQrEBUVxZw5cwgNDS3T/l+MhWXLYe5vMOPcgOJtKVA1GLIc8OgWmJOnsUZovJ+poNrc8JIajdDohA+VCSaa2phQqEwOtdhAPG9wkl/JYihZvEkmT6ByCrRsKNgEDgeBp5Kpln0PIacFxqz7EdknwQrCBoZ4gdsCP3yWu+O9Q6JkA4kgEjTIsoJqx4tw/Bz1EFIipMSg5qHIZIzSgVGaqczfWPgcd7YSShoVSEdBYhAqEg+sSMxIfH1zMZpUvIyS55wdH5yfy0IREHxBurdPfoFH34XoF2Demssf2/ffD6Z7dx9eeMGPbt3+GQQSFeWJu7vAaITo6LKflD///CC1ay/lpZd2uuLABg3awXffHeLNN//m77/PlLns8xRFMHBgU7Kzrdx3Xw1q1NAHkV0tTdPo378/Xl5ejB8//oalbNSVj/T0dFdmCrPZzIoVK6hfv+hgJrvdzvDhw6latSoRERFF1ptMJuz2Kw9z6ty5M99++63r8fnBcUePHqVJkya8/fbbREdHFwnruFD9+vVJSEjgyJEjAEybNo2YmJhC27Ro0YI1a9aQmZmJ3W5nzpw5l61bacotKyklmzZtonbt2pfdtqCgQJ+9UndL0O/flsGRI0d47733mDBhAn4lzZd8kbAwiWIQKAIqnUuGUSMIDqaBYoBDNtAMgHTG+LrZ3Bni5s0AfPA8dy3Tk9Z0pCGHWIKV1WhkkiKnUT8vgcC8FGyePqj+qRhEI5DhsOcEwiIw2jYiDF7gnwSnFTgunK1SghCKAzR/Z6P6GJDnrAOnzoBlEHT8Ho/MmthMCtKoYczUCK9xggLhjVQUwIEEqpHICeqRizd+hNKFWGpTiU9IxoqVM4o3NRumUk9YcBfVAE8+6wStq0KYr/NCQUoQAlbGQUoWOOww6GtoWhdqljA7aXi4kW++KXrh0rGjHwsX1sFulzRuXLZBIZom+e674wQEGFm+/DQJCQXUquWNwyE5395S1WsT9/z22635979b3fRTWt8qjhw5Qnx8PGPHjiUsLKy8q6O7zlJTU3n22WdRVRVN03jssccKpVLr27cv7u7urvRnv//+e7HlvPjii0RERNC0aVNGjRpV6uf/+uuveeWVV4iIiMDhcNCuXTt++OEHxo0bx+rVqzEYDDRs2JCuXbuyefPmYsvw8PBgypQp9O7d2zWY7qWXXiq0TVhYGCNHjqRVq1aEhYXRtGlTVFUtsW6lKfdKnQ+9sNvtRERE8PLLL192n8RE5x03faCs7mYnbrVpVqOjo2VxeSBvpC1bttC6dWv+9a9/FRk8URyrVfL009ls327noYf9eOQRd+5r72wIni2AtUehUgh0PYhzQFsFlcAAO20rJlHbkEpzEUIjbHjgSS3qIhDYOMVf8lEcKPhrZ2mYfAShSbB6o3iPQ+yf60yJkb0DCgTknAKTH2TbIcMODhVMnlDRBlKBmB9h83uQdBJ8gTOApkDNmvDaETj2IRz9ELJUEFBwtxu2ij5keVbFQQZGVeWsqQEVxQ9UpDYOLOzlT4y404iuGHHjF5nGtyIVMyq1cWMujVAQ2FTosR72Z8ODleGbaOjyISxdC0KDigGwbAw0uXznxBU5c8aBlBAcfPnrxGef3cHGjZlUq+bJokVt8PAwkJiYz08/HaFxY396966u907epM6cOUNgYGC5vz9CiL+klNHlWolrqLhz8YEDB0oVsqC7c53vPfbyKmaGqJuU/rm+vZT2XKyHWJRBy5Ytef311/nhhx9KNYhk1y4Hf//twMdHsG5tHh3uw9XzGOgFjzSBlmHwSwTUCRB0MBnZH+pJiPE4OcLCFlazjD9YzDyO4RyIoakLqK/uo759P8G2HAx2E4YEFcOBAsTawXBmD2TsAVMlSMoCsxHMOXC6AKx2UDXIV2EvkBIOf62BvGqQBpyGcymSwRbo7MaVLeGkBAtgBa9tNgJS61FZ/ZLqaflUyTATmd2acOpiwMBeFnOEDexjCRuZhJU8GgsvzKgYsHOKbBZwCoDEAtidBelWmHgUEvKhSgWoWBW8/eCpLtC4VvHHdttO+GUe5Odf2Xu4bVsBrVsfpXXrI6xbl3fZ7SdNasqff7Zm4cLWeHg4c4RWrerNhx9G8thjNcq98aUrTErJ7NmzUVWVoKAg/f3R6W4SXl5et1TjuDwcPXqW777byZ496eVdlTuaHmJRRh999BELFixgwIAB7N69u8QvfN26BipUEKSlafTs+c+gDKsdpq9xTpDxZDt4MMj5s0az8LbMwyZNGIWVIBwIQEOjgDwkEof2IUaHFaOQBO7NRSSpzkatewVQCkA6wOANrSZByocQ/yeo0tkA9sZ5aXTCAsEKqOnQLhISrWD3hDNm8BXg7Q9nJbxQByrkQIHmbDR7AlWAjPswheeBwxMQYFnlfF1sx4dluFPAWQSJ7MSO5AQVuZcMdlIPBSM/k8hDVKK6t8DXDVLM4OUG007Cp30hJBjqVoTn2v1zQXFegRn6D4O5i0Ba4MNqsHsleJQyScX8+dkkJTljDGfPzqZdu5KT1xuNCvXq+ZaucF25mzx5MgMGDGDWrFk89thj5V0dnU53Tv653gx9oF7xVFWjd+/fycgwM368G5s3P4Wfn/vld9Rdc3oDuYy8vLyYOHEi7du354svvuC999675LYBAQorVgSRmqpSq9Y/MxS9OxUmLANPN2fEw3MdYZ/qoIc5H5sEL7daNHdPIYIgBCq18cPCJ+zBn9oOP6RIw3BWw5CogoZz2j17LgQ2g7qvgkdVSLbAWV/ICYCTBZBkBqOEQFDPgkwQKBQgEsYhNNXZ4zygLxgUWLsWtm6HWmGQku1sWFvO/UigTTD8PQEC08FdhQwFNWAvmR6D8cFCEyRbaI4Rd06RTwppBKDhhQ1vPPDFgAU7PoobH0fCkD3OsOgKRmg2A9LOQo0M6BgF1S4arzZnMSxcBw4j4A6nMyD5FNSuUbr3r6BAwWZz9jQ6HPqNlNtJcnIyQ4cOJSYmRs9aUQ6klHqPve6SkpKSgFsnBvlGh6GqqsRsdmAyKdhsKjZbybHluutHbyBfhdjYWGbPnl3sbFAX8/YW1KlT+HD/ugLMVudPonPmTvZqKuenWRcaZAI55GHAgyB2IrBjJZUC8RRBRz5A5Dhjgp07GOBvb8iMg7smO+MWtm8BRUOGKshTRnAYEZqGZvHAdjIfNBWjERRHIpYCE1IDj7D7MJ6Khz0HnTHLCSfAxw0c1n8axyYPqN8HfvsMAg3gKcFLAVsyeEhAwQtvmtKDLFIJpAkHWIUFlSYcwEFVzuLLW2ziI1rSvbIHdXydL2XafkjLBocGafmwN61oA9nfFywSMDh/7msJNas515nN8M1EsDtg0AvgW0zncKtWXixY4Oz1b9vW2ZMhpeToUSuBgcZSxSXrbj5SSl566SVsNhsTJ05EUfSLnxvJw8ODzMxMgoOD9UayrljVqlUr7yqUmpSSzMxMPEp7a/IacHMzMHFiF37+eS/du9clJEQPRykveivgKvXu3RtwphRSFKXIdJ8lqR4A+WZniEXfc9MudzKaaGkwcVicJdQjGS8cpBBIDbLxpTY2NmC0mwlIWopilgiDAn4C1PqgPAXJ74EUcGANbLNDlgYKaHkaDruGyc2Bppiwd34Zdd9oDAI0Few2Lxy5+SAh7+k+mAJ88Ug5hWIyIALCICkVAnD2VAO4+8OMfnA8Cww2aCbAoWDwiiGIL7HI5XipLQk13I1dnGQtqwnnKBoqZwkkhwJ8qUoBlUggF3fcCPbTqISRtmEw1R8yM6FOMLSp6syLbHE4QzAAHoiBauGQmeVsLE/6wplXGuDrifD1j2CzQ24efFpM5/5jj/kQFub8+Ldt6zz5jR+fzrhxaXh6KsyfX4vkZDNGo6BVK/9b/p99QYGdrVuTqFcvhPDw2zdUZMaMGSxcuJAvv/ySOnXqlHd17jhVqlQhKSmJ9HQ9dlJ3e/Dw8Ljhk5u0aVOFNm30CVXKm95AvgZycnJo3rw5vXv35r///W+p95v1ASzYAM0bQu1z34UgobDEy4/Z5DINBYEbVajP81RG8BunpRs+toxzPacSiYLIN8K+eLB/A0ZvsORDlSZgOIzNcYbMPFDcFEyqikGA6mYg98gJPB1gVCBXBdXhRpCWh1AUZG4u2PMBgWrTUJPyUawaRgMIT5zxy2Y7HFgOnLv9c6omuBfAyg54BN+FR43DSG0KeR6SLL8wvAjBjQBUFEJIx0Jl8sknDCP++NKTJHLReIVA+lT3Z9OTzqep7ufM9HHfBDiZBSM6wbPR4OYGY96Cf30Cqid8MQtGvQg/z4cvpkJGujNc45ff4P03weuiDG9CCOrU8eDkSefkIkYjLF2ag8EgyM/XGDcukUWLnN36o0ffRY8eZct9fbPo338B27cn4+PjxsqVzxAcfHv2SlSvXp2+ffsyaNCg8q7KHclkMlGzZs3yrobuJrZp0yYAWre+iqlTdbobQL//eA34+fnRokULPvnkE1di+NKoVgle7eVsIF+sM6HcTQD18OUF6hNGBTLI5hT+JHuGobkBQQLp2w/irGBXwZECgXfDXhMsO4y9a29SchVyHYJctwASrYLdBbDlrIW9837jsA12WuCwBY6dziTZJsmzS7JUiTUrD4dDomkCNT0bR4GCPQ3nQEAboPpCngRNgBU4fQryTsOpTZD8M5j3ITUVD8tpwI0AzCiAERUPbEg0DKhonGQ5R8klF0WqfG2x8FB2Pn1OOXj4GKzPge2JkJQNHkaYtO2fYyQM4OMPJjc4kuxcNncZBIQAXuATAO5ezl7kiyUnS+6/38pTT9kYNMjGmTOSQYNCURSoW9cdd3eJw6Fht2scP24u9Xt6s9qz5zQmk0Jeno2UlNt3hr42bdrwyy+/YDAYLr/xHUIIMVkIkSaE2FvCNrFCiDghxD4hxNobWT/dneWdd97hnXfeKe9q3HJsNpWvvtrGhx+uJyvLUt7VuSPoPcjXyNixY1m6dCnPP/88W7duxWQyXVV5AZj4EOcMUBJJDlmksQsPUQ2rdGD390TJN2HITQGTAawq5APL1kGuBpg59X+/YrVLNCk5nXkGCeTgDCHG4eCsEBikxHpumV1zZngLtqkUOASKDQL8ffAzWhGhoYja1eDoFkCAjwkadod9y8ALOOuAHAmNgVwJdjNC5CE0T7zzzxDgNZJDYhE2LCgoCCzYUcgjmw0cx4gPdhT2mxthV1Wkr4WquT58lQLfV4EQL0jPh8cumPSqS3NY1w5OnIIPnncue6E3vPEp1K0Plf2hb3eoWKHo8T12TMNsdo4YnjpVZflyG1995cmBA40ASEmxkpJixWQSPPPMrT/BxKhR9/H555uIialOo0a3dm94cX7//XfWrFnDxx9/jKdn2SaEuY1NBb4Ffi5upRAiAPgO6CKlPCmEuP0+ILqbxoQJE8q7CrekefPiGTt2K5oG+fk2PvusQ3lX6banN5CvkaCgIMaPH0+vXr0YPXr0NbtClkh+ZDO7SSaWALw5jK/Mx2i2YEjOR9iWQbQb7A2EA2fBanY2gCU4snKR52blk4BFCDQpOT8mN9vNDWG14oUzYsOhKEghOKVpBBtNeAUGojzyCA4vdzzuqo2x/X3wSg8oyIPufWD9DJCB4JULmtkZn2wHAkIh4wzCx4jRz0xQXg6QQYR3L+KZj0IgJhwYUJGoeJJAOHdxFk8QDjTFiHRAkgNi3KGCD6wZCDlWCL1gwJ2HO3z5auHj9XB7uL+NM2SipPFZLVoodOigsHSpio+Pcwa/335z8MADzgub8HB3fv21yTV5D28G3bvXp3v3olPu3g7Onj3LSy+9RKVKlTAa9VPaxaSU64QQNUrYpA/wm5Ty5Lnt025EvXR3plsle8XNxs3NgHMYu8TNTT/P3Qj6Ub6GevbsSa9evVi6dCnDhg27qhH06Xb4Kh2CTVaOhKTgIzxYTjPacJYcxZPahgQqqVkIVTpTrBnywc3gzCShaWh2kO6e2B1mcnFGRWhSkg4IRUFzd0czO8Me3ADh7o7JzQ01Px9VSnIrVEC12zk7cyZ+vr6YvL2pFtEMr/9th7RUGPgoHDsCFfxBFkCQBj6A4T6QO5yBzd4OnLnhNDT1CKHSgxDRHht1OcM8cvE4Nx+JioVc6lGZv90l0qbiKPAm3B9W2cEmwcPk/CkNN7eiyzQNfpoFCcnw2tMQXlEwYYIbR48a6d27gPx8ydNP61+HW9GQIUNIT0/nzz//vOo7N3eouoBJCLEG5zyaX0kpL9Xb/CLwItxa2Qh0N4+1a50RPDExMeVck1vLI4/UxWy2k51tpV+/iMvvoLtqeovgGps0aRLe3t5XnV5qRCoszAaDcOcx/1Dy3dIJxYHADbMQnArsS6WKCqT+Do4KkJUCFSWE10E7G076jOUU5JtRcV5z5gEFJhOqlxde4eHkJCTgOLfOBvhXrYo9ORmvc/XW7HYc/v7Yjh4FqxUtJYWk7t0J7NuX4GYNUI7GO7td07OhogdkS8gCunSHvDhIwTkpyT3uYEkmyzCZbBmEFL6kUpEggonCyt9URcGdOlh5VlThiGc+p0wFpFRQsNiM1LV4Y+LKM0jY7LDjENQOh4qBsGIjfPYjqCokn4afRzu3q11bYetWbzQN3N1v7UwVd6KlS5cydepU3nnnHZo2bVre1blVGYFmQAec0wBtFkJskVIeunhDKeWPwI/gnGr6htZSd1sYMWIEQKlmodX9w2BQeOqp2+eu5q1AH6R3jfn5+WEwGEhPT2fx4sWX3d5mg+eeh3r1YerUf5afyYPTRyEjUdAyry3diMJMEKcJJJ8QzOI+lKpfQOA94BEPLc3g7gan0hAnl+PuoaEIUM6lJ7MANlUlqE4dPCtUwK9JE3KBbCDXYCArLQ1Zty5hAwZw10cfUeXpp1Fzc9GkJMNspkBVsWZmkjNtGrl/LHJWUgCKAXoMAe9AaBIDsS9CSA+weYDVF45lI1WJnz2LwJwUNC0DcKBgpBbu9KAFlQjBgoFprOIHvKglvQj0seEdYObtKnYk8N8D8OBG2JRZuvfh5W/gmc+g8zDnhCPubs7Z+CTO0IwLmUzimjeOpZTs359JWlrBNS1X9w9N0xg8eDD169cvcaIe3WUlAUuklPlSygxgHRBZznXS3aYmT57M5MmTy7saOt1l6T3I18mQIUOYN28ee/bsoXbt2pfcbu9eWL/eOUXymC+gXz/n8sxT4CdBWCT/yckjPOAANckjRDGg4c4JDtPGvAFsc8DrXHLi3AwwC4SHxC8crBZIM8NZ1dktZNQ0TG5udFu9mkUvv8zxbdvQAFVVEQ4Hprw86r33Hr7h4UhNI+O335wJK3CO/5NSIvLz0Wo1gCM7IDMVajUEnzrwwRaoWguyT4PNHdxDzjWgbeCloqgaPjYLFkcu0tQFb+GFpDYbWMlp/HDgTwGCA5wiRIShSPBRoIoi+Oss/N9JZ3FDdsOW9pc//n8dcuaXzrfAyTRo1xzGDIPEVHj6kat4Y0tpzJgdTJiwGw8PIwsWdKdWrYDr/6R3GEVRWLBgAfn5+Tc0kf9t6HfgWyGEEWfEVQtgbPlWSXe7qlWrVnlXQacrFb0H+Tr55JNPMJlMDBgwAE3TLrldrVoQHAQWC8ReEJLVPBj8DWA0ShK97ORrPiTiT770xIaVLLI4Ir/CYVRcg/LOpyRGEQhvqBAGuUgc5xYbgKxjx9j+4YekxsW55vxACKQQSCk5uXQpp7ZtQygKhqAgZ/Auzg+KBtitVnL/9z/yk7Ow2zzQDu2G9wfAw43gx//AR7Gw9A/I8IVmH0LtF8FqREgQqsRD+FBHDKQej5PManw4Rui53BreuNGYMD4z+PGuwZfvjP40VkxU9ACTApqE2t6XP/Yb48E7GMzA/c3Ax8s5lXeuBqdtUGAr5Zt4FVatSsRgUCgocLB3bym7vW9ikyfv5JFHZrJkyZHyrgoAmZnOY1q3bl3uvvvucq7NzU38P3vnHSZFlf3v91ZV5+nuyTPMEAckC4JEQUVMyCKKAcFdIwZcXNOa4/4wK7AihhUURfy6oBhQFlAEMZFEVJAMQxiYYXLuWFX390ehgqIMcQj1Pk8/DF23bp2qGopzT53zOUL8F1gItBJCbBNCDBNCDBdCDAeQUq4GZgPLgSXAq1LKP5SEs7E5ED777DM+++yz+jbDxmaviMPdZ/xA6dKli1y6dGl9m1EnJkyYwA033MB//vMfbrzxxj8cV1UFeXnQujX8LN9qmLCoFKqcca5wVCLRaaGVM9A5Dw2d1nxJuoTU8tU0zN+O56cw5KuwyoUsqYZtJsShplTjm5CfeHk5BlAqBIbLhd60KcVr14KUJJ9wAtHiYmQshktKXE4nHYcNo3jKFNSCAhxSEhACISVOIFETpLklbgcoQRAeBRQT0gPgDEO2BI8JzbvAhWdBxZtILYJMvRCR+TRCJLOCKWzkE2LEcNOW0/gHPnw42LN+7bpqWFsDZ6RBwh7ee0gJn6yCijA8/jZE4pZDne2H7SXQPA025lrtp7u3gXfr3s9lv5gzZwt33DGfnJxEJk/uRyBQ9w6LRxrbtlXRp88bqKpASli9egSqWn9r61AoRMeOHRkwYAD//vfRE+gUQnwnpexS33YcLI6mZ7HNkUOfPn0AOwfZpv6o67PYTrE4hFx33XVMmTKFu+66i/79+9OoUaM9jgsEoF273b9TFeiVBuBgjhlksRlniJJGEU7Ws5EsqomIHyhL7kB24v/A8zkUToQOMcSHucjqchAmSrlGtqaRn5BAbU0NXimpjEaRtbW4g0GklMSqqohWVoKUmIAzEmH9+PEQieBSFDymicPjISkUQgWkKYnFBPGYxOsWOB07F1mqA2TUSqtwC9jxI+QNhpwbEaoPkTEChBOJSZTVxKkABM1pRiKBP72WLf3W54+YvQpGTAFDgmZYxXgOFbYUQbIfVmwGj4SaWpj5DZx7K3zwNHgP0Zv5s89uwooVVx2ayQ8zgYALr9dBTU2M7OwAilK/xYyPPPIIGzZsYODAgfVqh42Nzb4zefLk+jbhuCMWMygvD5Oe7kMIuxi9rtgO8iFECMGECRN48MEHce5Je6yONIg6ENscrE6EnmnNaUlzTM6ggmW4yMCrNIXIHWAsAk1CcxPhFcifFEIlUZJSgxRWRNE0jQpdR5USioowhECPRNArK3/RidA0DVXTUF0uFI8HystRHQ7CkQh+jwcnoDg1pKaAlBiNs8ARglgEikqhSZLVYS+pGjQXlG6G3s9ZxXw7KeMt3MygIYIaGuDmwKS5YjqM+hK21AAxyEyAR86HU1rCS/+DmUvhhr9Ap8Zw41NQHYfPlsLwZ+FNu7ZrrwQCLj78cAhLl+bTp0/Ten3ALlmyhDFjxnDDDTdwxhl1SEa3sbE5ovijQJHNoaGqKsrAgf9l69ZKrrnmJB56yJbXqyu2g3yIycnJ4e233z6gOa5dBD9VgluF2WdATgIoOEim+6+DzDIrdKoC6SrENEh0kdSgBiFKCDRL4kctndDmzcTCYYxAAKW8HJeqohsGCIEnJYV+o0dTvmIFRkUFsW3bYOtWjNxcFKcTGY8TdTpR0zMI+twQiaLefBdMegakCe6g1aEjXAk7DHBXwbf/gUAqnPnIL6ZGWRFjlE0AACAASURBVI+GhwQqceEjmwNzdL7eDD/uAHNnsnXIgNQUaN8YXrrJSqNWLH+e55rBF8uscR/MB/MB2FEEXyyAVT9B29Yw5FJL8cLmV3JyksjJSapXG6LRKNdeey1ZWVk8++yz9WqLjY3N/jF79mwA+vXrV8+WHB+sXl3M9u1V+HwOpk1bbTvI+4DtIB8mNm7cyB133MH48ePJyMjYp32r4qAKK6c2pP/BoMzukL/USm9opENUQbRvjrqlAKor8UdKaBPScfh8bE5LIy4lyaEQsVAI4XLRcsQIXEKw9vXXqVq/HkwTt2HgdTpxNGtG80GDqHjmGWQkQmhjLu6VK3E1bIiIhCElCdLSYf0CmPwQJER36soBXgMKlkHNdkjIhuhnZIY+wecIU+07i6C4Cq0OEWRTWsWGzj14rh9ugIoooILYWXnYseGv23+WpH7wTcitAuEHJQSZKVBdA3+5AtatBD0CDRtAVgM4/dR9uEE2h4W1a9dSWFjIpEmTCAT+PCXHxsbmyOSpp54CbAf5cHHiiRmccEIKq1eXcOut3fe+g80v2A7yYSIWizF79mxuvvlm3n333b2Oz9sGC5ZAz27wn27w4jromQrt/0gtzD8A0j6AyGbIE+DUIXUdwu1CFocBSHFUINJb0PKuB/nhiSfYEI3i9XjQEhPZPHkykeLiX6ZzOBw4PB7iZWWYFRUUfv45UtdRAbcQFD3+OJkXX4h2z01WekbvPoh+54D+m6LPhEQQ6+GD06Hj7dDoLRSzkmDUIOpyst7xAAouGnAnSZyIk98nGpdIk79GqyiQJo86fFyg7V7wll8LGelQWgZNEuD1y6yivN/yvyUQ9EE0CZLT4YYBUFEFm/IsxQvpsIojbY5MOnToQG5uLn7/nySj29jYHNFMmTKlvk04rvB6HcyYcTnhcByfb/9TPY9HbJm3w0SbNm3417/+xbRp03jvvff+dGwsBoOugHtHwqC/wQkeeLkbXPln8pHu0yBtFoSyAT94AU82nBRD/LwMEgJngqTk1ltJ2bCBoMeDOxTCU11NrKxst+mkruNMTMSZlIQzJYXyxYuRqmopyfn9hGfNIvq3wcjiYsziYpgxDZ69F/JiVvcRgMQ06DoUyspAaLDpA1DbAQYIF6XKGgwKiLGBlTzOV/w/dCJsZAf/YykFlAOw2IizXRrEkYzTf99445FT4aRsuP5U+OGfcEqzPV+ivw+wdJEjEYjE4MUPwBDg81g61Al+uPYa6NJZMmSITtu2cT74wNjzZHth06ZKbr55LmPHLsM0jy6lmCMNXdd54403MAzDdo5tbI5yMjMzyczMrG8zjisURdjO8X5wSB1kIUQ/IcRaIcQGIcS9e9jeRAgxVwixXAgxXwjRcE/zHCvceeeddO7cmREjRvyi47onolErsul0QGU1RKK/H7NZ6jylVzPHiAAgMVnrmMlXbdqwsVt3zOTTkOVlkKpCpwDC64IGjQnl5kNtDRqS5Hgcl8OBQ9PweTy/zK0AiqYhfD4yzjmHhJwcEjMzQQiEw4G/Vy/8LqeV9mAAEqRTQqjGmqBGQLkD+t8MP8yAbRVQVAbthoP/RfCPh+As3OrJgImBQCNMlApKKGQic/mClYznU0wkHRWVmDApVOJ8T5TEHTX0zjfYsTNafWI6fDwYRp8Fnl2yNaoj8M1GqLQC6NxwHqx/1Uq/MAwrXdrrhkfvhsx06HcG3H0LfPutZOlSiZTw7LP7F1K+++4vmTEjl+ef/5758/P2aw4bi1GjRnHNNdcwd+7c+jbFxsbmAPn444/5+OOP69sMm+MI05SMHbuI226bTV5e5d532MkhS7EQQqjAi8DZWK1MvxVCfCSlXLXLsFHAm1LKSUKIvsCTwBWHyqb6xuFwMHHiRLp06cLjjz/OmDFj9jjO74dRI+HNKXD5JRDcQ7rlCL2SrdLgHSLkKBpZopjtzMRQI2xJjeE6PY/ElEb45pQiTpYwaCBk98d787VEojVICQFvAjWFhegVFaQEgygJCRi1tQiPh9QePTjxlltIbt2albfdRjgQIOPccxGbNhHdvh0qKvGakpguMBSJU3hRspsAZWAUW7rIrz5hVRQGU6HReZCQBqvHQNZfILExDbiKGn6gjEIMDALU4iEFicQAthLlH8xni6LR0OmhTG+AjorpD7OoyMMzFTAm1eoWeNFc2BGG57rDgMZWYd7F42FTKWQGYO6t4NQsnem3H4aZi6BLKysP+dqh8NeL4OvFsDkPWrUS+P1QXQ19++7fGjIYdGGalhPu99sr9/1lzZo1/Otf/+Liiy/mnHPOqW9zbGxsDpDRo0cDcP7559ezJTbHC3PmbGTs2MUYhklRUW2d9zuUOcjdgA1SylwAIcQU4AJgVwe5LXD7zp8/Bz48hPYcEXTs2JGPPvqI00477U/HXfgX6/NnGIbANBVwgJNkFDRMJG5CxIWktE0hntDlqJEgpPdGTLiBhJPB0yaNqsyz0d+dQQagS0msooIQoKsqJ1x+Oc2vu47FV16JWVWFZhig62x96y3SpEQAcUXBG0zCo0dRnBrCrUBpNdx+D7z/BNSUAyoYSSDKYNUk2PYqNEiGbS9D6ytwpl9OhjuAj++ppDUR4gTwcgV9mMoyKoiwHAMwUYSJX0QoN31IwAFEkcRNwV3LYU0VJDvhlbWWgxzRYX0x+JyQX2k1EEnf+Xa+YTrcsIuErpRwzW0w72sIeOGDSYK5czUKCqBNm/27z2PGnM60aetp2jRA167268T9wTAMhg0bhs/n44UXXqhvc2xsbA4C06ZNq28TbI4zEhKcCGE1ugoG696061A6yNnAru+WtwG/LaH8EbgYGAsMAvxCiBQp5W75B0KIG4AbABo3bnzIDD5cnHfeeQCEw2EMwyAhIWGf57jHDDJ4u0CRgk9TFM5P1mnOaEp5DRcfUiqTSJLlmK1fhmgQZcGniHgYEa5Ci1eS/NkkAgkaRUmwvhwEkIKlFqHGYqx//nni1dUI0yRWWoowTRQsYYqfY6pGNRhBP7K2GqfUUSPV8P47VrWbKsDnBi0G8TLrAJVAQhlkl0P5WGL8GzMrHYfqIiA2k8kYtrIUgzJa4WEbMTR0dJyowuQhJZWFUpJb6+IH1WRSucL72yWFJQKpQ1zC/U0t27xOuPMseH0BXNEN/E6YNB8SfXD+yb8qWwB8vgCmz4VoDKJx2JIH7VoLkpP38wZjaQdfe237/Z/AhhdeeIEFCxbw5ptv2jmLNjbHCKmpqfVtgs1xximnNOKll/qTl1fF4MHt+M9/6rbfoXSQ96Qk+9tqpTuBF4QQVwNfAtuB3wmZSSnHA+PBam96cM2sHyKRCCeffDKnnnoqr7zyyj7vXxLV8EqQSEZWxJnk3UK2O8JI7mILFcQpolSppLHxFWi10LYUNrWC5SGoAIwqcLtJ8oXwVwgqpEQCihAUTJuGqaqYkQhSSpASDfBg3RwV8GRlISvKEB4PRMJIRYJLhzWLwS0h1QPhcigpg4Y7dwLrt8KhgLsWzVDAqEBRNdx4iRDmO96khiqiJNGS5jSjK2sIcwmNuUANcq0K10idLzAx3Dq1ugqqBslQK0HdJZthxOnWB+D/vQsT54EiLBMGdv11XFEpBP1QXmlJvPW1Jd6OCLp06cKIESP429/+Vt+m2NjYHCTef/99AC666KJ6tsTmeEEIwbnnttjn/Q5lkd42YNeWOQ2B/F0HSCnzpZQXSSk7AQ/s/K7uGdRHMW63m/79+zN+/HjmzZu3z/uf7oVmDkmBARUOnZ8qG1BrVvAccykmhCAFQzgxEAgJJEZhaAxGfgPd20CqB9WtEGvagaZuQQs3uFUFISV6KIRRXY0QAs3nA8BUFBRFQQiBE9ALC6lpmoPz4ktx33objlN7WWFbVVj5D6EwhKUVNS4DNBUSgaiAcDMQoMVNUgpqwACTEAb3Y1CJiYFKJU7KKSEfL5XMZzXRnWunfl6BqlqpHqrPimyjWM36Hlll6Ub/lsqQlUphSqiJwI5SuP8/8MqHcP5ZcMXFMPQCmPWWpWhhU//06tWLF154wW6NamNzDPH888/z/PPP17cZNjZ75VBGkL8FThBCNMOKDA8BLt91gBAiFSiTUprAfcDEQ2jPEcfIkSOZPn061113HStWrMC30xmtCykafNYETi6OUyChBghQRQw/X3IO54lchPTwk28HXrOWprX5eJQSqFqBkMvh9GpEOILfaIqMOPBWShLyITeiE8daORlCEA2HEYqCIz0dzTDQIhGoqcHRqBEiGMQ3amehYSwKN/aHtYtB1Fph2ihW+7+cLqDlg6MAPEmwvRp8jSAYJ5zYEFPbAkgEDiQqKhoGJpIIXtYRpRUGJt9TSQ0mvd1JdHQK8nTJeU6FgR1h+HKry3aGGzzq76/XfRda0ePkBLi4h9Vyet4yy29vmglP33/At9PmIDFx4kSWL1/O008/jctV93wxGxubI5/p06fXtwmHhXjcYOXKYpo1SyQYtKMuRyOHLIIspdSBm4FPgNXAO1LKlUKIkUKIn0uk+gBrhRDrgAzg8UNlz5GI1+vltddeY9OmTTz44IN12ueTb+CxV2DTNuu1wdtJGsM9DqYHvLTX27JWD7CBbGbSmlWKhy+cvdjuzmRZUluqXQ70mvuRvhpwA4lxROF3KGoMZ0IMR8NEGqankggEgWAshkvXcUlJwwEDaPfuu7h79sTZvDlCCIK9elHUtSvlw4djbt2KHPMu3DcOHE6QAjQF0jIhtSuceDkEW1mJy7WFUBiBIi8+1xRcZkeiMoiQKXhJAuJoxPHgJAlJJ1I5iw48w0bGkcv7ylY+T3GwMM3Ja8kqFzaAH0+HlzvC9B5WBsfPLNgE7/xgaR2PuhLuvwhcDnC7+CXhx7n3Rn5/SllZlIqK2IFNYgPAtm3buP3221m+fDkOxwHeGBsbmyOOYDBIMBisbzMOOTfdNItLL32fc875L1VVe9BqtTniOaSd9KSUM4GZv/nu4V1+ngYc1yWtp512GjfddBOLFy8mHo//qVOwfgvc/CTE4jBvCcx7DVo7FB5xKPy7yuCV8oZUkU7XtPXUOEoQQLXwkytzaCXWUeLKIDt9Bzg8yFgIgUD4VVBABv3IuBcZdKEVFCEBISUKIB0OXMnJxEtLqVm7Fr2wEE3TCEyahFpRQfy7pTj+Ox5vShA+mIsYPQumjITcBRAJwYlnQ7tu8O47lqizX4BZAnEwov/Eoy7AJZzEFDeaWkgQN2EqiJFHFicylN7MIJ84UUxUSojiUwQ+BQwJS2ohLwLdkiBhl9/oJVvgqrchblqO8nODft321E3QtqmlaNGn8/7fv6++Kua665YghODNN7vTrVvK/k92nCOl5KabbiIejzNhwgQUxe5jZGNzrDF16lQALrvssnq25NDy9dfbcLlUSktDbNlSyYknpte3SfvFli2VzJmzmZ49s2nX7vgqsLRbTR8BjB49GqfTiaruITdgF6Tkl6jnb1sifxMFNyoxqZEUS+MSrZK1wo9CjFKRSSlx2ssNxDLdmH0krsUuBBo07gAtWqI0P4FA685ErroLHxABHB4PZteuONPSaHrLLRROnYpeUoIMh9EVhUhNDV5pGRQOSbyOSnhnMlw4AEo3QkYOREOQ0xlKV0BtvnUCAcDpAqMcJX8G5GgIJUREVuInj0KS0XEBKsm4+I4dvM+P1KChodGEDEwpeTEa47Uqk3V5Loy4gtOExFq4tRnc2QJKai0HGiC/avfrleiHWwYf2H0DmDkzn1jMxDTh00932A7yAfD2228zY8YMxowZQ/PmzevbHBsbm0PAyy+/DBz7DvI99/Rk1KhFnH12Dm3bHp2OpWlKLr10Ojt21OL3O/nmm7+SmHj8pIsIKY8uUYguXbrIpUuX1rcZh4Ti4mLmz5/PpZde+odjZnwBi1fA1RdA811KIBdFJbeWG8QwqXZG8SuChwMLyVW+RyA5l760kpWEzX8ADpTqTfhWuwABtbfA7PFQVIpRIyj8wiRWo5P0j5sJPDsGGY2iuN3ESktZdsopRNatQwhBmqYRiFsVcW4npPiBFA8iywVJBiQFIJAEj38DsWJ4+0QwotDAAYkJIMuQaRIjoBBNT2atLwtTQAwH6zmRKBrncStziTObfArR8OHgZFI5M96WG2vDbI1DZLMPoStgQNM4OE1YdSbEDXjiM8gthYfOhhZpVgORyXOgtBKu+wsE/iDtW0p45x1YuRKuvx4aNdrzuGXLyrjyysUoiuDtt3vQvn3ift374514PE5OTg4NGzbk66+/3uti8WhECPGdlLJLfdtxsDiWn8U2h45QKARYKYY2Rza6btK+/UR03UAIwVdfXU5m5h/L0i5YkM/33xcyaNAJZGXtu3zt4aKuz2I7gnwEMXLkSF5++WVatGhBp06d9jhmwOnW57f0cAkWZ2qcV1XL1qggLw6jKrozLikVn/DQklZADQotMVmHo8gJRgUIBTbPguLtEJaoTjdZnTUIdkLecx87enTHWLkK99ChJL/4IsmnnkrRjh04QiGiQhD2ePBnpJEkqqCqAhEKW72dhQe8xVAThncfguQCUPyguKDFw5AWhOIR4JKouge3ax6auBODKC4UskilCWfRiPacQQXLKCSMQjIehtCEWiAsJV4VlOQ4vnIXNWHYVAtddqa3OVR45Fzr55/XgR8vhH+9YUXgC8rg2eG7X8eXX4F/j4XGjWDNSksvefly+PAPWth07pzM999bB3E47JSA/cXhcDB37lyEEMekc2xjY2NhO8ZHD5qm8Oqr/Zg4cTkDB7b4U+d406ZKrr56NuGwzvTpuXz66cW7bS8tDbNxYwUnnZSO03l0PONtB/kIYuTIkUybNo1rr72WJUuW7DEfee5cuO12aN4c3pwEHq8VDc1Ihi8LYPUCN5XdInhdUGBomGYbPlF3sIYiBop0fOp0pDQRvjsh4U1wuEBbD8nSUp2IRMDnBzUPObA9yRuKiUpB6M3XWbVoEbF163AKgabrSKAaUEIR0hMkQgBOLAULPWyJJteWww//gx6NQPVYTnJGL8g4CcJ3IRxlIHTU6HpOcLxEGZ8QoBt+rMVdHtsoo4SnOI0dSJ5kDS+RS5JsjurQ8UnB5CaCNg3g9G/AnwA7ohAxLAENgH++A1OXQo9sWLEaiiKQ5Px9mgrA6H+DqcP8eYCEYNBqF/1n2I7xgVFQUEBmZiYtW7asb1NsbGwOMW+99RbAEaNvHgrFmTFjHU2bJtKtW3Z9m3PE0bt3Q3r3brjXcZGIjmlKNE2hpmb3ovXy8gjnnPMOlZVRevduyBtv9D9U5h5UbAf5CCIpKYmXXnqJiy66iGeeeYYHHnjgd2NGj4ZYzIpqfjIHJnwJG7bD4L6wKgecukpCgYarscFpboWpymZWUY2GQiPcdCaIEApkjgRXU1D94P+71ePwR2CrBhUhqK6FKhMzBpqQ+DSDolUr0UxLf/jnxBwByOJi4h4/LgdWfrEiII4lOuyQENoE66uhRQvI6gFpHaDqfRBlSAXAgOo78STkks7fKOdbFDazlXJmMR0dD2tYyw46U0YMA8kGGcKlOkFKthkm/94AxSbUROHiTHDt9FnnrYXnv7AiwR8vghSn1XEvIQHu3pkCF43ClOng9cBpveGjj0BVIBCAli3heJHs1HWTb77ZSnZ2gBYtDqCN4D5QVlZG586dufrqq3nyyScPyzFtbGzqj1dffRU4chzkf/7zE2bP3oimKbz33mA6dMiob5N2wzQlFRURkpLcR7QmfJs2KTz6aC8WLMhn+PAOu23Ly6uisjKKy6WyZElBPVm479ihryOMQYMGMXjwYEaOHMmqVat+t/2MM8AwwOuFhFTIzQe/F96fD6c3sHzSrC0uPnV7eD3goiTsZWt5KjFdxbnr7VYTIPUWSLoGss6zdM9aK1Z+QoIbNA8iLBAChLAcTKcpUbGa4ilYzrFfUXB4PYjkdHD5+KVjhycADRtD0GU1DomWQvkSWP0CfH4paFlIc5cIuShESoNVjGQjL7GUB/mSd5CUoVBMiBAdCaIicKJwq8NFJ6ERjmo8vE3lh7CkaTJkp1hyb0JAVQQ+/gkcmhUtdvugstZy7mvC8N0G69DPvQoPPwt3PQqNmsMjD8NZZ0HHjvD665CVdeD3NRYzyM2twNhT2HofKC0N8d57a9i4sfyX76SUzJmTy+TJKwiF9tAlpY48+OA8hg37iAED3mbNmpIDsrOu3HHHHZSUlBzzBTv1iRBiohCiSAjx0x9s7yOEqBRC/LDz8/CextnYHAzmzJnDnDlz6tuMX9i2rRqQmKakuLi2vs3ZjcLCWs4//0NOPvn/uP/+r+vbnL0ydGhrxo3r+zu1i3btUvnLX3JwOFQefLBnPVm379gR5COQcePG4fP5SE7ePYoXi0n69o3Qu7eT5s1Vgolw4iz4YR1cNxDu6ADnNoIUNzTwCtZF4cvtjaiQBsk1WbRv5MLEZC5rKCNEP9oRxAPdp8KmSyC6BAxg0EvwwquI2Oc4k3XMMISKQA0pGKbl4ClYbalTnn4aT0UhjhnvgjcBQkBqIlx7L7RtBK8NsbzTgLDynSVQsgzcncF3JuifgMOF6ToBnc1EyEcnRBSdCNVWtzx0BtCfDNJpQQIOFBoobkxpsjhkkuCEQgERCddmWgFs04SL/g82FIPLDW2T4JUhMPYd+PxH8DqgUZp1XatrrBzlUAheGg8BJzz2/2DokH27b6YpkVKiqruvO+Nxg0GDPmLNmjJ69mzA5Mnn7XckYMiQD9i4sRyfz8kXX1xBcrKHr77K46abZhGPm3z//Q7GjDl7v+ZevrzwF3tzc8tp3frQVl7PmjWLSZMm8cADD3DSSScd0mMd57wBvAC8+SdjvpJSDjg85tgczxxp+uZPP30Wjz/+FW3apNKnT9P6NucXPvxwPbfc8jmFhSGaNw8ydepannii9xEdRf4jVFVh7Niz6tuMfcZ2kI9A0tPTmTjx900Fb7yxgK++CpGcrDJnTmNcTpX3noBw1GqEAdB+F5+62gSBICA0VMO61T+ynf/xEyaSKiJcT290xaDGa+I3PKiqgJQgXNgVkhahrJYo22tJ8CuEsppTu24LsbiVf+xNDCJnfITSuQOitARcLhhyLQy6FNKTYUwv0CM72/IFLE9VNaH9rWCsQrAeqTUFDAoSs4mLK4njxCBGiAAmBqBhItlELhlk0JhfCzy6OAXJKpQCT7c2Od+lkuW0toV1yC2zguFqKsy8CdIT4NXb4fMfIDsV2jezxt5xgxWVX7oU1nwP8Tis37Bv92zVqkqGDv0a05S89VYvOnZM+mVbYWGI1avLCAadfPXVdiIRHY9n3/+TkFKSl1eFw6EQDutUVERITvZQURHB2KlnV1YW3ud5f+Zf/+rDvfd+RqtWKfTt22y/56kLVVVV3HjjjbRp04aHHnrokB7reEdK+aUQoml922FjA/DGG28AcPXVV9erHT/Ttm0a//d/F9W3Gb9jypR1uFwqqiooLo5w3XXtD6tzXFoaxjQhLc1z2I55pGE7yEcwmzZtYvjw4bz44ou0aNGChQvDuN2CsjKDvLw4waDKjh3wxFOQmQGdekJ+MVzWHwJ+6OyGe1LguwjcslOeV9slzcKJSpQQc7mJeKZBICmb7lVtcFX9gLLpLUS6CwK18H0iSpGDjIr1yBNVwpUplOeV46ksg4VfE1r8NVpAQXFqcPGVkOqFpy8AvdLKwzCBsAqnPwUFU8CfAlpTUBIQZg26qxu62EYMJyYhQMVNBDcKtYCDFBbyDd3pgUBQg8FSammuuvgqw0mNCSnq7g8OnxPuOhVe/w6uPtlyjsHqmndu192vc3ISPHk/FBbC7f+0osnXD9u3e/Xee1upqIihKIKpU7fs5iBnZSVwzjmNmTVrM1dc0Wa/nGOwOieOG3cuL7ywlH79mpOTYx3jvPOas3JlJ/Lyqrjvvl77NTdAt27ZzJt31X7vvy+sXbuWWCzGxIkT7XbSRwY9hRA/AvnAnVLKlXsaJIS4AbgBoHHjxofRPJtjhSPNQT4YhEJxvv02n1atUv5U6WFfuPLKtnz3XSGtWyfzxhvncuKJaQdl3rqwcGEB11zzGVLCK6+cQZ8+ey/SOxaxdZCPYLZv307btm3p1KkT8+bNY/LkKp59tpQ+fbyMHZuJqgpuvAlmfQJxHcxEcCXCeafDK4/ueU6JZAmbqSBEOzJ5nf/SkjkITJzodI5vxF1VS+qsEkSVgcADZXH4LGYV5pkSWSrQt0lCEcuZ9AXA4QAhgfFvWd7opNtBFIASsZQtulwOqYtBOMCMQZ+FoEnQc5HODhSJB6lgEWV4MZCE8VJBDkU0JoagMY25GEsf+lY2s5IwLhTeIIc06v+V3cKFxVx99UKkhAkTunP66b8v9NB1E02z0/5/JhKJ4HYfR6Lz9aiDvDOCPENK2X4P2wKAKaWsEUL0B8ZKKU/Y25zH07PYxubPuOyy9/nuux34/U7mzfsrSUkHJ+oaCsVxOBQcjsMri/bYY0uYMGEVigJDhrTkySdPOazHP9TYOsjHANnZ2YwePZrrr7+e8ePHM3z4cK66avdGFKmpVkEaWLVxAJXV1p81EfjrBPhsNTTNghl/h2bJgu5Yr8+/5ieq0CggkyTKKMdDrlpOdlIM49wUMhZWIlxRSMqGBYWI2jBSEQhfACEq8bhAlzud45+r9p78O3TtA+37Qv4XQK5lzPaFkJ0Nxjrw1UDhWGj0GLgyEEAG/yYdSQXfESGfVPqg4CVGlDx2UEGUbZTSgCS2EENBEENSir5XB1lKWJEHtSGoCUHjFBg1CRpmwH3XWlHlA6VnzzQWLDgX05Skpe3Z6bOdY6tJwKRJk7jhhhuOK+f4SEZKWbXLzzOFEC8JIVKllIenUtPG5ihn+fIinE6F6uoYBQU1B81B9nrrJ/hz0UUtePfdDZimZMiQva6Vj1lsB/kIZ9iwYUyZMoW7776bFusvRQAAIABJREFU/v37/+615oP3Q7u2VgT5wWegugAu7G1tm7saPvkJonFYvQlGzYUXd2nSl0MDfPjYRGuibEJDZ6VoT5KswR30QgMVdNOK+rZJgi0RhBfY7ERpokKFgfvnwjvDtNQq9GpY8DHUNoOzL4CV4yxh4dp8aPkW5F8CajaUTYW0q8DTEoNatjMaSYxM/k4SXZBI5jGd5SxnMwkYKJiopNGc1jTnOwwGkExD08VS3aS1JkhQ9pyfNXY2PDfLagySroHbgHiZtbDo2BIuPKPu96OqysDhEHg8v3d2U1LsVIG98dBDDzFmzBg6depEjx496tscG0AIkQkUSimlEKIbVtVAaT2bZXOMMmHCBACuv/76erbk4PHYY30YNWoRZ57Z9JAXN9eFcFjnmWe+JxTSueeeTiQn71swom3bZL7/fugei86PJ47fMz9KEEIwYcIEDMPg0Ud/nzfh8cDlQy0fVKmGVAEzP7K2nZBuBXWteeC3/lsWKdzDYDrTFFAwcCBFEKmcSBEpRLQQ0uGGRmeAV4PGEhpKOLkCtamKo52K2igZ4RaQBKQBigSnBFWDn1ZBk65W8V5SEDbNAkcK6MWg+JCOZKJyI2vpSylTKOYDvmMg8/gHS3iZtfxANU4MTHQATPKoYhU7cBHCI3UGl+sMLY8zoCzOhohE30PG0FdrrCI809zZu2SnEpqqWPWIdeXTT6vp0mU93buvZ+3aSN13tAFg0aJFPPfcc9x44422c3wYEUL8F1gItBJCbBNCDBNCDBdC/NxH8hLgp505yM8DQ+TRlntnc9QwdepUpk6dWt9mHFQuvrg1CxdezWOP9UH5g0DN4eTtt9fz2mtr+O9/NzBq1A/7NYeiiOPaOQY7gnxU0KxZM2bPnk3nzp3Jzw8ze3YBnTsncdJJvxaC9ewJfr/VCG/QIOu7ttnw3gi4Zxq0yoR7zv393B5cnM+ZTMdAUsHZ9GUbd6M601jV7hTaRq/A6TsVrYeEha8CEhy61YlDSrjofHjnfdCrLOdYCOu3qnIznHM1dO0Gc2+yDhZUwSwEZwjdbxAWp1EpVSRRTGH9KhpIYiynhgiZ5FCNjhuVCAo6frx4MHFhoDBPShbqBllCYWlEcmYedPHAu60sqbefufMv8I9J4NEgwwUPXAoVZVb3wVM71/0+vPtuBaYJ5eUG8+fX0qqVnSJQV6LRKMOGDSM7O5tnnnmmvs05rpBSDt3L9hewZOBsbA45n332WX2bcMzj9ztQFIGUksRE+83m/mI7yEcJp556KgD9+s0iN7cMvz+J+fPPIDPTynVq3RoWfGM5yOnpv+7Xv4P1+TOSCXANl+zyzWC28S4BZwcKna9j8gKpp15McFWm1TpaCwKV4HfCCW3hgmr49GMIx63+ztl+SPCCHoImZ0LnqyDvIwhvAm85IFH0dQg9B4cjiooLHYUIXmI40FGIE6IPl9IdN1VESCaJyWxkBSW0xiBGQxYoJgneWspCPrRaB8kCltVCSRzSnb+eTc+WsPTxA78HQ4YkMnduDTU1JosW1XDFFUl4vcf3CruuPPbYY6xatYqZM2cSCATq2xwbGxubY5ZLLmmOpimEQnEGD25R3+YctdgO8lGErussXToCRcnE7b6fUMjYbXsgYH1+y5cL4amxcEpXuP92qyven9GIwTRiMFX8j2K+RCIpDXyMc8RzeFY9CjIALiD/W1jxFBR4obEHIgLcQSAKTje07g2RYtjwGugVsOY76KhZ6RqqC4mBVybhF0+xig8IsxoTgyheXAT4iSJmMw8FlXM4l58ow4+LQqrpgZtFhGjgD3GG4mVKjUquCkMSJGmOQ/OK68wz/fTp42Xu3Ermzavmww8ruPzyw9OS+WinX79+CCE477zz6tsUGxubeuSll14C4O9//3s9W3LsoiiCiy7KqW8zjnpsB/koQtM0hg27ghdfHMmAAVvIyamb3uI/H4bKKli3EfqfBZ071u14XrqhkkaEn1DwUVN9C25XiZXX7PJChgS9HBLiEPGBIcHth0ufhA59Ia0JGFFwp0NFHrgcYLrAK1AUD17jdnRnL6RII8IUIriQSAR+mnE2M1mGBEwMVrGKDrTmG8opx8dXbGY4OaRKF3eVeigTEPHABgGPrYOz06BHMqwqgMc+hVZpUJ0Pi9bAA5fBeb/RQo5EoLISMn6vzrYbOTlO5s9XUBTIzKx/ebmjhV69etGr1/5rNNvY2BwbfPzxx4DtINsc+dg6yEcZuq7To0cPtm7dyurVq0lJSdnrPkNvgCXLrFq5OdMgu0Hdj2disJn+SGpJzl+LaoZwxCXur7IRW3MBCc36Q2U+NOoGcSesfge8iXDeaGj9FwgXwtJeEN8MXjc0SUQqCpUJDSnzwQ5cRFGIYlBJEim05kye4BM+5wsWoAMtOIlh9OdBVrOeWnQkN9KU/mTQd7vkyzA4hCWikVki8ApYeCpc+TqsLIB4LchC8LvA54bvxv16jiUlMOACKC6Gf4yA8/pJ5s416dtXoaZGp6zM5MwznaiqIB6XzJpVSVKSxqmnHhxB+GOZp556ioKCAkaPHo2mHd/r8frUQT4UHO/PYhub+sQ0JYsWlZKa6qJlS399m3NUUddnsZ1AeZShaRoTJ06kvLyc2267rU77TBgDzz0O09/cN+cYQEEli3+TQD9iGadTnZFMecN0ogPvgkYpkNMACj6BquXw06vw0/9BpAxK18J/B8HmuWCUgVkKQTe4IshqlYgnTNi7FhMTgwgKThQMJIJEmiAQnMsZOGmCgyZsppx8SrmQBphAAU5GUsILFPJuBvR1QHIMglGBKi3lOVNCo52y0U43eF2Wat2JTXc/xx+XQ2kpuN3wzjTJpZfqPPWUSf/+cS67rJKbbqpi1KhaABwOwcCBibZzXAdWr17NI488Qn5+/nHvHNvY2NgcTEaNWsMVVyzi/PO/5Pvvy+vbnL2yZUs169ZV1LcZ+4T9v9ZRSIcOHbj//vv59NNPCYVCeL3ePx2fkADn70HBoq4UEOQrWtFZ/YFENQ1Qkd5kSA1CfAtoOiQCBkA5hCSEgbiAFa9BRjmYcRC1oCQj9SIqfW7CwoNgG6l0YweJlBBDw8sJnA+AQNCQTHLZgRONRHw0xktPsniTEhTivEUpV2upfNJYJSxhXTVM3Q790iHVBaMHQd+W0DQZsnywPh96tN79/LqcDA0bwpYt8I+bYcwoq/lJKASaJlFVWLdu93xvmz/HMAyGDRtGQkICL7xgCyTY2NhYjB07FoBbb721ni05ulm2rBwpIRo1Wb++mk6dkva+Uz3x9dcFXHvt55im5KmnenDJJc3r26Q6YTvIRykPPvggDz/8MKp6cFpQbi2He2dCwA3P/AXeiOu8Fjbpl7CDzd6FKOgU0oVLySKZdridg+CEeRAaD26stgIhLOFlH1bTkLgOqU0hvg5IgTigRTA8fuLCyjaWqHhxYtIKDwWY6JSzlSDZfMMaIsQ4jXZ0pyUBrIWAQKBhaRpnouJFQQjwCjgpaH1WVcLKSmgXhEs7WedYWQupifDbrp3BIMz9FKJR8HgELVsoTJkiGThQ8L//uSguNrnvPt9Buc7HC+PGjWPhwoVMnjyZjL0ldtvY2Bw3zJ07F7Ad5APl3nvbcMcdP9CwoYd+/fbx1fABsHZtFZWVcbp2TUaIuhXEf/ttEZGIjqoqfPPNDttBtjm0OBxWgVhxcTEfffQRw4YNO6D5np0P32y2UhPaNJHcl2UQR+IUW8iSoAqVIlLwcR0mccrJJzmxpRUlDgA1WCoWP+e0K0BQg7KnLVFi/4mQ2AzcuWhCEIy2o9CzGolGLTvIIodKtuPESyonUEYNM/gWgaCAcs7lpF9svZ4MTCQ6cAuZKOz+j3RmPtz6PdTq8I/mcG87qKiFfo9DWTX06wTjfnO5FMVqugLQt69K377WzwMG2JJk+0ooFOLxxx+nf//+/PWvf61vc2xsbI4gPvroo/o24ZjgpJOSmDdvH9rAHgQWLSrhyisXY5pw++0tGTGibm2oL7mkOTNmbCEU0rnuujaH2MqDh+0gH+WMGzeORx99lKZNm3LmmWfu9zzNU6zOcgLI8UtMACSF0QxS3SVIBEU0ZhmrKWc6ccI0Tz2RnvFsRNI2CHoheibk5ULlBjDCEIj9muUe2gypw6B2E0JoBLibYj4gwmoEPgwMmtGD1vTHQyLbKKWKMDqShiQhdnGCE9G4h4a/O4fvQ/D3PCgPQ1EMamPwzEroGITMOJRWg9sB81fu92WyqQNer5cFCxbg9XrrHGGwsbGxsTl4bN0aZv36Wnr1SsLtPjhvmteurSYSMVBVwbJldc97btQogblzBx4UGw4ntoN8lHPfffcxZcoUrr/+elasWIHPt3+pALf0hrYZkOCCU5oqvF6rMbpGx+lV2EEWLkxKgPksowXVSCJsUL7lhKRzSQt/iswUiIRh0LI9rHwUtAQofRWMkHWAhNaQNBKcHTFUJyH3T2RyDiZDySOP9Viv3Ry4MWnLB8wjgsBAo3qnu743xhVBQcwKZDsSQCsDpwlbauCsFnBqG1i0Hu69YL8ukU0d2Lx5M02aNOGEE+oWWbCxsTm+GDVqFAB33nlnPVty9FNWFufuu9ej65Knn25BRobVNS8/P0L//ksJhw1OOy2Z11/fS7ewOnL++VnMmlVAcXGUO+5odVDmPJKxVSyOcjweD6+++iqbNm3igQce2O95FAXOaQWnNLX+PtSnsjTDxTxnM3qLZEAjlQhlNELFj4JAI8Z8T4Svg6eQ61dZ63yRmDcBs5WKzJ4JTXPA6YOEltD1U6RwIBMupMI7i2oxnhLuJ8YmNLy/xIcNBJP5iAqq8FKNgiREHGMPTvI6GedLGUWXkgoDthqwLQylUbi4KSSZVnO/n8rB6YDXR8Dq5+CqPr8/f12HL76AjRvrdr3y8iJMm1ZEQUF03y/2MUpeXh4dOnTgscceq29TbGxsjlAWLlzIwoUL69uMY4LXX8/n009L+fzzMl5+edsv3+flhSkqilFUFGfhwoOnHJGc7GLKlFOYO/cM2rULHvB8BQUhHn54KW++uZ4jUXLYjiAfA5x22mmMGDGC559/nsGDB3PKKacctLndqDxPC4oI8z82sYokttOJ3iyikFl4RSr52kZipOKghCRjKB7PNwg3eIwoahsF1DBSrsKovR0pdxBLEOiihgguqngMQVfaMRQQZNADyXoUQEOSQgL9OAmN3V8RrZRxrpVlGEguwcuOUj/fRiwHW5HwRgnggYZO+HgTtBDQuzF0zd7zeT7wALz3HmgaTJ8OrXYujiMRk7ffrsbnE3Tv7uLjjyvp2NHDbbetpaJCJz3dwddfd0LTju+1ppSS4cOHYxiGnXd8CBBCNAKeBbKBWcCzUsr4zm0fSikvrE/7bGzqynvvvVffJhwzNGrkwuEQSClo0sT9y/eBgJN4XKDrkmj04KRXHAr++c/FfP31DhwOhSZNEjj99MNXbFgXbAf5GOHJJ59ESknz5ge/OlQgyMCLizS+k0UY1JLAaZwsCillPQ4kCiYmCoZYgQQQOnE3iJgJcgcy8iyIIuKKArIWhMBNjAiCAopwMZPO3EaAAOfTh0X8SBfacyY992jTFnTiSAQwW4+xImRSpSggJKYhiIUBH2wqg7QK+PdieGUZfHk1lJXAnS9CWhKMvQUC/5+9M4+zqf7/+PNz7jr7PsOYsYx9jWwJEUpFkdAilRQKIUuRfCsSUUnKUpK9Qgv9UIqi7KIhS3bDGLOvd+56Pr8/zthnZcYM7tNjHnPvuZ/zOe97zT3nfd6f9/v19oLoaG1ehwOOH7/oIH/4YQqzZ6ejKGA2Z5OZ6cJkEjgcTsxmQWKiA7tdcrvL/C5evJjVq1czbdo0oqLcLU5LgC+BFcBWoC/whxDiYSllElCpVC1z48ZNkYiNtfLJJyeJivKgb99IFEVbQ5VSIoQgM9PFd98lERFhpF07/zzn6dEjjJAQIy6XpF27wAvbg4IMhId7Y7Go1KjhUSw2SymZMOEkP/6YyEsvhdO3b/h1z2kwXKxR0enKXr3KbX5Zv3Xw8fHh008/LdFjeEsdyag4kfwsHQxiEBaRRCobOcFMXNhIEJXw0O8F1Qun2YnBmYUUTtJM6zGq5UHNQBVayZ0NPal4YccApHOEH2nMUNrQjDY0y9eWtphoh4mTuEjJ9CbQILHZJcIkyM4ElwtwgZ8RfA3ac5cKDhe8vwT2nQB5HFb9Bb3uh7fegtGjNce4bduLx8nMlEgpUVVBdrZ64Qs9dGgE69en0LdvOTw9y+4d+o3g3LlzDBkyhLvvvptBgwaVtjm3KiFSylk5jwcLIZ4GNgohHkETn3Hj5qZg0qRJALz++uulbEnpMXLkQTZtSsFgEERFedKuXRDDhx/n+++T6dUrhJQUJz/9lIzBoLBoUQ3uuiv3TnlCCO69N/Cq7aGhRpYvr8s//2TSoUPR9ZH/+iuTr75KoksXPzp31hz006dtzJ8fh9msMGHCSXr3LofReH0rp1OnNmf+/MNUqeJDy5ZlTw7U7SDfYpw6dYpnnnmGDz74gMaNGxfLnKk2eGMrJLsCcDbPwsdD5Qwm7OjwIQwfemAiiKN8SpYiyJA1MCm7UfXxpBkdWBUTUhFYSUWhFjZxlHRMZOGFHokRiUAhgBoF2uJEkoaLQKFjqtC++Gs9VF6xqjT2U5kaoUNWhncPQ0wqvFwDGprh1bUQ5KGpdNStAhv/0fKuq+Ss6DRvDuvXX328kSMDEAK8vRXatQth4cJk2rf34dFHAxg27GoljduRI0eO4OXlxdy5c4tNl9vNVRiEEGYppRVASrlICBEH/IymPO7GzU3Bnj17StuEUsfDQ4eUkJgIr756jDfeUPnhh2T8/XUsWpRA48ZeCCFQVUlamvOajlG7the1axf91OBwSPr2PYnTKfn990yaN/ciJMRAUJCBkBAjCQl26tTxuiz6e62EhHgwYkTxFBCWBKIkE6OFEA8AHwM64Asp5aQrXq8IzEfrw6YDXpdSrs5vziZNmsidO3eWkMU3P6mpqdSpU4eQkBB27NiB0Wi87jmnR8PUPQCSiBo2rM1SuR8TegR3YaSzojXwSOcgMZwkiAaEEUQSA7DKH5E5Im1C6NHREAsHSMYHGyYkOrIJxUBDWjIWA1oe1WHO8iv7qEsE1anCYk4Sgpn1qJzEQVf8GMrFO06XlCiQq6zY2sPw8k/gdMG9UTCvK2yKBj8v8DJAuRDwucEuhqpK3nprF3/8Ecfrr9/Bgw9G3lgDihmHw3FBm9tN7gghdkkpm1zjvsOAv6WUf1yxvRHwvpTyvuKwsSi4z8Vu3Fwbycl2xo8/xtdfJ+Hrq8ffX09wsAeHDmXTsKEXkydXYsqUM0RFmRk+vMINTT9wuSTNmh0kPt6Jr6+OzZtr4ueny7Hbwf79WTRq5IOX180bDCnsubjEIshCCB3wKXAfcBrYIYRYKaXcf8mwscC3UsqZQog6wGqgcknZdDvg7+/PzJkz6dq1K5MnT+bNN9+87jnDvcCggJSCZ33M9BNhPCgTOIfKz1iJkHBUxJNOIueIJpstVCScXnzMf+IAetIJJhkD5XHwIHruwY+/SSWTbKxIwrAQTypHCaEuAPPZiAMXJ0hAxcoRsrGgkoE3AXizmnSGyFBOqZJzTsGyTGhlgoe9INYKvyVBM3+o7Q2eBi1yjNAc4rnr4N9TYDsHv2zSuuutmQ2Bead6FTt79yazZMkx9HrB66/vuCkd5OTkZBYtWsTLL7/sdo5LGCnlR3ls3y2EcBfouXFTBvjjj3h+/fUcjz8eSb16Fy8oUkr+/DMNk0mhWTNfAgONjBhRhXXr0rFaVRo29OaTT6pz4oSNKlVMGAwKs2ZVK5X3oNMJli2LYt26dFq29L7gHAMEBhpo1apwF0qHQ+Wllw6yeXMao0dXonfv689ZvtGUZIpFM+CIlPIYgBDia6ALcKmDLNH6sAH4AbElaM9tQ5cuXXjiiScYP3483bp1o27dutc132NREGACuws6VtSitGYpUHNiw19zjGMkYiebKugwA0eIZzUb8KQcVnyJJSJnHfgHFAw0ZzbVqMw+FhHDJgx4cYwYdrKPZtyLH56cIw0HsJd4bOgBHdmouHDyLEF8ZrMzw2onJt0DH1VhWqIg3CnxTRekZ4O3Hv5sAa0rwfSHICYNoozw0mdaTnLKQYgMguQ0OHQCWjS8+r1LKfn442S2bMlm+PAgmjUrnoKH8uU98fTUYbE4adQoqFjmvNEMGzaMJUuW0KFDB+rUqVPa5tzyCCEqAOWBaCmlXQgRCgwFngNuvquPm9uS8ePHAxRL8KYsER9vpV+/HdhsKitXnmH37o4Xiu/mzYtj4sSTAHz8cTU6dQqmQgUTq1c34PhxKy1a+GI0KsVWUHe9REWZ6N8/5Lrm2Ls3k99/T8FsFkyefPKmdJBLUpuqAhBzyfPTOdsu5S3gaSHEabTo8eAStOe2Yvr06fj5+fHOO+9c91xCQEYsLP4B1v2jbZshAhiAN2NdAURn+JJo9cWECQ88caJDAvs5AYQg0aGiR0XTDFaxYyWeM+zGgZFGDKQ6L7KdbfxDNN+xkP504DGak0QARuyYsGHCRRjwCn68TAg/2ZxkOBSsioskm8RpgTM2OIaWTpGd8yMEdKoJ/ZtqtksJqoTa9SDbCg1rQaM8ul/u2WNjxowUdu2yMmRI3HV/lqoqGTp0G23bruXxx6sxa1Yr5s6957rnvdGsXr2aBQsWMHr0aLdzfAMQQgwF9gCfAFuFEM8CBwAPoHiKDdy4uQEcOnSIQ4cOlbYZJYaUV6f6HTxoweGQ2O2So0etF7ZXrGimTRv/6y52u1bsdskLL2RSv34a335bvJr+Vap4EBCgx2qVtG59A5dni5GSjCDnljRzZcLzk8BXUsoPhBAtgIVCiHpSysu6Qggh+gH9ACpWrFgixt5qhISEsHbtWmrXvv6+58kZMGKB5mhuPwL/TIUIk57uDh/uPOIiXV8ek3cw74Wm8Zy+DTOYRwYWPPGgBn34iYVk40F1svHiGHb8OMxRYtmKxEk8B2hMf9KxoaKSRBrppFCDctQklWTiMKNSmQAqEkAXtDvbDjoDvzlV9IpEVSVItHI/B6TboYEHhF+UhuTDdfDZBjCFwUtN4Pl2EOijva+8CArSodcLbDZJePj1pxEcPZrBqlUxeHnpmTv3MKNHN0BRBMuXH2PnzkReeKEm1apdvwB7SZKenk7//v2pW7fudTWncVMk+gE1pZTJObUbR4B7pJRbS9kuN26KxKJFi0rbhBIhNNTM3LnNWL8+nu7dIy5EjwEGDarAsWPZeHgo9OpVvGoNWVmSIUOsxMSoTJlipkGDwucG797t4vffnRiNMGmSlZ49TcVmV0CAgV9+acSWLencfbdvwTuUQUrSQT4NXJpYGcHVKRR9gQcApJRbhBBmIBiIv3SQlHIOMAe0wpCSMvhW47yKhcViIS0tjfLlr02E22QATxOkWyDIFww5fzWdd8LpTAWEQnAlwd0h5dAheJFeHCeGCpRjJb+RSDAAp4kkFM35S2MXRtSc8j0IoTwhhJFKKgbMzGYdThQeogltaUwoHtTkcrmajiY9s7IcpKmQaVTR2/ToJAQ5wGyGrCuKf7/7G8wGsDmhcU3tvaSkwnufgtEIr78M3lcU61WsaGDZsgrs32/n/vuvv5KvQgVPypXz4Nw5Ky1ahKAogn37knn99R04nSo7diTy9tsNGT16G7VqBfDJJ60wm8uW2Mxrr71GbGwsy5cvx2QqvhOqm3yxSimTAaSUp4QQ/xXWORZCfAl0BuKllPXyGdcUTWf5cSnl8uIw2o2b24lWrUJo1erq1ISKFc0sX57nV++6WLvWybp1TlwuGD/exrJlnoXaLzpasnQpCKHDbnfRvn3u15m1a+2sWGGnVy8jbdsWrej/o4/OsGTJOYKCDKxe3YCgoJurVqUkr7w7gOpCiCrAGeAJ4KkrxpwC2gNfCSFqA2YgoQRtuu2QUtKmTRs8PT3ZsGEDinL5Us5338Uyc+ZJHnkkjMGDc2/w4GWGFSNg8yFISode0+CljpBoB8UFUoGWToXaObIvHphJJYIzSNKxomXySLzwxReIIw4nPjSnOxZiiaIVAE/Sh0Mc4A9OkkIiXnhygBj6oUXBz2DnO1JJROUJ/KlnMPOal4E3klRcVh2hRnjAG8p7wMYkeL0a7E+A51eCWQePNobP1kNUCDSprL23T76Cr1dpj8OCYXCfq99//fpm6tc3X/3CNeDpqWfNmvs4ejSDunW1ZSe9XsmR9AGjUeGdd3YRF5dNbKyFjRvPcv/9ZauAr3fv3tSoUYPmzZuXtim3ExFCiOmXPA+99LmU8pV89v0KmAEsyGtATlH1ZDTZODduSoxx48YBFEv6X1lGSomUXBZJLgkCAhTOndPqamJiChc9VlVJr15OMjNBUcx8/jm0aXO1O5iSojJ4sAUpYcMGJ9WqZXLmjMr06T7ce2/BwZHVq5MwmxWSkhwcOJBV6AK/skKJJb5IKZ3AILQT7gE0tYp/hRDv5IjbAwwHXhRC/AMsBZ6TZbEh902MEIKXXnqJjRs3Mnv27MteczpVRo06wOnT2UybdpyYmOw856leHu6tC5+thd3H4KXZMLceRHkIWvkKFlS/+Ke0AQujiOctEnDSlHBqU4M76MWTNOIJTlOBOELYQxophDOfX4jmICY8OEwWMSThwEEqGTRG6wwYg5UeHGAGZ1lBKiPR8oGPWxU8XHr89YLaJphSDjKywWKBbAd88TfEZcKxVFB8YP878MtQ8M2phQjwB0VomsgBNyizwdfXSKNGQRiN2smsVi1/Zs5sySuv1OXzz1vTqFEwUkqMRoWoqLKzNHX+q3n33XczbNiwUrbmtmMksOuSnyuf54mUciOQXMD8g9E69cUXMM6Nm+siJiaGmJiYggfexJw5Y6NVq73Urbu6GJbIAAAgAElEQVSbTZvSSvRYXl46QkM9CQ/3wGbLPcKrqrB4Mdx7Lzz0EBw6pF3zVBX0emjQQJ+rlJzRKDCbtRRDl0ty6JALm03y0UeWQtk2eHAEFotK/fpe3Hln7s1OyjIlunabo2m8+opt4y55vB9oWZI2uIE+ffrw9ddfM2rUKDp16nQhj1unE1Ss6MHJk9n4+enx989/+cPbrKVbZFmhUgjUMcLjVvi/Q/C/dJhyH+gVSMCJlt0gScWPt3j8whwWElAwAIIY4tjGP6hIThJHC5qyh/+wYgcEekxk5cz0FifIyOm550LigebhdvSExSmQkgHbJETGgZIO5SW8vQ9GR8DSvWDQQbNwLcXiUgb0grAg7STRtWOxfNzXRIcOFejQQathfffd5jz8cGUiI72pVKnsnFRGjBiB0+lk2rRpuepNuyk5pJTzhRAhaG2lj0gpU4tr7hx1jEeBdkDTAsa660HcXBfz5s0rbRNKnHXrUjl92o7RCHPmnKN16+uLvqSnS+bNU/HyguhohW3bBFFR0KQJBARA+/Y6du7UusFeyv79Wo3Nnj0wdCikpICvL0ydKli6VM+KFSrt2wuCg3M/n3t5Cb75xptNmxxUraowZEg6NpukQ4fLo8fHjjlYsSKLFi3MtGp1cbX12WfL0bt3WIlH0UuKspXc6KZEEEIwZ84c6tWrR79+/VizZg1CCIQQLF/ehM2bU2jUyBcfn/z/HAJ94LtRsOsotK0Lj82E7dkgFEizQa/60CQcOuPDIeykoTKAAFxS4gKMQlCZCBpQgzPEcwe1WMZaQOJCxYIVAzo80JOOiXS8Wc1ZLJiJw669F6ASOj4inCSXZLVNpaUn/JmpEGsVGBWwK2BxwN3BsP6o1oFGJyEwlywJgwF6Plzcn/j1odcrtGp1bfniJcWWLVv46KOPGDBggNs5LgWEEC8AE4GjQBUhRD8p5cpimn4a8JqU0lXQ/627HsSNm4Jp1swHb28Fm03SqVPRWz2fx2KRbN0q+fprF2vXQlaWgtMJWVmwdy+sXAnBwTBqFFx537FyJQwfrj2+7z4tYiyEprJRpw7UqSOoU6fglIw6dXQXxm3YEEhyskrNmpfv17t3IjExTj7/PJP168sREXHRl7hZnWNwO8i3DZUrV2bSpEksWbKEtLQ0/P21XKDAQCOdOxdcVSslLPgGJs0AL3/I7A1n08DDAFkqeOihYs5NssOm0MceQqQPHHOqNE/LxiJhoq+OJKOVBtzNw5hYz0lc+KLHigEfunAPXuzEAmwgBRd2/iOesziwE8z5r+SbRBKBgVHpLr62SKSq2ScFGFxQ3w8mRoHBCo9s1CTfghUt1aJOaMl8vrcyVquVvn37EhERwaRJkwrewU1JMBSoK6VMEEJEAYuB4nKQmwBf5zjHwcBDQginlPKHYprfjZsLjM4Jc7733nulbEnJUaeOJ5s21cdiUYmIKHwhs8UiOX7cRY0aOgwGQd++LnbskKSmgskEiiLR6TRHV+SkBmr7XT3Xzl1gd2jXxuBg6NcPYmKgWze45x74ZAZ4esAzz2iBosIQGqoQGnp1Zq7drtklpZYLfavgdpBvI15++WVeeukldLrCy8BYLNCrF0RHQxZg8QBLPIyfAS8Ogj9joVE1GNoWQr3gSBo8ugaynfBGY7BXcpKgghF4U0nEhAsTgnF48CUxKFQgHCd9uRsfPPGiMj9wEAsORM6/bPQYkASjxws9NXNajvgqWkTZ6QSpQk0T2FT47Q7w0kPnb8DHBMnZ0KIStKl8fZ+f0yl57704Dh2yMnZseWrVKp7CvbLO+PHjOXDgAGvXrsXXt+zkRN9m2KWUCQBSymNCiGKTD5FSVjn/WAjxFfCT2zl2U1IkJSWVtgk3hIAAPYGBuUdPHQ7Jhg1WwsJ03HGHljdstUo6dcogJkaleXM9ixd7s2+fvKCr3K4dtGghqFRJux6HhcHx45pzO2DA1cfo8xxs2QyKDl54Ac5nRM2bD1HVITsbggMBAX2fz/t9OBxarvJ5wSK7XeJ0gqfnxfc2b14w8+dn0qaNmUqV9GzenMXevVa6dvUlLOzmUq64FLeDfBtxXsEiPj6eRYsWMWzYsAKXy3fu1JZyzGZISwRpAp2iSb11rAnjHr98/K54yHRoralXnYC3q+nxEU4cgI8CLrSfD8niMGFUwswdeFKD8nxPHHOJwQcdOnzwwJMAvDiARAJGJB9RjWC0L9wIX4UInYpOCj7JgGQH3OevOccATcvDwSSI8INxbTS7z6OqMPoj+H079OwAj7SH6rmLeFxgw4YMvvoqCVWF118/ww8/VC3sR3/TkpKSwowZM3juuefo2LEUk7TdXKliEVFYFQshxFKgLRCc05Tpf6B9iaSUs0rGXDducmfOnDmlbcIFpJTMmrWPdetO8cord9C2bcR1z+lySfr3P8X69Rm88koIQ4devUL7zjupLFmShU4HS5eG0LixibNnVU6dUvH2hr/+cuJ0SsaNU3juOYFeL/j3X/jyS4HBAJ06FWxHlSqwbt3V2z+bqTnV6RlwNh7eGAdRUXBv26vHHj0KPXpoKR2zZ0PFipLu3TX1i88+U+jQQQu21atnZMqUQACOHLHx3HMxZGdLfvopnVWrqlw98U3CNTvIQog1UsoHi9MYNzeGxYsXM3z4cCIiIujZs2e+Y2vX1ooAkpOh/wtwb0fYthfq14LGucg6GjJB2MFlhAH1oL5BYXOgBzYgUdGzmHT8UVhBJj7oSSeAPlRgL+lM5hguIB4TJkzYEEA2PpgwIfBCR2W0qK0qJUkueNpLQS8EXerASRvUuUQC8s3WcH8UlPeGyleoy+w7DCt+gcxUGDMRZs+HRZ9As0Z5fxYhIVqlr8tVPE1DbgYCAgLYtWsXQUE3ZzvsW4iRVzzPV7niUqSUTxZh7HOFHevGzc3OkSNpfPDBbhRFMGjQH+zb1+uy17OynCQm2qlY0aPQtRdHjtj4/fcMfHx0fPJJAkOGhF617+HDDlRVoqpw6pSTxo1NVKqk0KmTgTVrHAwaZEKvF3TooKN8eS2VIiNDi+YWNh3i1GnYtAXubgZVKl3c3rkTfLVAm8ulatr/Cxbm7iD/+iskJmp9AhYtgrvvliQlnX8u6dDh6n0sFvWCOkZa2s2db5GvgyyEuDOvl4CGxW+OmxvB4MGDWbJkCQMHDqRdu3YEBwfnOTYkBNavh3PnoGpVLe+pQW3o3lsrAPj4fXjofm3sf2fhtQXgcEK9SDgv3+urnG8GYmQCwcTj5GeyEQgew5swPDiBDYn2h2VEhwEFK04UoA1++EsTbQhEEQIpJf2TVX6zSuobBcuDFXz1gvpX/DUrAlrkERCoEAbenhAfo0XDbTY4eCR/B7lhQ08WLarMyZN2OnXyY/v2dKZNO8099/jRv3/4LVe8duDAAWrVqkW1atVK25TbHinl/NK2wY2b4mDEiBEATJ06tZQtAX9/EyaTgsXipEqVy9PHkpJsPPTQZhITbfTpU4mxYwvXlTYy0kiFCkbOnLHTrp1PrteFceP8GTMmhchIPQ88oCkyKYpg+vTLm1EFBMDUqfDtt9C7N3gWrgcIDgc82huSU8DPF7b8DB450qbjxsJzz0BSEjzTB6xWeKxb7vO0bq2pXthsEB4Ov/2mRbClhO7dc7/e1a9v5s03Q9m61cKgQXn7FjeK+HgLNpuLyMiiK0KJ/GSHhRAu4A9ybxt9l5TSo8hHvE6aNGkid+7ceaMPe8uxd+9eGjduTPfu3VmyZEmB46WUfP+9nePHVQJCTEyYqmAwQM1qsPKbnDlPwaMfaUVxUaGwfmze86XhIgEXEaoBvRDoBXRXT7IVCJNgEFk4RRoVMPO+rM0g0jklXTykejBe50vdsyqBCqSrsCFMR0V90Z3Tswmw9g/4chGEhcCc9yGwCAXHTZvuJCVFk6FbubI+depcf6e9ssL+/ftp1KgREydOZPj5Umg314UQYpeUssk17jsPyOtkLaWUfa/dsmvDfS52cy0MHDgQgE8//bSULdH4778U9uxJpH37CIKCLro0Gzcm8vzzuzCZFLy99Wzd2pYvv4xj375MBg+OICoqb/fHYlGJibFTrZopV33hksZigTtaawpTqgt2rNc0/68kM1NzfvNbIMzMhJMnoWtXrQDPbJZs2gRBQdf+vqxWlRdeOMLff2fy1luR9Ox5dffB4uDvv+N56qmfcbkkU6a0pGtXLS2ysOfiglIsDgD9pZSHr3xBCHFrK33f4tSvX5833niDt956iyeffJKHH76odZaW5uDMmWxq1fK5INGyZYuTUaOysduhcVMVHy8vsizQ5aFL5qwI7/aEn3fD39HQbCDMHwW1K115dPBDx/ZUHQ8dA18dfFtTcshoxOWSnFJUPDEgCeSc00wvmU6c4sSO5Buyqe8y8YSnkW8skntMgoicmsOjGbAnBdqGQVAhSpjKh0Cf7trPtRAaaiQhwYHZrODnd+uk87tcLp5//nl8fHzo3bt3aZvjRuOnXLZVRFO3KHzVrRs3pUxZcYzPU6NGADVqXB0ZadzYn5o1vTlwIINRo2qwdWs67713EodDcuRINqtWNchzTk9PhZo1S6aIOzVNK0wPzsep9fSEjybCwm/giW65O8cA3t7aT354e0NoqJYyYbOBj48gMPDa7QfYtSuTrVszMBphypQzJeYgb916jqwsB0ajjrVrT11wkAtLQVf1t8i7297gIh3JTZlj9OjRZGZm0qxZswvbEhNtPPDAX6SmOnj00fJMmaKdBJxOcqppJWajZNPPkJEJFcIvn/PxFvDfUfgtQ1t2WLweJuS0b5YStpzQ0jTuqgTz47VtCQ7YlC6oFmQgXtjRqQpOoYDQke0ycdipYDABQmBy6bDrYHKAjkirZM5JeCRWMCYS+v4JVhdU9YFf22v5VV/8BQkZUC9Es+ehRlpKxaW8Oxm+WQ5PPwmjXi385zd/fi1+/jmF+vW9qFAhf4/82LF0Vq06RcuWYTRpUjIng6KQXxvUjz/+mG3btrF48WJCQ926eGUBKeWK849zZN7GAPcAk4C5pWWXGze3Kl5een766W5cLoler/DPP5mA1qbZ2/vGBkR2R2vX1fLloP9rWiR3xkS4v03e+3TuqP0UByEhWie+zZu1AsHrzSasXt2Mr6+O9HQXnTpd3UTF5ZIsXBhHerqL558vd82fd6dOlViw4ABZWQ769q1T5P3zTbEoi7iX9UoGKSVCCLZsSaJ3752YTApms8KuXe0vvL5ggY0jR1ReeslMeHjeXco37IH+07THnwyEjjm9uZb+DWPXaI7q5M6gi4CRJ8GswIqaUN6kMsCeySmXSqBB5W8c6FSQDiMGwE8InjEZeVHvgdUpaLQHzmaBKiHYDknJoBdQwQMOPwLf74HhKyAzA+xpEOgJAzvCiC4XbU1KgqattLvkjEzYsxX8irnltJSSu+5aydmzFjw99Wzc2JnQ0MJlJ61fH8O5c9l07RqFh0fxnJTj4jLp0eNb4uOz+OyzTrRvf1G+48iRIzRo0ID27duzcuXKWy6vujS5nhSLnP1rA28AjYApwCIppbO47Csq7nOxm2th6NChAEybNq2ULSk6v/2WwqFDFnr2DCE4OPe2zsXN4aPQuZcWvQ0MhMQ0LZr78H3w8fiSOabDAanpmgxcSV0CkpMdnDljp25dz6sCNcuWxTNy5FFUFZ55JowJEwqQmMqH8z7updey4kqxQAihAwKklIk5z43Ac8AwKWXhstbdlGliY2Pp2bMnb731Fq1b30vz5gHs3JnK8OE1LowRQvDss/kvGe3bpyX8t20Mv72vJUxWvCQAeShey0+WEmZthiAvmNcOGpYHbx2AwiKTLz8nQrpDsiAMfA3wvWLnP6nyrMFE+RypOr0OgvUQK7UljrRM8DNAtgv65BQT6hRAaHfbUmoR5TMpl9vs56fJ4Zw8BdWrFrzcdC1ICRaLE71eweWSOBxqofbbuPEM/fqtx+mU7NmTwOTJxdOVff3645w+nYHBoDB79q7LHOTTp08TGRnJrFmz3M5xGUIIsQytocdUYBiaWqLv+f8jKWVy6Vnnxs3tQfv2AbRvf+2d8a6F5FTtGqbTade9oACw2aFXHoV1V/LbDhgwETxMsPAduKOGJnP63lewORpG9YaWd8Cv2yDIH2pVgkdehJOx0LcnvDGw+N6LlJIdO5wYDNCokYHAwNwlOVwuecnj6zvm9VzHClKxeAKYDWQJIQ6jpVwsBHYAvfLZ1c1NREBAAAkJCbz44ovs3buXxYubFbzTFaxfD/37a87guHFad54refEu+PcsJGXD4UQ4mgTvrYFVL8CGE7A1CT49DalGCDIJjmXD61Whm/Hq9AWjAqPDoH8SZDhAkZDmgDv84aXqmh1tqsO4B2HrIYiLh2AfGPnI5fPo9fDjt7D/ANSto52ErsRul0ydmsHZsy5Gj/YlPLxoKZ+KIpg/vw3z5v1Hx44RVKhQuGK+pCQrLpdESsm5c7m0SrpGmjYNx8vLgNXqpHPnGpe91rZtW/bv31+kZjJubghN0e45RwDnqybPn/klcO0hFjdubiA3Y+T4SpKTXXh4CDw88l5JLQ6mfg7zlkGVKAjyhddfgfp1NAe3sHJvAybCiThAwsD34c8vYM9/MG+VpvQ04mN4tA188YMWVHr1SdhxEGwO+Gxp8TrIS5daGTcuC5B8/LEPnTrlHnR77LEQkpIcpKU5GTjw+rWpr5WCIshjgcZSyiM5km9bgCeklN+XvGlubhQeHh7MnTuXe+65hzFjxjB9+vSCd7qCf//VloDsdvjmG+je/XJJmtgE6DESktNg5EswORUcKkT6w2e74KPtcMYCXuFg1Wu5xPE2bczhdKjsDZ5X/LUeyQAvB2RZwaCDEB2MrKFFkod8D9/vBcUFlnOgWKFaEByLhfArCgy8vaFZ08u37djhYv16J488oufAATtz5mQhpcRqlXz+uTbB3r3ZHDxoo2NHH3x983co77wzmDvvLJrkTadOldm7N4kzZzJ5442mBe9QSKpXD2LTpj5kZtqJjNTySWJiYvj2228ZMmQIev2tU3B4qyClrFzaNrhx4wYWLEhn3LgkAgMVVq4MJyLi+jXxXS74cgnEJ8BLfTQ1pSwLfLoQfLzgUCxEeMHzk+GLsXBnrcLPHVUBTpzVVlWr5NQMhQWC0aBFoqMqwJEYzel2uWD/cciyaeMSMwqe327XZOhMJq2NdX6xlX37nDgcWv3LgQOuPBueGAxKqTrG5ynoSmiXUh4BkFL+LYQ47naOb01atWrFwIEDmTFjBj179qRVq1Z5js3KcnH4sIXatb0wmbQ76MhIGx4eDhISPPnnH4UxY+DSQMFv2zQn2aCHXzfA0pfhRDI8WBte26ClPxgVEFbtTvmhEHitKvT5C7YmQKQXrG4Pl6bhPhUJv54Ds11LtzhzBsb8CpujYOW/kJkN6VaQNhDxYEuHFz6E6NnaySEvUlIkvXtnk5ioMmOGnZkzdeh04HQKAgO193v8uJ0ePU5is0lWrEjj668vSnXY7SqnTlmpVMmMwXDtEQajUce4cQVH85cu3c+iRft5+uk6PPlk4QoRAgI8CAjQ8qCllPTv358//viD7t27U6lSLrIjbsoUQogAKWVKwSPduClblDWZt6JgsagMH55AaqpKWppg9uwM6tQx8+ijHpjN176Uv+pn+N9kzYmNT4SPJsC/x6FyRTh9Bsw+EHNOixrP/g5mjyn83Msnw9wftWveczliVRVC4cepcOA43NsEziVBRhYE+sPv/2hjhAD/PKSD7Xb44SdNW/nwATgfU7PZ4Omn87ZlwABP9u51YjIJnn768uhxerqKxaJSrlzZCdAUZEmoEOLSun7vS59LKT8sGbPclAbvvfceq1atYuLEiaxevTrXMXa7SufO0cTE2GjQwJsVK+oSHe1g5MhkUlMlOp0dvT6QuLjL92tWD7w9wGqHh++BxpHQqIJ2B/tqc4jNBF8jvNgU/PUw5hd4Nhr26rXUiFNZcDYboi75wlb0hLZmmJcCp50gneBpgvWn4L4aWlGgUQG9CTCBlwk8jFpXotyYPx+mTIGmTSVpaZLUVO337t0Kn34aQEKCi8ce05zKxEQnTifodILTpx0X5nC5JD16RLNvXyYNG/qwbFmDXJUiiov0dBtjx/6JwSAYO/ZPOnWqiq9vITTuLmHhwoWsWbOG6dOnu53jm4ffgLwaOblxU2bx8Ljh7ROKjUOH7Oh02jXEYoEFC7IBG/v3O+jQwYOsLEnHjsYiax8v/RESkgChOapTF8KcH7TjjB8J4WHw4kQtkNSuiIuJPl4w9Kmrt1evqP2cH7NsCmzfD7/tgfCKkJEGa2bnPufHn8Gnn2tOdLP6WvRZCK3bX26kpmpR5kqVdAwe7M+yZS6WL4eXX5YoiuDoUQePPhqPxSJ55x1/nnqqBIqBroGCHOTPAZ98nru5hfD29mbNmjX5OkkJCQ5OnrTh7a3w998Z2Gwq6elay0xPT0FgoErLljD2iiYhNSvDn/PAYoXwEEjLgMdGaCkPb74AKx67OPbDv+DvWC0/qkZ5iHHCA+FamsWV7EvSEjAVBSr4wtlMeP0u6Fkd4s7CwVh4pTu0rQqb9sH9jbVCh9yYNElbHtq0SaFjR4XvvlPx8pJkZwseeODyu93GjT3o1y+Q7dstvPbaxUrE5GQH0dGZ+Pvr+fvvDNLTnfj7XwxXq6rk7FkLoaEe1xVdPo/ZrCcoyExiYjbBwR6YzUW7+46Li2Po0KG0bNnyQmTHzU2Bu4LSzU1JWeigV1Tsdsn06alYrdCwoYn9++3cdZcn27dLVFWya5eDJUvsqCoMGeLJ0KFFaxqVnAFBIVoX2k73w9I/tO0OJxjMcE9j2DALrDaIKsHMg/pVoW4ViD4CE56HO+vmPi4pRVOPEhJatoaqVbQUi2efzX38iBHwyy+Qna2tQDsckrAwSdWqggcfFGzbZiM9XcVoFHz/veXmcJCllG8DCCGCz6tYuLm1qV1bEyaxWCycO3eOKlWqXPZ6eLiRHj1CWLkykUGDKmA262jZUmHYMG/+/dfJ8OE+5NWZ2N/n4pLN7ztgx3btrvOzb6FPjvSaqkJVfzDptUK7F+vBU3nrsfNmMxj5J0R4w0f3aCkYioAlmyH6pBZV3vwfDL4P6hdQxtSyJfz+uyalM3myJzVqWMnIkIwYcblzvH+/jXXrsnjoIV9GjbpcJzg42MCjj4by3XfxPP542FUNRAYO3MrPP5+hdm1/vv/+XozG6yuGMxp1/PDDo2zdepYWLcKLPN/gwYOxWCzMnTsXJa/QupsygRDifOmrAAIueY6UckHpWOXGza3H0aM2Nm3K5J57vImKMjFgQDwLF2qF0j17erFvX3lMJoVJk9KJj1epUsXAvn3ZCAGnThVddmHcUBg1EWpVhQfbQWRlGPYhRIbBfTlZduHXIZ+fadeui54FpEt7mOCHyWB3gCkfFbsRr2jpFF5e8MJzubfAjjsHi76GWjUhPV271lutmqqElBKH42L767ZtzZQvrycpycULLxTNOV66NJY//0zmgQdC6dQppFhXbAtqNd0ZmAc4ABXoKaXcXGxHvwbc2ps3hrZt25KcnMzOnTsxGotf7/HdT+Cd6dqS0b2tYN18Ld3i8QnwzzHo3A76PACNymuO8voDWpT43lqF02XceQw6jof0NAgPgt0fQmABax8OhyZVV6UK+OfRechmU2nS5ARpaS58fRW2b6+Cp+fVjqWqyqu+qE6nStWqKwgMNJGebmfduo5ERZXugsyWLVs4ePAgffr0KVU7bgeKQQf5f5c8HQDMRHOWpZTyneu1r6i4z8VuroV+/foBMGfOnFK2JHesVpW77jpESoqTgAA927bV5IEHzvLnn3akhObNTfz11+UdsjIyVMaMySQjQ/Luu95UqFD4QIWUsOEfSM6ER5pfXh+jqrBqPyRZ4ImG4FnIS/GGMzBmK9QPgqeqQv9ftR4BSztBgxvUp6p7b9i+E4wm+HgSrFurRZk3bNCkTkeOFDz5pLggw6aqEpcLDIbCO7jR0el06fI3sbFWdDrBgAEV+fDDgtWHi0sHeSLQWkp5UAjRHHgfyKd3i5tbhVdffZUuXbrw3nvv8b///a/gHYpIzapaoYDLBT3u17YdOg37ToCvJ/y8EdpUhfjTEO+At37UxrzbDZ68C5IyYNcJaFIFAnO54WwSBeW9wE+vOdYHYqBlAfVrmjZj/mNcLm25zWAQ2O3gdOZ+g5nbXaxer9C7dxQLFx6jdeswKlUq2jJccaKqKoqi0KJFC1q0aFFqdrgpPOdX9ACEEF1Kwyl24+Z6CQrKp0dyGcBul2RlqRiNCllZKg6HZObMELp1O6dp+M+62n4fH4VPPvG9puN98B2M/0ZzfvedgLcuKXJbcwiGrtTSGY4lw4QHCp7vWCY8vBqynbAjAf5NAocLsiWsPa45yFKCXQVTMap5Wm3wy2aILAeNamuFfEIAEkKCLy3aF8DVB1YUkWd9UF6YTAoOh4rLBUaj4I8/ilcOviAH2SmlPAggpdwmhHDnH98mPPLIIzz55JO8++67PPbYY9SrV69Y53/sQQj005Zy7r9H21YtHKqUh6OxUDEERs4CocDdLcCZ01vjZBLYnfDINDiXBuX8YMPoi+2js6wXC/GGPQITvoXaEdCoaC3Y88TTU+GLL8rzzTfpdO9esLzblUyY0JgxY+7Aw0NXqo04+vTpQ1BQEB9+6K6zvUlx5yC7uSl57733StuEfPH11TFtWgWWLk2hV69AvL111KqlY//+yHz3s1i0dsy+vtCjR97F4JcSnwof/KjJqlnscCbp8tez7JpzDJCWfXF7tgs2JUE1L4i6Is7SbwdYVW0/ndCiyEnp4KnAg1XA7oKn/oCdCTCwNoxsABYHTNgIGXZ48x4IvYbYzeiP4ccNWo3P8g9hxlSY9SXUrQ1NGxd9vkuRUrb1QOsAACAASURBVPLbb5nExzvp2tXvwqptzZrezJ1bnzfe+I+0NCcjR1YpYKaiUVQVi1C3isXtw/Tp0/n111/p06cPW7ZsKVZ9XCGg3RWN4TzNsPpd7cv8/tdwPBakC5pUAJOnts9TzeHD5XDoCBg9YecZmPYTjOwKk76DWT/DHZXhm+HQ9354tr0mfl6cvmjr1p60bp1L0lUh8bxS0PkG83//938sWLCAcePGlaodbq6L3qVtgBs3tyqdOvnTqVMeeXZ5MGkSfPWV5hibTNC1a8H76HXaiqnFpj0e+8Tlr3etC8eTISELBra+uH1gNPyRBGYF1raAyCuEQUJDtLzfHpXhw1ZAS8h0wfYs2BMLW1Mh0Ahf/Kc5yEv2weK92r4eenj/viK9dQCOn9Z+O10QGw8NWsHE61h8Xro0k/ffT6dNGxMPP2xkwIAzOBySf/6xMnly+QvjOnYMoWPHkskbKege57xqxfmfK5+7uYUJDg7mk08+wWg0kpx8YzrZGvRQLhBeewJqhUNGPKxbAx8/Dl/0gUW/wMxVoGZA/FkI9NKc4rgU+GoD+HnCvzFw6Iw2n15Xcr3kc+PYMSuvvHKUOXPiyC+/v7RIS0ujf//+1K1blzFjiiCm6aZMIaXcV9o2uHFzLfTp0+emqHlIS1M5e9ZZ6PGWnGanUmpqDbnxwxZoOAie/0hbPQ30gYWvwhs9YfP7UClMGxedCvOPQ7IDhrWBE+Xh3l3w6kHIdMK/mVp02KbCkiTodBrmpWn7zmkKL1aHpffBvLZagy1PAww4CoOOwIvHIdELTurh4RyZt2CPi4GkkFyix1LCR79A+w/gh925v7d3X4E7a8PjD0C75oX+2PJk/Pg07HaVn37KJjrafqH9dHx84f9PrpdCqVi4uX3p2bMnPXr0uOEKB2GBkBUL5Y1w6Chsj4Z2LbQvKhJ8PCDUG5w6LQfZzxMeuwuWboKoclD9khoKKSHbCp4el287dEgrxitXrvjsHjLkGHv3Wli2LImDBzMZO7ZSnv3mS4NRo0Zx9uxZvv/+e0ymoukluymbCCHWSCkfLG073LgpDJGR+acqlAX++89Bt27xWK2SCRP8eeKJgpUVxozRIscBAfDYY7mPmfiNpiix9BBsfAe+eRGa1YAGUTBqB6zeAt0qw9I4zRGO9IIFd8GeDHCZYXoGzD8CSjnwzoQeJphllySabPxqUdHrjfT21vN2/cuPmy4l/2WDKgUuoIKH5pxPydFUfqQmGHWQ5YAuNa+2+0QifPq71rF25DJ45A4tUh6XAs99BmlZMLu/llpREBYL/PQTRETA3XfnPa5ZMyN//mnDz0/hqaf8yMpycvq0gzfeCM17p2ImXwdZCJHfGqyUUo4vZnvclDGE0KpMz507x8yZMxk3btwNc5YfaA3zVoCfD9TJkY4b2g0SE2F3NLzwMIRGQMPKmjzNhKdg8EMQ5HMxJ9nugKdeg53/wovd4Y0Xte2zZsMHH4HRCN8tg1pFaN2ZH76+OqxWF0lJTpYsOUdSkoP58wuuqr0RxMbGsmjRIl599VWaNi2+1tVuSh4hRF5NQQTQ8Eba4sbN9fDOO2W/tnTbNhsZGSomk+DHHy2FcpADA+Hdd/Mf07I2LNoJLgUcKnz+J5TvCg+ug39ToZwHzDsKKXpwAemZ8M4ZqOEFv6taNDhdQKQCLj+YUBn+74wLm6KiB760Oejtdblbt8JuY5zNiq66oPJpL2w2hQRP6O/HhToYRcBD1S+31aWCQ4JZpwWgbGZIcUDDYO31LDus3Kmt2Bp08OlazUkuiNdeh1WrtKL4pUugyRVaEtHRTiZNslK/vhf9+/tQo4aBoCAdY8eGFTx5MVNQMmRWLtu8gL5AEOB2kG8T1q5dy9tvv01ISMgNayjxxsvweCcIDdKcZNDylNdvgAwLvD0D1s+D0JxUMSGgXMDlcxw5BXsOavrL83646CAvXAyxZzUdxn+i83aQt27N4ptvkunSxY+2bQuuUp4+PYqJE2NYuvQcBoMmil5WCA8PJzo6mvDw8IIHuylr7AD+IPfivKIlS7px4yZXpJS8/XYq331nQa/XvmpF1eXNj6kvQJN68L+ftevVfbVgawLES3BVgDNANRc4JaTawewL+7NhX2NYlATjz0EyoAq4w9PB/5R4zOVtmFODCJB6HjRe7tIdxcoHzmzicKFXFLpVdhKbZMQfWK3C6DzsPGOBbhsg2Q4fN4X0VFC9tEZffzug5eew94TWqdbDBIoLWuYSec6Ns2e13y4XJCRc/fqwYRaOH3exfbugTRsvgoKKUWqjiBSUYvHB+cc5ChZDgD7A18AHee3n5tbjmWeeYcmSJbz22mt06tSJypUrl/gxhYDquRzG0wNS0sFovlwz8jwOB4yfCcdOw6i+WuehIzHwaDvtdZcLTp4C1aXlitXOwzm2WlWee+4Edrtk9ep0tm+vhZ9f/l/WoCADU6ZUoVYtM4cOWXjllRJse1QEdu/eTcOGDalatZjkPNzcaA4A/aWUh698QQgRk9+OQogvgc5AvJTyKjkaIUQXtGCHCjiBoVLKP4vFajduruDppzUds0WLFpWyJVdz8qSThQuz8PAQqKrK/v0RmEzFt2Kq00GvltC+HticUCkI4rLB6g0oWlGYhw9MLA8LksCuSB6IymKa4qBXiA9PBek5g5Xf1SwW6pL4HhWhh7qBSfRVg+mru1g8vpYUphFLnN6IyxUAQqWCwYVZgFVC43wy7P6Ig3irFhmedwQeDQKEFvX2UmB7HOicYAMqR8Kix6FOITNnJr4LE96FqlXhvlyKAcPDFY4edaHXQ3Cw9tmrqqZi4eWlcPfdN04etcByeiFEIPAq0AuYD9wppUwpacPclC2EEMyZM4d69erRr18/fv7551KRKRMClkyBleuhRUMIC756zLrNsGiVJnNjs8NPn0JiCpTPKXRVFKhZA06awMcH8vL1FUXTVrRYVDw8lEJrNCqK4MUXy06UdvPmzbRq1YrPPvuMAQMGlLY5bq6Nt8i7qHpwAft+BcwA8uq29xuwUkophRANgG+BYko6cuPmcmrWLGSosRQICdERHKyQlKTSoIEJo/Hya1x2NrzQH6Kj4d0J8Ejngue0OGDNMYjyh0Y5WQLl/LTfqgRpgDHVYexxiVOROELttK9g4KWKOnZj52VScCI5gJ2HFZWPOI1eASsufDCRjhm9ksgG5Sg+VKYn1RAIosnCiSTQmI23QRKIJw8Jfx4sD6ec0PQSBzlNqvggUHKu6XeFgK9Ry0nuXhm6RUJ8Fry/RXOSwzwgMRPMemhTrfDOMUCNGrBgft6vf/qpF2vW2KleXUeNGrqcbUlMm6Y1c/7sswp07HhjNCIKykGeAnQD5gD1pZSZN8QqN2WSSpUqMXnyZAYOHMiCBQt4Nq/G68XETz+5+PJLSY8egiefvBi5rRIBQ565fKyUsGmb9jgkULtTly6IKKdFmcMvyesXApZ/A3/+BY0aarqVuWE0Knz9dRXWrEmnfXsffHwujx4nJdn56quzVK5splu30DxvGI4ftzB9+jFq1fKmX79KN/TGwmq18vzzzxMZGUmvXr1u2HHdFC9SyuX5vPZDAftuFEJUzuf1S8/rXkDZk19xc8vw5ptvlrYJeeLlpbBmTRgHDjho1MhITIzg33+hVSstmLJ1G2zbpuXPvj8ldwf575Pw5ndQszxM6g5DfoNfT2jpCN93gzrBmk6xVYVBCfBXNrQww4j6Dr6SNpw6+DBbMsvb47J8KicOPucMFiRGsvHBghk9bQliH3GkAF9ziE0cQEWlPGGEEkhFFB4UATTHhwroQQ8ROZ6fDcnTziR2qU4aq2YWm/wwCkGUD2x+QNNbDjZrY4/9P3vnHR5Ftf7xz5nZnt4hQAhV6dJEQQFFECyAioDtpwIW8AoqWK+iKHpVrHi9WFHRiw1RwUazAgoC0pEOIaT33WTrzPn9cSJFEgiBAHr38zx5srtz5uzZSXbn3Xfe9/vVIT8Z9CC0iYXPhysDkjPT9q9x9U6YPAvKK+CannBN76NXkYqOFgwbdnB6e/t2P6GQRErYvTtwdBMeA0fKII9HZdEfBP55wIn9D3vT2lnHhPnLcuutt1JQUMCAAXXbNO/1Su6800TTYO1aSd++GomJ1b/TPvwc/vmUuv3Y3fDuU7A3Fy7qWfX4+HgYeOmR19G6tZPWrZ1VbpswYSuLFhVhtWokJ9s499y4KsfdeecGVq8uRdcFrVtHkZJiZft2N717p+B01q0m8qOPPsrmzZuZN28eUVFhZca/MkIIHYiTUhZU3rcBNwB3SimPqRNUCHEZ8C8gGbj4MONuBm4GSEtLq25YmDB/WeLjdXr00CkogEsugfJy6NABZs9WVx4jIlQAeO45Ve//4GzYnA2/58CFbWFPqQqYQhLyKsDqhyGZ4DahXEADC/zsg6vjNT71qW+nrXR1sagDNiYSz1aC9MPGg2ThQGLBJAYLNjRchLAgMTAJEqCUCvyAGx8tKCKJZL5hBz9j51G6E8l+v+qZ0s1izYvQYFUIdspIThPqnBRhVT+gMt2fZqpmPsMGBQFo3+BQJ77b3oTVW8AfhPW7lZpUtyNcMCgvh8mTlbrFQw9BYhVXhe+6K4m8vBDR0TrDhlXdcrFlixuXS6dhw+o9CrKy3Fx99ReHX9ABHKkG+cRqe4U55dE0bZ/BhGma+1Qujjc2GyQkQG4uxMSA6wi+HDsyVO2xALbtUvtD1TXKJSXwxTfQsjmceUQ39uoJBlWiTUq573ZVREXpmKbEYhGUlPi5+ealBAIm55+fwuuvn1X7BRyBVatW8fTTT3PjjTfSr1+/OnueMHWPEGI48CpQLoTYiiq5eBfVvHfMlwaklJ8CnwoheqLqkS+oZtxrqCuKdOnSJZxpDnPUDB+u3DA++OCDQ7ZJKdm4sZCkJBfJybU3Yzoe5OWpoM1qhS1b1GOpqbBwnmo0q85c9vT6sDkHLBo0ioOnz4PHlkLbJDi3IbxTCiUGWIEo3STDlJzjklxst9DQ4mQRWVh1H7k0IgUnA4jgj3TUo7RiPWW0IYJP2YpAcC3pGGwkF4lOGRomkWiUEE8eJhkU4yCFUvzsxcNpxLOEHDLw4BHxOBF4pSRJaKSLqntsBNC9HnydCZEavNQFMsvBb0DrA/JCiVEqwBeoYNpSxXRrNypb6q5nqOzyu+8qB0KAyMiqlUDS0mzMnNm42r/Ve+/tYtKkDWiaYObMs+jcOb7KcV9/vZMdO0qqnefP1Gn6SgjRH3gRZbz9hpTyyT9tfx44r/KuC0iWUoY7sv8C5OXlMWjQIMaNG7fvA+94ouuC2bMt/PSTpFs3gct1+CB81NXKXS8Ugp27YNoMsNugpBRGHRA+GAZ07wc7dkJSAiyYA6e3rN0ap0xpwcsv76FZMye9e1edPQZ48cW2fPRRFs2aReB0SoJBlRnfvLmsdk9cQwoKCmjXrh3PPhvup/0b8CDQWUq5rVLy7WdgeGVge9yoLMdoJoRI/CNTHSbM8eSMM6pXJXzyyeW8+eZ6nE4Lc+cOJj095gSu7GBatYIbb4TvvoPx4/c/npSkfqrjySHQrw2kxUOrVHitAH5tAet06O+DnhHgKjIplZLmiQXER3ooFpAhGiEtHpaTgYFJFl4m0wGJpIBiInDSmihaV3q0taEr2WTwLq9gJUQqIcpwYaBjohONnxABotFw46cZiRRTwmMsZzNBDFw0p5R7aY5bwC2WSOzVJLsWlMKvVohJgxH1Ic4GA+arzPJjneGqpmrc9DEw8yfYngUXdIDOzQ+eZ/73MOYBQMLEu+D/rlRXc3VdlUke7rgeju+/z8MwJH6/wW+/FVcbIHfqlILLVXNfgjoLkCsvB74M9AUygV+FEHOklBv/GCOlvPOA8bcDHetqPWGOL/Hx8RiGwe23306fPn1Iqu1/diV79wZZvdpL9+4u4uLUv2VqqmDYsJplp5MT4Z2p8OBkePkdcHshIQ6KSw8et2wF7NpdKTFTCMXH0G5av76dyZObH3FcfLyNW29NByAUMrnyyjRWrSrm4YfbHX7HY6Rfv3707dv3pDRThjnuBKSU2wCklKuEEDuPV3AshGgObK9s0usE2IDC4zF3mDB/5r777qt227ff7kHXNSoqQmzcWHjSAuTiYpjyvLpyOXeukgOtKTYL9K/8aF/qgYeyochQttCvFcKzjQxSm+wmBkmRFiKmsvf2NZaxCzdenFixYK98/Ht+4RdWYcPKSIYRy/5jMp9P8eIDTKyEiADKicCCRmtiyCCfSIIMpwMd6cADfEoQE0kAgQOB5Baxf74NVDCFvTTCxgM0wioFmRjkBnUMBJoOuUGYX6Lqk3Xgl7z9AXJClPIiqI5N2yAQUA3w6zapx4YMUcfX74dBg2p+nA9kzJjmrF5dQlycjYsvrr5BvmPHFL7/fjj1699Uo3nrMoN8JrBNSrkDQAjxATAI2FjN+KuAY3DuDnMisVgsTJ8+nU6dOjFu3DhmzpxZq3mKi0PMnVvEk08WEQhAerqVBQuaIoRSj3A4BJpW8wBv9x6Icqhvtt27wC3X7d9mGErHMbkeFBZAm1ZwRnvIyFCuPkfjf2Ka8qjW9QcWi8a//lW33wM3bNjAF198wfjx47FY6rbGOcwJI1kIcdcB9yMPvC+lrNbDSgjxPtAbSBRCZKI+Z62V+70CXAH8nxAiCHiBYfJU9EkP87dnwoQuTJjwA23aJHDuuSdPIvP5l+C9ygqQeikwqpbO2BKwi8qSA80gP2UvVxOgXJM40LBi4XxcNCTACtzEo2MhyCU0pS/1AVjHBkyC+JFkksV6PqSUTFrTl2hiiKIILwI7EisVxGBwEdfhpgIPuQgkfnIpIhsrBQjKSCaKNnRhIE0OWu/LZLOeClbiQZOS3aEYVssQp0VbuDYplsKQoNgL37ihIgFa+eHWo9C7uWowLF6mnG1HV/b4axpcWoN+oMPRqVM8K1bUrIywXr2a61rX5dmzAXCgPmcmUKVDtxCiMdAE+Laa7eHGkFOQtm3b8uCDD/Lwww8zfPhwBg4ceNRz3HDDFlatqiA310rjxjZ27QpimjBtWhnPPltKy5ZWPvkkmcjImkWvD98LE/8FjRrAo/cr688/uPNB+GohxMTCc5Oh59lw0UWQsQcGD4KaViK8+moGTz21gzPPjGHGjA7YbKdOqb5hGIwYMYIdO3YwcuRIEqvqeAjzV+R1IOow96tFSnnVEbY/BTxV+6WFCVNzrqj0Yf7kk08O2XbhhelceGF6jeZ5441tvP32DoYPb8w//nFs0nFz5sCrr8GNN6iMZlSUCmqFppryakOhNDnDJXi6geC3CkhLLGeWzYcOWAhSjo9+OHiEppQTZAvbKMXPeaRyOtnkUEgZLiCDciwkEgdsJYuVQAGr+J3TGcrpDMZCkHW8gw8bDny0oTUSiR0/vzCbjexlCytwEYNGFJIQ19IMB+oEuYtiPmMDIAjgBARzKaBUOkhFZ5MI8u80kwR0mv4MsVbQBczoAU2PIruenAgfv16743kyqMsAuar0WnVZieHALClllbZj4caQU5f77ruPTz75hOeee65WAfKePQHsdoiONkhMtHD33cnoumD6dA+RkRo7doRYuzZA9+6OGs3XvCnMrOYN+O1icDhUB3J6GmRlwZ5M1Rjw5Zc1D5Bfemk3ERE6K1aUsm6dm86dT16d3J954YUXWL58OTNnzgwHx38jpJSTAMK1wWH+6px99tnHPIfHE+SJJ9bjdOo899wmrroqnYSEwzhfHIaSErj2WpXVXLgQunWDc3pDngc6nw5Dr6h+X58BPxZCUxc0PyAx+ZHhZbLhRgrJpDgnT8dHsw07cxEEkNgppR0B9lBEKc2Jxc5j9KIEHztYzBKWItBoRisiCNCMEA3ZRQ5LseEmiBUNC9l8ThvOI44hbCMCnQrqoeo7/BSxhxeJJ0AByUgc1CeBAkppTGPsB6hZvM1K8vBgIEkgGg9WbDjwax6KzGgu0ewkoiEEjG4Ar+yFC+IgvWan5VoRDEpuvz2HZcu8TJyYyGWXnXjRtLoMkDOBA+WjGwJZ1YwdDpwY/+IwxxWbzcZnn31GSkrtfNJfeqkpzz23l549Yxg7tv6+etkhQ1y8+aaH1FSdNm1sR5ilZowfDf96EXqcCW0rRbE6doRff4Xbj2S1cAD9+yfy6ae5pKTYad5cdVp7vSF0XWCznTxbzK1bt/Lggw8ycODAOmmcDHPyEEJcArwFBIUQJjBUSrn0JC8rTJijZsKECcc8h9Op06hRBFlZFdSr5yQqqvahjM0GgaBqEgP4+geY8h4YJsSnwM9bweODvu0OLcP7xzr4rkBpHH9+pmS21cdu0yRTC1Aqghj4eEy6aSYsdMDFO6RTRIiPKGEXFaQTTVRloOrAQj0i2UQ5JiE0LCSQCgQx2YnOekJ4sKPhJJUgeTjZSTabcNKU85lIOfnEoq6y72IuUIoDSRJ5pHEeXRiKGw/RRODDjYNIfmQ5PtZiwUUZcURQouqfhYMWFhevyCY4DlC3uLMRdEuAFpXfR17ZDNvdMK4VNDyOJne//eZj0aJyrFbBY48V/O0C5F+BFkKIJiiL8eHA1X8eJIQ4DYhDdWWH+QvSpEkTpJRUVFSwa9cuWrduXeN9e/SIpkePQ//x778/hlGjooiN1Q5xM6otN16tfg7kow+VPJxhwD33KFm5p5+Gw8X7Tz99Orfemkb9+nYiIiz88EMeN9+8AodD4+OPe9Cy5YnXG5ZScsstt2C325k2bVq4Me/vxxPAuVLK34UQ3YCngV4neU1hwhyEaaoos6b9GUuWZLN9exmDBqUTE1PzDLCua3z2WU9WrSqmY8e4o05MBALw6KOwezc88gg8MwWeex7OPx9c0RAMqXHf/wZvbFTB87j+MO4A+f8P8+C/2YCEpEiDh0JeVsgQFkwaaYJoRy5WzYcVQRFJSCQapfjJ4h+0wIeVFFzoB1xsN/Cj8SNReHERS1u6YdKM3VxCkBJySUEgaMFKPAg8BJFAkB3E0hs7+9PYAgMNgUYQF6UYzMVLV2Jpxo+8Tha/k0gLlhMkgQhseEkiiWWUogNOLCThI1OU05z95+jb9sJ35eAU8FAETNmgNJ73VsDMnhAIwZ5iaBxftcxbfiG88DokJ8BtN0J1bTLp6VYiIzXcbpPevU+O5F+dBchSypAQ4h/APFSz43Qp5QYhxKPACinlnMqhVwEfhJtC/toIIbjyyivZsGED69evJzKy+kJ405RMnLiRZcuKefDB0+jV61AFDCEEyck6X33l5aOPvFx1lZMLLzx8sVMwCNOng9sNt9yi6siOvG6VQZg4EZ5/Xn0Qrl8PK1dWv4+mCZo33/9VeebM3YRCJsXFIRYuzDluAfKmTYXs3FnC+ec3xuE4/FtVCMETTzxBdnY2qamnjs11mONGSEr5O4CUcpkQIuz6EuaUYsOGfK6+Wpk6vvvuQNq3rzrL8Ecp3uTJb3HDDd8RCBgsWrSXd945/6ieLy7OTp8+9Wq11q+/Vtq7Uipzipkz4R//UNs85fD5j7B0A8hkCBaq88TO/IPneC0bkqMh3y2Rrd0st5q4ZYBGzkz8AuqLIFaKcYky8nAxkx1sYANWLCQQz22MRP+Te3yAEkyKaIyDEHvR0fDyKzbysBKiMRkEpI3IQAUJITf51lS81lQig5swQpej2R9E6J0ASOMSCphHgEzAhoGXQn7CQhxZbMJOBPlspR5dyKOY+sQznG5I1pKNnyJgL+W8yVb+Red9a1ztU4GjV8IfisJSgssC326Daz+AkB/ObwrpGsxdDkN6wCNXqeP46HPw+TyQJuTnwj1jq3azTU62MH9+Grt2BTnjjDqs5TgMddriLqX8CvjqT49N/NP9R+pyDWFOHA888ADnnnsu9913H//+97+rHbdiRTEffJCJpsE996xn2bLzqhxXVmYybpx6Cy5dGuC33+x8+GGIOXNC3Hqrlf79D9Yz/Phj+Ne/wDShtBQee6zmay8vV7+FUPseDZdf3pDvvsvD5bLSu3fykXeoAVu3FnHZZZ8SCBhceGETpk2rvkM3FAphsVg466y6Mx0Jc9L5s4pFck1VLMKEORHMmrWJ0lIfAB9/vKnaALlPnz4AlJb6MU2JEIL8fO8JWyeoK4S6rq4cNmp08LbICMiPAEcz2FYAnZuC0w7j/+QvOSQJnvFDq2QwXCY+YeLUyokSJrFCwyZMLBTixMov/EYimWgYBJD48GFgoqNSrMV8TSGzieVC6tOLXH6hKVeiYcFOM3QZgUEFFtNFlOHGGSgGHNT3B0CMR/jHI2UI6euHEK0hcipOS3uaihaUsgmdUkLYKKEcP8toSFcy+I14UricSynAQxIJ2LExkbPZiZuJ/IaBpCH7s7fLggaxkQYlbgtn2jV6xkNMR1iaD3e2ggtegZwy1YD25UbwbleGIW8ugBEXQONkcDrUOTp/F7w5HVatgK8+q/rvlJRkISnp5CkxhTWgwhw3evTowe23387UqVMZNmwY5557bpXjUlMdWCyC3FwfkZEW/H4D+589KwGrVRmElJRI4uIEOTmSJ57wo+swdqzJpk0WdL3qS3lHI9kGKnuwfj3k58PLLx/dvhdeWJ/ly/titWpERByft1RWlodQSBmKbNlSVO04KSWXXnop7du356mnwkIEf2NqrWIRJsyJ4IILmjBz5gYA+vZtWu24cePGAepK4tixbVm3roi7767ePKQ68vICvPzyHtLSHNx4Y+pRyW6edRbMmAE5OUrJ6M+kJcLufKVp/Mw10KyKRPXoVBicAEFLgJvIxE0J0VoAp4gggCSOLEKE0AiRwjYsBNCRQCMupT82pbRIIVMp4AUMIshlGy2ZxemhS8C/GOwZ2CuWkeD1EbIYRJSXI4VERlkReiJoTdFEK0yhI4IliHIPiI0Q6A1mHBExl+B1qeyPIIggD5McWjIILz8CpWxjJm24mQKya+5fcQAAIABJREFUsGAhjhSaEMUkOpKHj84k7HvNo0r9+C1QFh1iSb6DgcUazjyVYFpTBA4dMJTMqm5Rxy8YBKcNkip72SfeBVFOdZ6NjYGt21XAfLTn7BNBOEAOc1x5/PHHmTNnDiNHjmTNmjU4q1BYb9jQxQUXJPHRR3spKAjw3//uYcSI9EPGOZ2CWbMS+OmnAL162UlM1HC5BB6PpFEjccgbauhQ8Hj2l1jUlJ9/hhtuVG/SqS9CbZqsY2OPTyPhH/To0ZArrzyNNWvymTSpR7Xj3nnnHb755hsuvvjiaseE+evzh4pFmDCnKj16NGLJkuuRUpKUdORuLU0TjBvXodbP98AD21iwoBBdFzRs6ODCCxOOuE8wCN/9BCnJ0L179eNeHgXz10CL+lUHxwClhPjUnk0ZQSy4iaAcEDRHMIp03mErPjTqEU0MdjQcmJjcwK3YUSUDBm7KeBYdAx0/AYJIuRmyR4OZD3oy6K1w+S1gBiBUDKYfWR6PbDIVYTsXIWIQzlnIsoeg9EugWIkvWzxEBT8g0GAo5frPCAKYuNFxUc5rWLBjYMFHESuZxy98hYGgJ5fRkd40JQofIZ5gDT1IZokZyW4NMDQ0U8chBV5T2WYnaZBRAY/1hjs/UzbbDeywcQ/Uj4V5j4CrssTc5YTGqdCtCxSXwJ23n5rBMYQD5DDHmcjISN544w0efvhhiouLqwyQAVJTnTidOkKojuTqaNHCSosW+0spPvvMxcqVBh06aOTnS5KT92cNLBa4+ebDry8nB35cAl07Q0K8knmb+m9lFhIVBQsWwnnnKTm4k4kyFDl8D1Z2djZ33nkn55xzDmPGjDlBKwtzMhBCTDzMZimlPIqCojBh6obExCM3Uw0YoDrdvv7661o/z6pVbubOLaKszCA52YLFUrPs8aNTYOYs0DV4/w3oXE3iOsoJl54JU7bDAyvhtjQY8KdWmTfIZCFFgCQFF9l4iEKnI4mcRgo3cD75lNGRJmTRgnUspBnJWA+oOxbYACsaISSQhESULgD/RiWKaw1C3JNQuBmszWHbLyBBmCGEfw2c1h0cIArdiLXLQDcgXgNdgkVDGCESfJcSG/EAATLJYzwmbgzWkYIgRByNuI/ZTKt02BMs5QvOoCch4G5W4MfgZ5lPLqfRJspJdlDj7lA0H5YIUpxwhh2+2K1ULK5uARYBs3+DRT9BsxSo8Ksmvj+Y8wU8/JhSCbnqSrisGnVYKSVLl5bh95v07h1bK2OuYyUcIIc57vTp04fzzz//sEoKd93VguRkO06nztChh3dMKiszsNkEDodG06Yabrdk8GAvwaDkxRcdXHRRzbzVTROuuAqyc5W1pdMB2dmQnQUyAKEQrFwBp58OY8YoVYtTFSklY8aMwefz8eabb6Kdql/Bwxwvyqt4LAIYCSQA4QA5zF+CS4/VNg148cVMXC6dQEByySVJnH9+XI3227xVnQdMEzIyqw+QAZ7eCpN2q9ur3LDybMlaezlWBL1x4UAHTCLJoT2RPEF3AkADrJiYtCSVlqRi4CGWzbTkaySSXEqoz23gX4pW+k9SZTMqzB1YDD96/Qux+BPBGwP2CpAdIaK/+tk1G7J+ANMPoQrIexHy1kLb0fDdYAiWgh0wDYhKgIQKCEnEnuexnD4PCw1IYjKFjELgwYLAjaCY6dixUkYAAAODArLRSCBUGTT7haSDNFmrm5yj69wsrNx2gFjVP9vsv71uN/z8O3hNyHND8xRoeEBy3zBRwb9U59zq+PzzAiZM2I6U8MADaYwceeKbz8MBcpg6QQhBbm4uU6ZM4YknnsBmO7gEweHQGTWqSTV77+eLL9zceWcuEREas2c3pGlTG4sXh/B4JFYrzJ0bqnGAbBiQVwBWC5SVQkWF8n9HqIaNuDjIzISYGKWGcWCAvGWLl8mT99K8uYMHHmhQ44xFXbF9+3bmzZvHpEmTaNmy5UldS5i6R0q5z8amUsFiHHAj8AFQQ4ubMGFOPtVd7Zo27Xfef38H11/fnJEjD/+Z1qNHNEuWlJKcbGPkyNQay1o+ci888Bg0agj9+xx+bFFANZsZAPYQEywFrMOLA/gnCYwgFR972UEheynmFyJoTiY/8wkaJinE0oqrcfMyPjIw8KITT4Ac9QSlE8G7HfueTOxSgDUS9NZQ5oTAWWC3QP3K3tuSDFj0TzD8Krg0gYoiqMiFLf8Ff2VnXBDIBww7OKPVY7J432ty0Z1CgvvuS8DDZrpxK9/zE0EkkcQQQTRO7JxHfb4iDxs2gqKIL+lAMjr6YY53KAQISEyBMT1hTB9VXrFsFXz9LVxyAdwzHgoK4B+3Vn/8d+/2EwiYgGDbNt/h/1h1RDhADlNnrFixgmeffZbIyEgeeeSRWs3xwQdlBIMmGRkB3nmnmEmTUujf38r06UG8Xrj++poFxwBWK7z4DEx9GfKyIa9IlVIkxYFVh5degpemwq5dym70QO6/fw8rV5azeLGHM8+MpH//2Fq9nuNF8+bN2bhxIw0bHj77HubvgxAiHrgLuAZ4B+gk5QFnvzBh/qIUFfmZMmU9DofO44+vZejQJkRFVf/ZftNNqZx9dgzR0RYaN655PVzr0+Gz/x76+Lp8WLQbBrWAJpXNZPe1hPwQ5AXBckYBy3UvFUishPiITHaSST0iyUZHInGgsYGPMPFjAiXksp3pxJOPhVhMAkSH2tIgczWEekFMY/AuURppUkKgDFb+B7ZkqAA4qh34roCBU2HNfyFnF9hQUZsfVU5R5oItn4ALcACaFbRoiDgPks+E0u+g0f2wayy4f0LUv4+ouAGU8wVuLYqAiEXHQPItN/Ike9lBAvVwVfb/3sTprMSPHxOn0KmHjqjSJHk/910EEQ6IccLoXpUJKTdcPw58fpj1Bayar+RVD8d116WwerUHv9/k9tsbALBiRSHLlhVy6aUNSEs7jq4k1RAOkMPUGRdffDHXXHMNjz/+OFdccQXt2rU76jmuvjqaTz4pxjAk775bxK23xtOsmZVff43ANKkykxsKKfH3jRvV7/bt1eNeLyxcAFmZ6tur1QL/dx3ceD3cdRdMfxNee02VX/xZSjg11cbKleXoOiQn1zworwuWLFlC9+7dSU9PP6nrCHPiEEJMAS4HXgPaSSk9J3lJYcLUigsuuACAhQsX7nssMtJCSoqT/HwfDRq4DtuXAuoKZbt21WvtHw2bC6HbDAia8ORvMG8odIiBZDu821GNuQqwIfBiEk2QfLLJooRMiriMrpj4aIafxVgw8QNgw00TuRprIJ5AwIfDeRPx7ngonw2F5ZBTCJHtwfcraBKKgdwN4AH8Eop+BWsEfHoHdBgIWhS4/WBIKAQCwO/zoaEOPouqO255msoaNxwIi8aBNMD9NtjngxDIwtFEWW1ECSsJtm5schQSwIMFDzoa6bQ66NgkYOOftOQZsihEZxUVdObwgWmsCx66pHplipoaXsTHW3nrrdP33c/J8XLttUsoLzeYOXMnS5ZcWMOZak+4cDFMnfLCCy8QFxfHiBEjCB2u4KgaLrooihYtbDRooCTd/P79Tk3VlTn88IMSfl+xAu6+e//jc7+A2Z+pRj23W2WU27eD2bNh1SpYu1aVVjRooPSQD+Sppxrx9NNpzJjRjE6dqv+AWLeukPff30pRUd1cEpo7dy7nnHMOM2fOrJP5w5yyjAdSgQeBLCFEWeWPWwhRdpLXFiZMjRk2bBjDhg076DGbTWfu3D785z9n8fnnfbBYjm9oUlYOc36CHXsP3bYyRwXHMgLy6sElqyUXbZW8WSb5w79sLA4SKKEeRSRRQBL5+AkShYMzScPkNVbxME6KiSWJBrSivdxDfGEJCVkrqJ+/kfjdj4AZCWUhyC+DvEzwtwa6w2YgFxAO0GyVAbAfyosgYxvoaTDoNRj0DvjiVQbZB3gNyBXgSoWzH4DL18Dla2HnHCgvgIpi2PUdYAPfNqRZjB7IRfdnY/GvIoYoBCYV5JDDl0gkC/mJKbzKdygn+82EWIHJBoKMZg+zSiVdt8JdWSpWr4r734GmN8HY11RyPDoK3n4BrrsC3nvpyNnjqggETAxDYrUKPJ4QJ8JbLpxBDlOnJCYm8vLLLzN06FCmTp3KkCGj8PtDtGgRX+M53n67IW++WUSfPpGkp+9/Z339tY8ffwxy3XVOWrfe/69cvz4UFSltxkAAXn8dLrsMGqQqpYuICLh8MNw8Cjp1gi+/3P+GrS7J7XLpDB16eBmhzEwPQ4fOx+czmDlzK3PnViGweQyUlpZy66230rZtW6688srjOneYUxspZTiZEeZvwU033VTl44mJDvr1a1Anz3nDZFi9VdXCLnoJUg44/VzYFFomw6YYsNqhwITFxbDFDqfZJOc4BJvIoRFF+AgQQSn18JJEPKPoi5csfOQCEoFBQ+rRgUm4jY1YfNsqa4ZNJdH28wjwJMHeHPC6wdwFHZ+A1cNBN0GvB5feq3TmCiqUB3EooGznWg9W0ebmVTDnRfblYgNWuGI2RCfDvweCEYR26arcwgxBo0sgNgi5vyNMqco3NCshuQeNIHEEKSYGCFGBl+WsxoadpaykE2dgqXyeP3JGj+SoKeaUwfVx0OEAoapACKYtgNfmQ6NE+GI5/PNKSImDszqrn9qSlhbBlCkdWbAgh5Ejm9e47vxYCAfIYeqcIUOG8Pzzz9OixXlccMGHmKbkySd7MWTIaTXav1MnF506HSwftHu3wdixHoJBybffBli2bH/wevrp4HIp2bacHFVm8eWXKjv87ltQWAQX9lMZZICLL1YlFcEgdO1a+9dZUuInGDTRdUFOTkXtJ6qGCRMmkJOTw2effXZI02OYMGHC/J3JzAxSVGTSrp1tX3BUVKRixoQjSCBv3wsWHXwByC/eHyCbEta4IbYNWCrACCmZMlesRI/dywO2UgYQS0c07GRgwUIM4MCgJSv4lU+IpIgIAnjQseIijSsAiNTfReq9QKxCeIFs4PdiCBTDHxdTV/wKu16EUFPYvhmG3AhNL1L1w1u+V5GoI1KdvB6YAF17Q+8B4HeB5lUvfuAdkN4JvnoStv6kfJ7tLmg3Bvb+AnoUZHwENtQ6DAfSUg+Pw46FaMBPKsOox6VIrMQTRzGlRBLDXSzHAK6mEbvQGUsyzzsFSyogSoOGf6o2fP17eHaeUrDILITup0FiFTbStWXw4DQGD047fhMegXCAHKbOEUJwxx13MHXqCrzeALou+OmnPTUOkKtC01QZhJQc4qanaTBihPpMcThUdnjlSujcWdUjf/zx/uD4Dzp2rPVS9tGmTTx33dWeH3/M5s47ay+AXxULFy7kjTfe4J577qHrsUTxYcKECXMS6d27NwDff/99jffZsMHPFVdkEwpJxo6NZezYOJYtg+uvV8nZ118H3Q7P/wfOOwduu+ngMrnnxsIzM+G8TtDmAJO/GRnw2CbY5QChgbDAxHSwxRp8EllKkqbzLaU42EUiAonB+aTh4R38FGHDjR8/Dqy0oBHpTEVHRd9CRCKSfoBtw6DwW9juUwoTEtVQVwzkVcD2zyFkB0cCfPw2vPU+FOeAHgOuCIhpC98vUNH8gs9gyUJl9WfkQXITGHA7VHjAEQP+cqWjtuYbKHYCZZC5DJoYECXBbgXjXkTceFzacgSLiOJK7HQkhB8NuJGh5FHAj5ThZS8agnoEmFhZn/xaQ1jpheZ2SPhTBBk01HFPTIHrzoaHL1cKUX9VwgFymBPG+ecn89BDLxIXdxY33XRsJQKNGum8/no0S5cGGTrUvu/xPXska9ZIxo8X3H+/4L33YPly+OYbiI2FDRuUSkVdKKMJIRgzph1jxhx9M+KRCAaD9OzZs9ZqIGHChAlzKnDDDTcc9T4bNgTw+SQWCyxe7GPsWFi0SDVeaxp89RXM+xnKK2DNBji/J5zeEr76Ve1/UVfo0+XQeXeVg0+AtAImpFhhZD1BvM3CblxsxEtrnDQmgTyK0NBwkk8ZXgTgw44DH5JynKEV+LQXidAmqZIIfzHY46HF57BxJBR+AlK57RHVBPQGkLNUBb4VAZBBECVQLMAZBV4NXvsVPpsB3y1QCzaAEg9oTugxUGmTXt9Vyb0l1ofIKDBLIOCDXT5I08FvqAY+K0AQdj8Kll1E1HudCNEHiWQ5r7OTZUTQkAsYTyNS6UYE88gmhORsUvYdM7sG3atpw7m5twqSAW7rA7aT289+zIQD5DAnjDZtGtG9ezN++mk2kZGPAklH3Odw9Oplo1ev/aUGZWWSSy8N4XZDWprgxht1WrQQ3HIL3HsvfPQRdOgA6enqg3XuXKhXD3r2PLbXdSIYMGAA/fv3PyF1V2HChAlTV9QmQO7b10XHjnb27g0xfnwcUiqr6PffV1cRhw+HDbthw+/KACo+DmYsgkmVvcx5pTCin7ptSlhSAPE2GN0UFgWgxA5RwqB+w2zusRk8QD2eoQk5BEjBVqnv0JAYXDgp43vm4yeIJoPYcdCyOIO4/HyEMRWEH7Yvh9IdkHYRuOvB2p8g4ICIaHCXwgYJF18GviCsXwseO2QXICOSkJYIApt3o3XoirZjNybRWC66Fm3eB0gzpOSXSosRX34MTjtEG6AHobQI6reC0uWV0nGoOuRITdWOaJXCzgLwfYfX/y4eRwl70djJdwAUU8YOltGaC7BgIYCTECYrKaMdR+4bctpU5jghSi3zr87f4CWE+asghODVV1+lTZs23HTTTcyfP/+4BnxFReDxqJKK334T7NihSilmzIAnn1RBcmysyjhMmACzZqmmvRkz1IftqciSJUtYvHgx48ePx2IJv13DhAnz1yYYVEYV1j/XuR2GuDidTz/dr705+Ql4622V4Ph8NiQmwoxpsPB7aN8G6qVAbkmlaxuQV7J/rhc2w8vbQBcwoxu83AqGZkEo0o3hrGA78AYFPEkDGvLH1UlBK/7QnI/nUl7GY6zF7h6IRbrRih1oQSsEy2DPFCgSYKsH22bBWp9qlotOBG+6uqTp3w07HoVXF8E914G1FEwP/oIAwewcsNnR1m/GGDIQdB29YSOcP2RhDO6DnrFOBcB2DRHwg89UOsjecmjeA8qssGs5REZD2lmgrQGvBOcZYFkDEQEMm4ss+1tITPYSi0BHItAIkUcGrYEMKggi0dHYiBLKCZgwPgPWVcDkRnBO1MF/pwffh/eXQNMUmHOvaor8KxPujA5zQklLS+Ppp59m4cKFTJ8+/bjO3bgx3H67RoMGEB8PRUWSQEBSWqrqouLjVXAcDMKyZcpJzzCUJvKpiNfrZeTIkbzyyiv4fCfHSShMmDBhjid9+/alb9++xzTHp58pvfq8PNiyRT0WHwdDL1OlFQA394fLzoZBZ8HNA/bvu7ZUZZEDJmz3QHs7zG8IT8TYiNcEOtCS6iM7D69TSC8w78Fu5mORATRHBWBBGEKZwmsW8JbA737I9kKODzYWwXdLwONXUhlZZfDGC/DUu9B/KJzRi1BeKdLpwvD58ZV58GQV4N65F++mzUh/ALlxEyG3TqgUpGkFYQNTB68FPAbMekGlw1NaKFWL7ndD40HQuBXI9RCyQuQYSP4QhPqCEoPyGpJIAkTSAOUh3YU42hFNDFauozEAi93wdQnsDcBDew49Np8sgygH7MqDrdnH8hc+NQinpMKccG655RY+/PBDXn31VUaMGHHcsshCCMaN02ndGkaODAE6MTHQr9/B/+bTpsHOnarM4txzoX//4/L0x51JkyaxefNm5s+fT2Tk8RHFD/O/hxBiOnAJkCelbFvF9muAeyvveoDRUso1J3CJYf6HGDVq1EH3TVOiaUd3Dhg1Ep5+BlqdpsrmqiIuCl6swsr4ntNVvJrigEsbQAUGLqvBUFycQSPKMOiEUk0qYy9usoinHgF24KI9HnMKTnch1lAQAzuWYj8U1kekTYX8eaB9DlKDZdlQXLG/3KGkXKlSlKFULHQN1qyE1p2gdSekaeLrcSbabyvxGgJPgRtME7vDga7ZEMkpyOhYREkRMioWOXAQ/LwAvPlgNZTLHiasXwQxFkhNhJ/ehAG3QO4LUO5VGssyAt3ankiGk8dbCEys2AmicQ5jcZCKgYkLC4/Q5qBjl24Hq4CghA4HC0sBcENveHUBtG8MdhO27ISWTY7qT3tKEQ6Qw5xwNE3j/fffJzY2tk5qamNjBTabJD4+SI8e+iFdtIWFKpMcFwfnnVc70fK6ZuXKlTzzzDOMGDHimLMtYf7neRv4NzCjmu07gV5SymIhxACUW1+3E7S2MP9jXHvttQCEQpKRI/fw44/l3HZbAhMmJNd4jtG3KAdUm61qt7bD0ToGvumlbufg5y42UUGIETRi4AHNaOUUsJh/YeKjPltw4MQmY0n0FhJRXgIINNEefs9TUhqFd4PrZtgAZOdDqR9CmnLJwwoFQZVd9gMOp9IrPne/G1zhSy+Rs/w37CYYSMxK/WFfIICtUyeMggJ8Fw1BrF6B1QwRXLgYYTfQApVW1VZUROcAIg3Q8yFzLsz/BrQiSLVCTEdIvgofW8hnOiZubAhsFOEmnbdYRBBJU9K5lWGH2Eo3dcCXp0FGALq5YPZmZRZyWUuwaHDfZXD7APh1DQy8RS1ryr0w+DCnMJ/PZMmSMpo1c5CeXnPb8BNBOEAOc1KoX78+AOXl5WzatIkuXapoMa4lXbtqvPmmlYwMyeDBh2rMjBunnPQcDqhFv0idI6Vk1KhRJCcn8+yzz57s5YT5iyOl/FEIkX6Y7UsPuPsL7Cu2DBPmuFNRoTTid+/WWLy4guhonWnTChk/PumoEiYOhwrAlmwGjw8uaKeSsjUlFx/Ps5UCKojExncUHhQg+yjGxEBDImU5QoYIUEJkrhfNKhHCgrC1rBQXrlAacZpFLcpphww/uA2lYyycyMIiZMhEREUikupDkxZw1yP7nq9w1izKTWVUbWe/MYcpBKXr1lHeqxfOoiJsRhDNYqDXS0Z4yiBCU7WCPqFqkU071I8GhwsC+VBhgEOqxxO2QGE/ZML9CNsfdccgSKCERPyYlBLFUjys5Hu6Up+RtMSCxrIKuCML0qzwekP4YANMWqLWWFABozup2xEOWLkOfH715WXJysMHyGPGbOPrrwsRQvLdd2dw2mlVpKZPEuEAOcxJZeTIkSxcuJCNGzeSnFzzDMKR6NWrevHF+Hh47rnaz11RoXRsXK66EXgUQjBt2jTKy8uJjY2tk+cIE6YaRgJfV7dRCHEzcDOofoIwJ45XX13FnDlbGD26M5dc0uJkL6fWXHSRchj96qtvSUuzkpERpG/fqFpdTZy/Fsa8pWLScf1h3IAj7/MHU9nGJsrwE8KCzuADgmOAeJqRTm8K2UJsaC2GyCKhtBiLTwe3AwwXZGdCm0ehYhs0GAjWNPjgTcgqBy0ezFLw+DC69IONc/BUgLvEi/PiAcQ98wyeX37BkphI0OOhYPVqgqjGsKAQ2AFd09BcLvTiYkLl5ZQbBlLT0KIcRBoS46x+WNbPqzQGkJBQH1JSINkKuRshsRnU86gsdkoUWEyQHhzeLSTbbsLNciz0wKCCZNLYzQYkgmISkPj4gVw6ygT2+OKZVCBxh3RygoIFHijxq4oRpLoN4KmABT+DMwKapSkn2xFDDj7uUkrcbpPISA1NE/z8cykFBV5A8sgjO3j//UOqwE4a4QA5zEll4sSJfPrpp4wdO5YPPvjgmOYyDMn77+dTVmZwww3JdRLA/vprCf/3f2sBmDGjPV27Ht8A1u/3Y7fbOeuss47rvGHCHAkhxHmoAPmc6sZIKV9DlWDQpUsXeYKW9j/Pnj1lTJnyMxaLxp13LmDAgGboR5MuPYUYPXo0AC6XxldfNSErK0iTJkdX5yYlrMyAxdsrzSmA7XlHtw4bGhqCJGw8xGl04ODPcoFGW4YBEPD/B5GfiwhK2K0j3BJCQTAzYO9P0GOq2mnraihxQ1AgywrAr8orxJ5MfM54SnPzkITw/Pe/lAUCZM2ejQgGCZimkmBCSR17pUTY7UR360ZMjx6UvfIKIiYGSkogNhbZtg12ZwVi5VIIGRBhgBNwREDXNpDxHdhc0OYisMwCMwb8UaCp5I5wXEQS3UjiBgAaYPIDv9CWRuQgqEAjgA0dwa6gnfvLQhRZwHBIUv1WWtmhX3vYVayy9mM6wfS5cO+LUJwFVh3GXg9PTTj0uN9zTx4ff1zGWWc5ee+9BlxzTRKPP+7GatVwOE4tGdNwgBzmpNK6dWseeughHnroIYYPH87gwYNrPdcnnxTw4IMZSCnJzw/y8MNHl+HKzAzhcmnEx1d/4pk7Nw+v19h3+3gGyKFQiJ49e9K3b18mT5583OYNE+ZICCHaA28AA6SUhSd7PWEOJibGTmSkDbc7QKNG0Ufd1HYqMWzYsH23nU6NZs1qpgVW5IFHPgFNQIdm8Pg8pUbRJh0sTnC0gqX50L0G8voLWI2fDXQmkd50PCQ4PgjfTiy5ZyAK50NAQKEANGUGoktIqizXX/AhvDoJCnKRIQ94BZRK/H6DrKxt+AtL0CXogOb1su2ttwj5fAjAqmmVpQ6qpEJYLFQEg/iXLUNERxN38814X3oJdB0tIoKIerGwbh1UuME0VE2GATTuAo3awe8fqvUVrYdEPwRzoKwQmr8DUf1AiznoJW5gC/P4EROTCGKw0IVsIJ1krKYTE5MoDTpEwMupkGaDt36GWT9AlA3u6ATTvwDDr36kBrO/PjRADgYlH31URny8zvLlPvbsCXLffWk4HJCZ6eeee9Jr9L9wovhrfgUN87fi3nvv5YwzzmD06NEUFxfXep5gUCKlRErw+80jjs/NNSgqUuM+/LCC887L55xz8tiwIVjtPgMHpuB06jidOgMHplQ7rjY8//zzLF++nLZtT51LTGH+/ggh0oDZwHVSyi0nez1hDiU62s6cOUN55pk+zJp1xV/aMKi0tJTS0tIqt635Ha68AyZPU31vB/LqIvhsBczvUTv3AAAgAElEQVT+Ff77CwQMpXPcsw1kNYEPs+DGXyDvCIqYQQwWshYrGhXk0YYqal79P0NOF8jqDJvPQ9v9LcInEIUgKkIqKA25IGYENL9K7fPao/D7dsj0QDZQJJEBKCi34S8qQxomXqBc09CHDydUKd0pAa/FguF0oqenY2/aVGmRmiam34/niy8off11EAJLWhrWQDm21UvAXYI0DIiksjkvAq7/JyQ2VLXIkUD2FxDIVTXRCYng/vGQ4LiEEn7ndwxMQODGSzaSbCL5RvqZahZQXKYTLNQZErTQsFK++vEvICsbNu+Cez+EoX2UAaBugQgn9Drz0MNqtQouvTSSkhKTDh3sNGxoxWLRmDAhnRdeOI3U1FNLODmcQQ5z0rFarUyfPp277roLt9tNXFxcrea58spE8vODlJUZjB2besj2oqIQwaAkJcXKV195ueOOEiwWwXvvxfPll14Ayssly5cHaNOmahH7Ll1iWLmyB3B8a5C3bNnCxIkTGTRo0EEZljBhjhUhxPtAbyBRCJEJPEyl8ayU8hVgIpAA/Kcy8ApJKY9f12yY40JaWgxpaTFHHniKM2jQIAC+//77Q7ZNmALb98CqTdCzK/Q84L8wJWZ/E96A1hCxWwWXTU4H3waVWZYoVYU/U0I5RZRSRjGNaUgaiWRSRByRROE8eLBZAfmXg5mrajkMDbIk2CRICwQ0pUbhFrDpvf9n77zjo6jTP/7+zmzf7CabHhICIXRCUToqYAMbKqKAZwGVQ7Fyepz1QE7FQ+HU87DwQ+XUUxTboWdDFCuo9CYl9JDek+0z8/39MRHEBiJIcd6v176y2W+ZZ3cnm88+8xTIGwAdT4G8TsiV65ES0EGGQFfdOPudROPniwk3NFAuJTavl1Y33oj6+usEq6sBUFwuEgYPJrVrV7Y+8MBubzJNPw2XCyMSAVXFnZKI0CpNr/G3/yrtApoHoLEMqpaAXQOMpnHN7KSnRiFw+d5PFYNn+TcNNGDDCTjIoStrzI8HYobKOk0SlCqNO+D2HYJIBK5uBVKDpkIbrNoOL46DkafBjl1QXAaDTvrx9//RRzOZOFEnJUVFVY/sL3qWQLY4IjjuuOP46KOPftUeDofC+PHZPzq2fHmYSy7ZQShkMG5cCtu329B1CIcNPv88ytixCXz9dQ1paQqnn/7z32IPdmyzYRhcddVVuFwuHnvssaPaO2Rx5CGlvHgf42OAMT83x8LiYHHjjTfu9XttAzw+F1ISIScTCneYMawZKeZ4RDO9xaP7Q5rPbPp0Vjf4k4DBq+GucnAnwzAnnJkFWd/Tu4WU8DQLqKWOAJI03IxhGCVsx+BttvAuOfJaPLRBCA8QMxPekKY6LTSgATNuQGZATicojkLRZjNeQjVllDb0JrTn56Iq0FgHceEm4fTTSLh3KpuGDKEuFkPabMikJKqXLCEcCBBqEshqQwOlCxfiTk1F9fmINTRglxK7w0FCejp6ZSXqccfRbP58xNefY9x5HbIyiKIbZv1jpzQVefEG0750wxTQdkAYEMgAnwccZiJ8lBDLeYtSyqiiCgNBEjbaM5SZ1KIguZQk5gTtyNqA+aWjEmpDsMhvCuQHLoTLZ5kv05+bkiPTk80bnX/6/RdCkJ5+dEjPo8NKi98NpaWlTJ48mQceeACfz7fvBfvJ558HqanRqarSmDKlnPPOS8LptJGUpHDWWW7y822sXZuBEPzmAnXNmjUsW7aMGTNm0KzZDz3fFhYWvz+klEyd+iVvvbWZ6647josv7ni4TfrVrFwDWc0voM93PMP3zoKX3zcLMUy5Hs4ZAPnNoV0ebK2BC16GhhhMHwTndd+zLmrA5gi4BYRUuLkTNHNCOSGeZR0+HIyiI4WUYBAikUqcSAzsrOU6NOpQCZKgg2gYBCQg3fcjnMMhMAvK/mjWKlMTwVYPoTqoj4E/E1qcDBv+Bb3ORSuJI1/6KzI9k8ZqlVhMJyqhLiuJ2s07iJ1zDno4jBoIEKuqQvV4cLVsSWNRERJTgysuF4rLhaegAHdyMno4jD0SIaF9e2L33YcIBKCoCGPLZmzTJ6DqleBzQpoG9jg4hBkw2284aDthvdcUzNihdQ+wl4GSQlx1E2ILhayhkC+JEMGPlwZ8tKEtG/m2BjO0QOWfahqTgB5R+LTGdKhv3g6cAMN6wtDuZpKkc/+7hh9VWALZ4ohi69atPPnkkyiKwowZMw7avmee6eORRyqoqgK/X6G8PMbq1dkIwe6Elx9LfGls1Hn44XJUVXDTTel4PAqhkE51dZzsbOdBEdNdunRh48aNlji2sLDYzfbt9fzf/63C6VS4665PGTGiw1GdnLfgE7j6FtDjldx0DYy/JhUwQyO+jSdwOiAagJVBaB+H59ZCRQg8dnhxDZzXbs9+TgUm5sLMErgiFQIOjYdZyRJKkYCXBqr5DBsV5FCMn1oEAj9hIlShkoBhRMmvWI1LC5meWOUZcA4HzznQsgjiZZAdh48nwNfvQigOVcXw0t8gGESueAyt5jmMeIyqYJxIVg7uqkp2xHWC1dXoJSWgqkRUlbAQ+Fq14rg5c/C2bImzWTNC27YhpETxekns3Jnc4cNxpKRQOGgQDR99RMjtJknXMWIxbMlJqBuXQkMVJChmFY0E0dQdz4D+l4IvGTSXGQQcDYIvhkw4g7i/E4a9C18q9xClDkkKxXiROAhjJ0giWXShG2msohEnCqcYAe5YLthZBoPTIMtlevLz/HveA0Ux34djFUsgWxxR9O3blxtvvJFHHnmE4cOHM2DAgIOyb36+k5Ur23LzzSWsXx/l7rsz9iv+acaMCmbOrEQI8PkURo5M4uyzV1BZGefqq7N/VdatlJL58+dz+umnk53946EhFhYWv09SUlwEAk5qa6O0a5fC0RB51dgoeewxA48Hxo5VcDj2GL2h0KyLW77lQqbdD+OvWQjAXWPMy/LJidDgg7vfNT2VL+2AtUGojEGqgJ1pcNU2mJYDgSblMjrTvAEsopyVVBDDQBIhl02EieFAkkgMFYGCgV1GcREnKqK0jZ2Kw9gKMg6halgThtJO0Ho49JwIjmamcP68GlY2mj2WFy4Em4toeZBoNSieGEFFZVdpNbg9JPXuA9u2YautRY9GQQiiNhuO9HSi4TCVq1cT6NqVtmPHsvpvf4NIhGhtLY2bNlH+3nt4FIXgV18hhUAPhbD7/ThS/SR5KxGTrzabfqRrZghFAoAKva+CIZfAksshuS80BzSQKgT1f7DZVYCgGWFUQgTRqKeBPugIGkhGEqCQGvrRmucxr1RsC8Hn5ZDshPcq4MWzYHs9nJ3/m5xKRwTHsPa3OFq57777yMvLY8yYMbu7Lh0MPB6VJ57IYeHCfPr08e7Xmvp6nWjUzERwuRRWr26kqiqOyyV4/fVydF1iGAdWDnb27NkMHjyYN99884DWW1hYQHV1mGhUO9xmHHR8Pidvv30hM2cO5qWXhvxmoV87dgTZufOnP3eDQYPPPgtSXf3D1/yhhwz+9S+DBx80eOEFswxFbT3c9gAsWg+tO0DBcbcw6a+37F7jT4A/Xw5XngchzRTHEigMmpfumzWHLn1gVwDmN8Dc7xU6MjDYTgWJqNhRSMDO8aQRwIkNgYHATiYKAZobNvrEFtOpegV9tpaT3piDKpqDZodiN2Lj56CH4ZunIVJpHiAeg01LQWv6nNd0pCYIlwmMuELcEATz2xNDEA2FKFm5EvegQST16YOje3ciWVlkDhmCISXYbERDIWKNjeSefz6KophPWNOI7tzJtssuY+MVV0A8juJw4GjZEt/UKQQCIRR002vs00zlZmC+UDkGtCiHz06C4ldh04PgPQVpF0gVNqVkESRMNTupRbKefFZTgIHEhQsfHny4yIu25txCGLPdbACY7YGOSVAXg0FZ0C8HLu4I/iOr0MQhxfIgWxxxeL1eZs2axamnnsr999/PPffcc1js2LQpwiuvVGAYBm3behg1KoVwWCc/382mTSHOPddPp04fkZRkZ+7cHjRv7t73pk0UFxdz8803079/f84555xD+CwsLI5dnnpqGVOmfEpqqpd580aSkZFwuE06qKSneznllP37Mn8weO+9Em64YRkATz7Zg5NP3ruUpZSSESO2s359lLQ0lQUL8vF49vjZlKa79fUwYyZ06Qb/+wyeegNqNUjywz9uG8JlZjM9qoKQ6AJbU97z6B5QHTIT83wt4Ik1cHwKnNAC1leZgqXl9wTaqyxiGVtwYudmTkFHoQMpFJLFLt4kjc0051ISOYGYMQ09/jHO4npE5BuouB5qUhBhAfjBFoPaHaA5YPOXUHAO2B3Qfzh88CzUR8yQhpPPQZQtQMY1lBZ5+G4cj/HVEvRolNqqKormzsXWogUV27YRj0bZOncurkAAFfhy6lQ2v/02573xBjlDhlDy7rtoDQ2443FsUhKIRnEpCs6ePcn4+GOUzevgOT+UN5jCWFfA6QQ9ArkSkiVs+y9kqpAQBj2KTL2fCF1pkP9HxO7CrNwvKSObenwoqDQjnRPpSxc6oCC4qhRWRUCGYV4dXJIMrw+E0jA0O3K6P/+mWB5kiyOSU045haeeeuoHGc+/JTt2RNE0SExUAIndLvD7bbz77nGsX9+PXbtC6LqkpCTCBx9U7Pe+UkrGjRtHJBJh1qxZphfBwsLiF/Pii2twOFSqqkIsWVJ8uM05YpFS8umnxSxaVIqUP33F69NPK4hGDaJRnc8+q/zBuKbB2rURXC5BeblOZeXeXuQ//UnhgmEKNq9CVaPCzXdAot/sYSExnaWLlpVSWlrKfR9Az0dg8CxobGpV7HHAXafB8P4wywC9Pbhaw/hMuL9FjOl5Edr565jKIp5nDToGmyhBpQ47m6hhHTovsIHZtCSZLN7DxiZK+BsGEWzqBQjRDKE3GSM1qK80lbpMgBoF1huw0wPr50M4BI/cA9EUtJvfoCbvYkq8x9HY9Sx8i5fhmfEkvtfnkXrBBejt21PndlMrBJGaGspWrKChqopIYyNISSwUIlxXh+pwUL12LRv/+U8yTzqJ/NGjyevfnyynEx+mKJMuF6K8HKOsDNoUQPs0aC2gpQ2ONyA7Bp1TzNgTO9BBQisNMiWyfYBt3n+zMWEhFb4uCKEQxUM5mYCBghs3ifSmB93oiNIUAN7OaRblcCjwbWNDmwI53qY48f1g69YQV1+9kqlTC9F/rN7eUcYh9SALIc4AHsF83WdJKf/+I3OGA3dj/v2slFL+4VDaZHH0cOWVVwKg6zqGYWC3H3iqrGFI/vKXlbz7bgnXXdeGceNa73PNSSf5OPfcJNauDXPPPc13Py6EwOEQnHtuJl98UUNCgo3evfe/dvNLL73EvHnzePDBB2nTps0BPR8LCwsYPbobkyYtJDPTS69eVhz/T/HccxuZPHkJQsCDD/Zl6NBWPzrvkkta8v77ZQgBI0b8sBOp3S646650Hn+8mosu8tG8uZ1oFG6/HbZsgXvvFVx/vco7H5vxxrk5MO5icDhg9jtmnPGy/41k5AdQPWQhCU7YXgPryqDXdw7XaJj6VRFQp8NXopb/+LYC0IoagkQopIZOpJFOLXV8gw2ddcwlhzoUIIEgUlYjpcSmRaEoBUW2wJXzGoSHgbERqjQo0k0FX1QEZS7TZarUwMAc+OcU+M+TaKqNugcfpa4mjFQUGtfcQGTwYFpPnYqjKbm6x3/+w5qpU/GUl7Pls88INTaaLnXDwJASFcg56ST08nJSUlJYP20aRkMDWe3b41m+HBGPI4UwvcOKguPEE1FzcszqGdRAq05Qvtns3ucQQC0kOEBEwa+A3XS06GqIehYRRVJInPWcRBg3jfgpJY9GPARwcjmtieiwug7a+eDPGdDDC8kqdDtAj/Ftt61j8eIaVFXQtaufM85IP7CNjhAOmUAWQqjADOB0oAj4WggxT0q57jtz2gC3AydIKWuEEEf3q2lx0AmFQpx66qkMGjSIyZMnH/A+27YFeeONItxulQcfXM/VV+fvMyPc4VB46KGWPzl+4YXNOOGEZNxulaSk/RfvPp+Pc889l/Hjx+/3GgsLix9y6aVdOP/89rhcNmw260rMT7FxYy3xuBm0unlz/e7HV6yoYevWIIMHZ+Lx2OjQwc9XX53+s3tddVUKV12Vsvv399+HN94w70+aBK++CnOfhU2bYdApYLfDNSPNG8D/3r4NzYANXnh8EbRNhU6Zex+jrxduyTBz5sanw7PsJEQFAiflhBFE8GFDUINkK67dPmqQCAQCFzNxyEqiUietsg5FaiC3Qc1zkD4OFkwwBfLujhyaGVqh2MCbAsUlyOdfRJZXEYtIog1glxA1DOKNjVR//jkbJ06k67//DcD25cvZUFhILBymqqlLHoaBarMhNA0BNGvThrK1a6nfuhWhaRCL0bB4MXZVxSYEOBx4Tj+dtKlTcbRvb5qmKNCqO2xdAW16gXMbxKqgfWs4bo2p4jQ7GAJcGahJU/GIr6nnI7bSC4nAjkYUB3X40HDQaHh5vjbCR+u8bAtCpgvmnwin/MrKqunpZvyLoggCgaO/9tuh9CD3AgqllFsAhBBzgPOAdd+Z80dghpSyBkBKWX4I7bE4CvF4PLRp04YpU6ZwwQUX0LVr1wPaJzPTRUaGi/LyKD17Jh+0cklZWa5fvObss8/m7LPPPijHt7D4vZOQ4DjcJhzxXHttAYWFddjtCqNGmbXS1q2rY8SIL4jFDAYPzuKJJw6seWJODthsZvhF69ZQXQe1MRh0Gvi+Fz5d0gj3lJ9BZRjuHwhXDzOdt8b3vtsIAePSzPs6BoWUY0OiEyKBGtLZiIsIH/IpAeJInPjJ4ATOQ6UKG25sTEDK7TikwBnXzE0NL2wugcK5QGsIrjGrQQjA0RxunwNz7oXqanj031BVhyFBVQWKEESlQY2qUiUE5WVlFH/wAc45c2g1ZAgf/fWvNJSWoofDe56IouDQNFRAhsNse+opPIAiJQ5FwY55eD0tjeSBA0m7dATedq0gv73ZzvrZy2DrIug2DEb9HdJagN2BNMLQ8Ayi5k6QDWC3gW8UJM9AIkmgP8uJEd/dk08QwE0nklgtHayp9vHk5gClVdDaAyVhKI9Ci18Za3z//R3o3TtATo7rF11VPVI5lAI5G9j5nd+LgN7fm9MWQAjxOWYYxt1Syne/v5EQYiwwFiA394eXfSyObR566CHee+89rrzySr788ktstl9+2no8Nt55ZwCbNjVQUHB42rW+9dZbrF69mgkTJhzQc7CwsLA4EJo18zJnzqC9HistjaBpEiEE27cHD3jv446DuXNhYyH4M+CMG6G6HvKz4Z1/7kncA/hsJxQX7cSmwL3rmlPbVFNXAre3lTyoN7JaakxQE+im2KkjyhsUomDgII4NAz9lODGrbISRpOAgmyzO5ubdx5HGNnSmE2+4FFuwEEXpBCkPgGgBn50BtWGorDArQdQCdheM/DvkdYcxT0LPfGhsBCEQhqSuUaArCmWGQQ1QqevEpCRSXMxHY8ey68orCRYVYcTje702qt1Om9NOY8f//geAwzAQQqACSULgBSKqQu7oS8m46nKYNByMIHRsBb3OgW1fgicJVr0Mgy6H+peR8lXQ/gfCg1STEYYK7gGQOAmAN/mQ1WxCpT0ZBCmjDQtoR3cCXEMaKoJO28Cug88NhoThOZC7/znmP0lCgo1LL8359RsdIRzK/9I/5qL7ftS2DWgDDARygE+FEAVSytq9Fkk5E5gJ0KNHj6M/8tviF5GSksKMGTO46KKLmD59OrfeeusB7eP32+nePfkgW2diGJJXX91BQ4PGxRe3wO3e+0+rtraWsWPHkpqayi233PITu1hYWFj8NvTvn8all7Zg7dp6Jk7sBEA0anDbbdvYuDHMffe1oFu3fVcFqasHhxcefgOKK6CsAVplw6adENfM5h/f0rsZVD93GbqEQbMX8m4QMz5XwGIZZ44RAQz+YpRwu+JlHTtYRDFxKvETw0OMJPZculcRBHDRjd5UcT9B/oNLqyQpWIdqeHAVaYgqHeQqsN8GsdaQ1AZKF+1RIwZQDJQ2JSW+/RoY3yYfSuqiUKOBhk6VomBoGo5AgHBtLToQj0RY98IL0BRG8e22iqoy8M47yWnfnuAXX2DU1qJKiVNKXIpCICMDWVlB29YKnk+egF2fQLQREkthZxmEdkJ6DiSugMwofNMdafOCvQE9XaAajZB0GXjuBnVPyMtGtmPDhobGqVzMFQjiSD5FYy1xugoHEwMwbjY4DJg2Es4p+KVnz++DQxm0VYRZrvpbcjBPw+/P+a+UMi6l3ApswBTMFhZ7ceGFFzJs2DBeeOEFNO3Iq3n6xhs7mTBhOZMnr2LatG9+MH7LLbdQXl7OM888g8NhXRK2sLA4vNhsCpMnd+aVV06gS5ckABYsqGXevGrWrw/z17/u2Oceu0ph4Ag483JYvx48bnCq4HLBnVfsEccba2BxMeT44dEH7iLv2rtYIuCsHIOaVJ1prjjbIgIVA6mWUqMW8QBb2EwYiURgJt2pxIii04p2ZBKmgCICfEgx91LGq0hZgydcgzCiCFmLdEZMF6kOlK2A4vfB64Chz0IgH3QVqoHaOMyZArs2QvsCZFoGhtdDHU6K43biUtIoJREpaVAUUFU0RUEDtHiceEUFLil3BzS4gSy3m11PP4386itaahrJTiceIfDb7SR7vfj69iCvbxJeexgRboT1y6F5GJyaGQ8dD8PQydDeBgkaSB1JI9IAISUxu42V7m6sVteis+d/4kB6oqORSxbZpNMNB3EkXgTZmPX0dm4AVyP4VHh56UE8qY4xDqUH+WugjRAiD9gFjAS+X6HiDeBiYLYQIhUz5GLLIbTJ4ihm5syZuN3uIyI8YenSaq6/fhnp6U6eeaYXwaCGlBIpoaFh78ts8+fP5+mnn+bWW2+le/fuh8liCwuLw0l1dZitW2vp0iUdu1093Ob8KLm5Tmw2gaZJ2rff9zX3Vd9AfQO4naDawO2AKdfBuBHm+Nw18MiXsDkIXi9c1w3oehqNSRCOw6txg1BWlBAwsUHlL2mCZ0QMHWhAoxnpnEQa69hMPRXYECSiMpBz2MBadGKAgU49YamRZjRiuCCmK7hCOoq3F9hWQF0YggbIIEQrof0F0PxkePQiWPchIKG6FEIhZLNcGqoiRCtiRCIa0u2hOq4hbTbTOSMEjZWVZmdqIAo0peSRoKq4k5OxV1YiGhuRjY3UvvQSvsxMfIaBPTGByOatNDurPxmNHwL1TUl2gNuA9BhEFAipcMq1SPvjEGgE3UA2qqD6aGyZguEWrFPPZr2yCShEQaETJwLQk870oADRdBH/7ySzkhgtsZGKytKN8PgcqK4FvRn8YcTBOnuOPQ6Z0pBSakKI64H3MOOLn5ZSrhVC/A1YIqWc1zQ2SAixDvM73gQpZdWhssni6CY52QyPCAaDLF26lP79+x82Wx56aCPl5RGKi8O8804Jw4e3YNeuMHV1MSZM6Lh7nqZpXHPNNbRr145JkyYdNnstLCwOHzU1YQYNeoHa2ggDB7Zg1qwjszlQQYGX117rQFFRlJNP3neuxgk9oF0r2LQNpt0BQ8/YMxaKwW3zIaxBZQgcLlhWDueqW1DLQM1qRYrP4Ntqy6ow6KQ4caMSRCcTOy0JU8gOQpTgIoE8fHSkLVlkEmEQ23kblRIkIZzo2FCBTAylDGIBhLsdnPA+bH4Olt1l1o5rcb55QG8ArpoNSzpBNAR1wA1DMeJO4uVVxCMaimojMTmZSCCAHgyS3aYNpStWoFVVoWsaEjPJLoZZjjhL18mMRDCkpBrTk6zv2oWS4CXBEadtcgzZTiLqPgJnEJIw1VEM6JUH3rgZtJ1bgBx0G3JnCtjiYINQbhpez9d4bRoGpdioRvIJAMb3olfFdyJcHQh6sqe7yuqtoOmQnQgn5MEZnfb79PjdcUhdcVLKt4G3v/fYxO/cl8DNTTcLi/1i/PjxvPDCC6xZs4a8vLzDYkO/fiksXlyF263QqVMiTqfKbbf98JPGZrPxwgsvoCgKbvdByIKwsLA46tixo57a2ihOp41Fi3YdbnP2oqFBIxw2SE834yE6dfLQqdP+lTPw++DtZ8Ew9k7GkxJWloHbDroEnxPyEmFCD7jxoivJNOA/7y7E6bBxXo1BLTrJiZX8iQgaUVzEkVTxISGCRPAhSMZGc1qgU8163mE9TwA6idhIJEYcA4322JQybPG+KM7jQS+AJW2gPgR2FWx+aH0FNJRB1SYorTBjImx2cMWgsRYlEsOVlogoNVv3RTt0ILWmBucJJ5AxdSpKQgIfnXEGRfPnYwCKouCTklQpSRMCJRJBsdkINAno1JxMXFojqekRUEBIwDDvowJZwOk2aJYHqRdBsAa6XQWKRAskotQ3Ytjhq4RulCmP0olT6MJguhIhAiTgoAN99vv9Prs3vPoZVNbBLcP2e9nvEvFzXXWORHr06CGXLFlyuM2wOIzs2LGDgoICevXqxfz58xHi4JRs+zFmzFjH889v4rLL2nDttXs8w1JKVq+uIynJTm7uj7eCDQaDeL2/XZtYiyMbIcRSKeWB1dI6ArE+i/cfTTO46ab3+fTTHdx6az8uueTIyIoqLAxxwQWrCIV07rsvnxEjMve9aD94fT1MmA+aAUPbwbkF0CsTvDb4+OOPARgwYMDu+f+mmieopo44CiHSqMBLkABRvNjIRKETAWpYhEEcJ9UkshUBpFGKkxgKBj68JMmBpIup5sYr+kLtV6aCN1SI5ELBw/DcFRCqhaAddjW18QsCZSoytxXhxjS0xYuRUlKGEyQY8Tiuzp1pvnAh4epqPh40iHhxMV2aNyflgnPYOfvfRKIGRjCIMyWR1FaJ+LRK1EYntuPb41j7MUJt6n6SrEIzwxTnXQyzKK5DIG0D0QqeRyUFBSe6toB6/R9Uqel8aUvEjo84YUYwlYlsZyUF8vsAACAASURBVCkNHIePKeTt7ohnsW/297PYqqxucdSRm5vLAw88wIIFC3jqqacO2XFqa6NMn76a+vo406atprY2untMCEGXLkk/KY7D4TDdu3fnnnvuOWT2WVhYHB3YbAozZpzBqlVjjxhxDLB4cR319RqKAq+9VvGr9lpVBIs3m97j9RUQ1838uIVh+OMyOOMjCGqmMP6uOAY4AS9+FBJQSSKOiiSJAHE8nEkn7mAoZ9MLpakNiEEaLpJRcOChNSp+QEFBEhevUUdvIvwTHAngNzB7OOuQ2BY+nQzBapAGhKN76m15gWZJiF6noOp1CGFgVyTOeAQRjWCTOsnbVhN/5y0S8vI4/amnOCEri/RYFb7nH6GTq46ubRUKbriQgq4q2WzBl6rgaVWHI7AcUeCBvAD0bgln50JPG/SWkIEZn4Eg5ljOVi5hG1dSyWbKba143XkCH9paAC40omTQmiCSpTTgR2U5DdSj/6r3zuLHOfzZThYWB8DYsWN56aWXuOWWWzjzzDPJzj74bWa9Xjs5OV6Ki4Pk5HhJSNj/zkB33303GzZsoF+/fgfdLgsLC4uDwcCBATIyHFRXx7nqqmYHvM+H38DVz5vi+LYzYXQ3WFoKugHLBCTazGYUO4MgSjcA0K5du93rW+PkTfJ4j0oepwENB0F0TqcN3WlOFB0fPgYxkq18Qwe6o1HPKp6glB14CJBFPoJPcFJFnBokj+NwpaJEHaDGINAVMm6BVReyux7bXgWFBLTJBY8fh1aJLRcUA5pVQjRutsu2+3XkP8bD8V1Q8/MRbjeu4DYEOiIOdmlgL98MNtEUThEyhXl20HSnJzvNhh9fTsJIykKoVQgXmIs91AWSUfCwgTAVPI6BShw7Ck7ctOR4eRYrZDKlQtJb+vlPoRtHQwLb26gk+Q/47bP4CSyBbHFUoigKs2bN4rrrriMWix2SY9jtCv/97+msWFFFt24p+93K9uuvv2batGmMGTOGU0899ZDYZmFhYfFryclxsWhRTzRN4nAc+AXljWWmiFQEfL4Z3qowK1s8fhrM2QmPbIBTMqCND04972oAFi5cuNceDgSVxDAQKCRxGikkE+RvfIYLGxM5kVzakEsbNKK8wj+IUoKBCy9hXDhR8OOmDgcaClmIhNMhWgLCBS3mwicXgD1oem2DQIeewEnwwSyIRiFcDuVLEDKC4gEk2Bx2bGUG0m2AXSLsEXjsRtTJcwg8+mfEPbdDUTXoMfC54KJr4evpkFYOiXFoTIDUOkgNYLhSCBe8QqyzjhR2lGhL/Lv6oGTeAPYEFPsCDJ6njmxUnICGlwQaMUjkJK4LJ/JZg4LXFmG6kYvcpRAFbl0veLfXAb99Fj+BJZAtjlry8/N5990fNF48qAQCTk4+ef89K7FYjCuvvJKsrCymTZt2CC2zsLA4FqiqCjFq1JuUljby2GNn0KvXwb8a9nMoisDh+HXxqxd2h4UboSEMagCWF5ve5BfWwU09YGxr+KAS1jTAlClTqNfgmSpo54R+3+lFcj7pbCeCjmQkzXiQz1FRKKORW3ifM2nNSAoQqEgM4jgQGARxU0UxCmko6ATIoSUvINICkDgM1FRQEgANvC4gCG4VMprDoAeg0wB45iYz7KL9cVBUjdi0GjAg3QatFChxghKFvAhEV8H9fVE9QDc7nNgZMmshOx9O7AgNDeYTkhKyIhi5fnTDQX371gTFx7hFCIENXLno+aNQ6AKAh2zm0YIgRSSxmURyeZ5TWY3Ei5P1DTbicZWIprLBYWAXKlEN4uvhlRhc0G/vZEmLX4f1Uloc9ZSWljJ69GjKysoOtyksX76cLVu28MQTT5CYeHhaWltYfBchxNNCiHIhxJqfGG8vhFgkhIgKIf78W9v3e+e997awZk0FtbURHnroq8Ntzn6zbics32JqwFQfzBkL/7sJTmwFNgUcKrQNmHPvXA83rIKLloCnYz9mZfdjUjGM3g7rm4oIG1LyeVzSI96cyTKfFBycT1t0DCSSROy8xWom8y47qWcgV+MgAQU3Duy4SMVAECOFGpxEqAYhwNkWbMmgOKDns9B+FGT1hxbnQNuR8HpbKL4DzrseBv0RThsG10yCVCckKpAahpQIoqAeMcCNcElwSAgVgTcGARW6FUPKNogsgKV/gK4TQNjB5kYPuCnp4KWki4M67yZ0oRBpKrumkIFKAduo4E2W8T6rWEsZ23EgOQMbl7K8wUdRaTNKqtzo6x0Ym234NMFQv8rLx8Mpu2DTAvjzLHjx48NzLhyrWB5ki6Oe6upqXnzxRUKhEC+//PJhtaV3795s27aNtLS0w2qHhcV3mA38C3j2J8argRuB838rgyz20LlzOi6XDU0zGDAg97DYsHGjxuzZYfr0sXPuua59zp+/AkZMh8YojDwRnr1xz9ioAlMYu2xwfFNRjMKg+TNuwKVvrmGTDRI6FOAQUN+UX/ZsPMbUaBiAGqebyxxO+pBNdzKZwqdspwoFg0qCvMEqxjOQYdxPI5XEKGIbb+DEwE4tKh4cpKJTTy2zUHCTyOWI5O6I5J7QHdNbPP80kEUgY6BNApkCS6ZDxnAYdR0sfQFCxdDSgJACHjsIL8hG6JAInjrwXg/iLYiXgxDoNjuR9gOpzZ+ON5zKDs/LaGohycIBog5kgDpcfM612EljF4tZTREObLixoaAgEGSRRLLmpqTGhYakvMFLIKSAFFwTU+jqFOCE3KaeM1JCffAgnRAWgCWQLY4BOnbsyKRJk7jzzjt5/fXXGTp06G9ug6ZpvP322wwZMsQSxxZHFFLKT4QQLX9mvBwoF0Kc/ZsZZbGbzp3TWbDgD9TWRunYMfWw2DBmTD07dujMnRulfXsbbdua0uB/H5i3UcOh9/F75r/0BdSEzZjjN74044+/2A7/WQbDOsOZHSCiwcpyaBOAe9vDX9ebZd5e/cv1KAJ4YiG3ZEPPppLLldLYXYuhQhq7j2VH5Q5OYgXFPM/XSCQtMJtGeQngJQC0oTknU8x6alhCS07GThJVTKOeuSiECPNPbOSRzNMoaFD2d4RzOagxhA2zy54/aFaUiM2EHtci2/4LSm5HGNvB4YeaPMj0EO24jlhOI/aKAK52kyE4BrY/Q6V3Axtb1BFR/ojmtIFT4MAHJOIgTi53o4hEVhFmGzuIUkM1CYSxE0GjFgjJXnSqSuXO0jRsArJ9kghgU83EPxXBKUl73oubzoNIDFwOGHXaITk9frdYAtnimGDChAnMnTuXcePGMWDAgN1d934pkYjGc8+txu22M3Jkx/1OzPvHP/7BrbfeysKFC39QwsjC4lhBCDEWGAtmuUWLg0N2tp9DUIhnv7HZzFLBAGqTR7KsAsZPMh9fuAhWf7hn7MtCM3rBADrlms1ArnnV/PnxFlicC6PegfVV0CoJ/n4ydDYgywkfXv4gugOuTYZx3/ElXOVwUm5IBHClw/ld87Cj0pPmePEwnyqakb7XeANB5vEGO1mHH4NtBDmRCwAHtagYCNJQUSilkVsR8gs8wa0oGQIljtnJ7tvGHcIscEHlTCJ5T6PqOrYGL4rig8H/RPoLiOidQFOJBpw4lGoUXz4U3MtaRlCNCwc6BgoCgziN2PCSzp34MasapbAIwU5s2JC4qCQFN1FqSGJTSTbzSxOIxATJKpzjgcFpcKITtvgFCTY47jsCOeCDv195MM4Ci+9jCWSLYwK73c4zzzxDz549mThxIv/6178OaJ9//vNrZsxYsrv5yKWX7rtm6YYNG5g4cSJDhw49rO2vLSwONVLKmcBMMBuFHGZzLA4STz+dyJw5EXr2tJGfb8oCu828NQYhkGgKYoDpr8OmHYBhNqA7vy9c/hQ0RMCmQqILYgasrQC/EzZVwyXvmjWQy8KQmtqTVBfc8b0mqAGh8ID75zv4zaaCtTSwkAam0o6V7GQLNQRZh2QHIFAIs401VLKLrrSgBB8O7ECUHOzAWnQJO3PTMRA4WkJicRKJlQK0QtCjIASGU9LosUEHFXexht13D/V+PwEEipqHoRYjSERg1lerpJIKBAKdOA5UNMJ4qCEVQTL96bb7efSjN6mk4MCBAz/PUsRKooTxo8dUpCbQY1BTDn2zBCOaEhmzD88Fht8tlkC2OGbo1q0bL774IgMHDjzgPSKROGZzSUk4HN/nfMMwGDNmDG63mxkzZhzSrn4WFhYWh4KWLVVuu23vpkfJAXhhBnz2FZx1qlkdYdqrcPtzpodVAGl+eH4xhKQZmTCyL4zuDVk+GNMVnlsLF3eEN3eaMbJSgrZ9BXUCDNntx0zZi80x2BaDk7zgEBBGR0EgkWykhvlsRccggpt8FEI4SCKEips4cZbyFZI0XERIogUermIlf8MpNpBoM7vvxWxualol4c37L1tD91ElV5MYrSPsihF3SVqwg3BeOvOUJTSwiJa04nTmoPElNrohMEX9Yr6kiPYE2ECERKJkEyZMHCinJQ8aFfyZHDyKioJCe9oCUBODRUuS2R6C27votMySnL9ZwRYFXz3k7PvfkMUhwhLIFscUF154IQC6rhOLxXC73b9o/fjxvQFwuexcdlnnfc5/7LHH+Oyzz3jmmWfIysr65QZbWFhYHCbicfjmG2jZEvw/0miiW4F5+5YXPgK7anbJS/TC2NNhUy18scVMyvtjH2jdFP1wVScY0wkyEqHjKhg/H5I0qH5mPIqAaf0XcudJP23blhicswNiEs5KgEez4C+0Yi6ltMVDV9y8hcBAkE2ACNk0orKLJCQRbEjyqMOBShgvGVxAEZ9Tj42IyMeJjpM6JAZ2AtSKLWz3biEO1Ce40WVLwii0lCcQFmdTxvsArGcLgwjg4Ky97G1GM1bi50OG0UA67WjgDjpwA2VsC2axtjGZqUT4b5KL05zq7nUfVcDaerO3yIuFKvP6wbQsmLQIsr3Q++B0/7Y4ACyBbHHMEY/HGTBgAF27duXxxx//RWv9ficTJ+5/mESLFi0YPXo0o0aN+qVmWlj8JgghXgQGAqlCiCJgEk3NbaWUTwghMoElgB8whBDjgY5SyvrDZLLFb8TYsfDpp5CWBu+/Dz7fz8/Pz4S1WyHJB19Nh7xMqA/De2uhbcYecbxgHYx71gzLeOoKWLoN/DFo1ME75GGS3fBOIT8rkHfETXGsAKujoEnJp40uMmjJ4ASwC8EE+lBCI8eTyUssZhVFxAgCdjQkVaSQg0I+3cihH+WofMJXaLippgfNiOEgTCuuwkNzFPPPgjAJLBXtEPiIic6cwwnY+Zg4saakwD1XCpfJGItllDNEAZnCx1YaiWk29FgGzdyt6CAkH4bMkp9xYGY4vpdA7pxolmSOGnBKU0z2ZR1hWBtwqqBaxXgPG5ZAtjjmsNvt9OnTh4ceeogRI0b8qpCLfTFkyBCGDBlyyPa3sPi1SCkv3sd4KZDzG5ljcQTx2WfgdkNFBezcCR07/vRcw4BlGyE3DXSdplA08Lvhoh57z13wDcSa5ny0HoYWwNvfQLIKGd26sasBbthH57cTPHCeD1ZG4J50eLoBptSYY/USxvkhnwD5mMWWz6Yr9USI4GAXRYCgnGyKOI5EOiAQCDrQQCKCKAoOwkSALDLoiYc0OvMwZcynkQAOSlBQ2UUZCSRyITdQxGbyKUA0CeRKqXOtrCGMwWsyzN1kkKDBqsIcqgwbN/thevM8alxhZodMsX+xc2/Z1SYB5h0PWyrh1Pw9j3vsP//6WBx6rO8mFsck9957L61atWLMmDGEQqGDvv+zzz7LlClT0DTtoO9tYWHx2xKP62zfXoeuG/uefAwxYQJoGgweDO3a/fS8jdthTSG0b26WD/Z74dFX4JppUFr1w/kX94ZEN6QkwEU9oX8r+OpG+PpGOC32NR12fk3+Psot2wX8IxMWtIR0A+aVQdgwaym/WA5TSs1kwG9Jx89NnM6tDOMOLmMgvYiRggc377IJHYMNlFBBO0I0A3pyLg8ymCl4SeMDqriSCu6nBy05g060wYOLMzDd3Jnk0oOTCWC6eQ0J6xogLiUqggiSvngZFWuGX7eTJlS+CIIdhSd9XpYnu9iY4maoe2+BXFoJF90A1/wZpn2nUnl5ucGbb8YpK/t9nZNHEkLKoysRuUePHnLJkiWH2wyLo4CFCxdy8sknc/PNNzN9+vSDtm9xcTEdO3akW7dufPjhhyhWb0+L/UAIsVRK2WPfM48OjpXPYl03uPDCV1m5spy+fbN5/vnzfhfJtsGgGQLh+fnCEXyyFK76m+kNvu0KaNUSVm2Cf7xsrr9oIEy77ofrDMMc/+5LWVgCnXsMBKDDHxay7EEoqYXJr0NUwNfl0DEDBnWEfrnmfYA+n8CumCQUgFwfVEZBQfD3bLj4Jyp6xtG5h4+pIEhbUvkTfSmnnn/xHlHiXMKJdGFPqcI/sYGthIlLSY9gLpnhFC5PBq/64/vfvBzmFYMjM8wZXaKMsnnoKhzEDLh2JywJwcRMuCDw86/v+4vg2vvBYYfUJPjkKYjFJP37B6mokKSlCT75xPur24Fb7GF/P4stgWxxTDNu3Dg++eQTli5disu17w5R+0JKyfnnn8/8+fNZtWoVrVu3PghWWvweONYEss/nk927d9/rseHDh3PttdcSCoU466yzfrBm9OjRjB49msrKyt0Jtd9l3LhxjBgxgp07d3LZZZf9YPyWW25hyJAhbNiwgauvvvoH43fddRennXYaK1asYPz48T8YnzJlCv369eOLL77gjjvuACAW01m+vBRVVfD7h7Jhw2S+/PJT7r333h+sf/LJJ2nXrh1vvvnmj37pfu6552jevDkvvfTSj+Y/vPLKK6SmpjJ79mxmz579g/G3334bj8fDY4899qNdQRcuXAjAtGnTeOutt/Yac7vdvPPOOwDcc889LFiwAIBgULJtm0ZaWgqrV/+XqioYP/523nhjMUJA+/Zm7HFOTg7PP/88AOPHj2fp0hWEI1DbCEVlYE9oy5U3zGTkafCHy8dSXLIRoZilx5qnm1WEHn74YQAuvfRSioqK9rKvb9++nHvZ/Zw+bg2RdX8iwRunW0v4aguEY0DLU8ka9FdqomC8fiY2I0y3ZmBXYGkt2HqdQ+qIP3NOa3j8woEAtHFCSpND9sfOPQNJHB0HNq4YPZo+I0dTXVnGbZcOR2Fvwdnyikv4ZmQP2FnByj/cC1IhwwZ5TSWZv3/uLak2q3kYEjr6Yerknz/3/jxhCqec0o8Vy/ece2CGq6zbAp7WDzP9zm4kKx8wefK9LFmiI4T5xaR7d5Wnnjr6zr1vSUlJ4dVXXwXg9ttvZ9GiRXuNf//cW7FixV7jbdu2ZebMmQCMHTuWjRs37jW+P+fe/fffD8CwYcN47bXX9uuz2IpBtjimefDBB7HZbAdFHAPMmTOHefPmMW3aNEscW1gcAzgcKoGAm+rqMKed1pKEBMfhNumgsnmzRjgsCYV07r47zIsv2ikuNtB107tbVfXD5Dxdh9UbIBo1Y5S9HnB6YfQQuPhGqKwCdGiVDWlJP3rYvaisgUXLoFCA319AXPWT4TNjM7Rv2+cZZvc9TQNVmsIzEoc1VWbVjDzggQIYkAbvOsyqDyn7UDAKAmnYqNDg43q4rxD0WhW/Lkj6jmdYAu/v9ONY1pnaXbuQhrK7EcpP0dwD20Pgt0PCPuwoKYdr7uL/27v38Kiqc4/j3zc3QpCrXOQSbooKRbCRWlEEjsRzIqVBUUyxnCNaofVo9dFyrNQqlFbr8QIFpVgRRKAVL4BgRRRBkKqAUKioFQVrJeoJSAgJJReSrPPHHnCIgQxhZnZm5vd5nnmc2XvNnndlZl5e96y1Nm07wcRxR+9LToZzesCUKZCVBa+95m3r2jWJgoJq2rVLIkWVmi90BlkSwoEDB3jjjTdqPasVqrKyMrp27UrXrl158803SU4+xm9vIrWItzPI8ZaLKyqqSEv7+jv9zjtfcNNNK2jXrglPPZVLq1YntmRkQzF2bCGrVpWTmmp07dqCf/wjmQMHAJJp0SKJBQu8wixY/pcwaKRXGBeXwPY10KgRHCyF74yAffugrAh+dTvcPPboYRQ1bd4GeT+FikOQ0Qb2F71FssEz0y7koj7w4l/hZ3+CM9t7Z5Lf/xRKD8FvxkC7FnDnK97Scr3awpLRRx/7jc/g3d2Qng6/3AgdT4F7zoNuzaFPazhYBRe9BUWVUJYBaRleMfzTNvA/QcunVTvo/RZ8fACsGi5rA+d2gFvbQqsQi9Pp8+G5V+CGq+Day4/ed9kY+Ec+HKqEKXfB8EtDO6ZERqi5WIMnJSFMnDiR3Nzcb/x0cyLS09NZtmwZTz75pIpjkTgTXBwDTJ26gb17S9m2bQ8rVuz0KaqTN21aCx56qAULF7bitttScQ46d4Z164xNm75ZHAN0PA2uHuadzb31eq84BshoDH98GJoC6Ukw7TF4e+PxX//wJazN4Kw2cGrRL2h74Bdc1Mfb/v0s+Ogh+PPPoGQ/NE2DNhkwIBP6dYJT0qCyGob3PPq4HxfCDS/BA+vhptWw9yBs+T+4biXkLoZ1+VBaBSVV3kVGUsuhcxqclQ55NcYtJxlc3xia7oE2+dC2AH7VIfTiuOArmDYf9u6HX/0eSsuO3n9Dnve3bN8GLqzl7y0Nk84gS0IoLCykV69edOjQgQ0bNpCaemJr6BQVFdGiRQi/JYocg84gx5bf/34TU6ZsJCUliWefvYI+fdr5HVJYVFQ4UlIgKan+k75G3QBvboBGabBoHvT51rHbOgfPL4dtH8HYPDhYsh2As2osm1FdDfNfgaffhkvOg//J9Yrq4jI4UAEdalzI5N3dMGKRN0TjKwdl5h2jURFU/gtOP9VbNeOlQnj2S7i+Eww7zltYWAo/eRn2lsIj/w692oT+9ygrh8HXekNJMtvDqjnelQeDlZdDauo3t0v0aZKeSA2LFy/myiuv5L777mPChAkhP2/fvn307t2bW2+9lTvuuCOCEUo8U4EcW5xzvPfeHlq0SCczs5bLzDUQ27b9i5df3kdOTkv69GlS9xPCoHAfPLcUzjoDBg8IzzHvnQFPPuedrV72OJzepe7n/PE92PAFjOwJS/8JpzaCe1+ARinQPBVeuB76dAhPfHXZUwhbP4Tv9IYWDffjIoSeizX0WxLGiBEjGDlyJJMmTeLyyy+nZ8+edT8Jb/ZyQUEB2dnZEY5QRBoKM+Occ9r6HcZxlZVVM2rUdoqLq3jqqd28805fMjLqP/zrq69g5Uro2/f4Fw1p1RJ+PKZ+r7F27VoABg0aRGUllJZ6kwT/8o53drWsDP6+I7QC+Ye9vRvAxZnef5uXw0NrYEA36Bk4Y7xmA9zya+jSAeY9CC2b1y/242nTCi69MPzHFf+oQJaE8sgjj1BRUUGjw4Pq6vDqq6/y5JNPMmHCBLJqG6wnIuKT6mpHZaUjJcWorHRUV3tDKLZsqeCMM1I49dSji+X8fMfzz1fSr18SXbokcfPNVSQlwaOPJtOxozF6NGzf7q1c8frr0C4Co0omTpwIwOLFa7j8csjPh7vugjt+DD+7D5o2gs8/gX9dAE1COCH+wUdw7e2Qkgzzp8F/D4AbLzp64uCUOd4wiPc/htfXw4j/CH+/JP6oQJaE0q5dO1544YWQ2paUlDB27FjOPvts7rnnnghHJiJyYjIykpkzpwfPPbeXq646lZ07DzF+/F4++aSali2TWbXqNJo3/3rQ65gxFXz0UTXp6cbQoSls2eIwg7lzq7nrrmS++AJSUqCiAvbvj0yBPGfOHAA2b4YvvvBWoJg7F9atg4dvhxvGwn2b4OPt8NBDdR9v/mLYs9cb6/zcn2HCzd9cVeOS/vDBDmicDr3PDH+fJD5puLgkpIKCAkaNGsXOnceenb5582b27dvH7Nmzw7aOsojIYZ98UsTatbs4dKiq7sbHcP75TamsTOa66z4nJ+cz1q4toaTkEEVF1eTnVx7VtrTUkZTkFZPdukFamjdx7FuBSXYzZ8K3vw3jx0OPHvDZZ4f4wx/2sWVLWS2vXD/du3ene/fuZGVB27bekIprrvH2FRd/vepF4b7QjjfoAq8PjdLgou/U3ubWa2HZY7B6PpzZ7eT7IIlBZ5AlIR06dIjly5dTUFDAqlWrar207ODBg9m1axfNm0dgwJqIJLSdO4sYNuwFDh2qIjf3dKZMGVyv42zbVsrLLxdTWprE3r2VNG+eQmVlNbm5GfTsefRqPdddV82sWWVcc00Gt96awoAB3hnkrCwv/110kXcDb5LiqFGfs2vXIZo0SWLt2i60bXvyJcNrr70GQHZ2NmvWwIED0Cqw7NrQofDhdm/YxZ0/D+14OYNh1dPe+OVO7WtvYwa9epx06JJgdAZZElKnTp148MEHef3115k1a9ZR+w4ePMizzz6Lc07FsYhExKefFlNRUYWZ8be/7an3cbp0SaNZs2QaNaqmW7cU+vdvzNtvZ3Lnnc3Yu/frM9OffVbJAw8UU1BQztNP7wfgvPPsSHFcm+LialJTvfHNZWXhWfHqN7/5zZHLeKelfV0cg3cm+Od3wCPToWPH0I/ZueOxi2OR+lKBLAlr7NixXHLJJYwfP55du3Yd2T5x4kTy8vLYsmWLj9GJSDy7+OKO5OR0pUOHJkyeXP/lD1q1SuGVV85g4cJubNt2BsuWZbJ7dyUDBuxgwIAdrFv3r6DWDudcrb+Y1WRmzJ7dnuzsJvz2t23p3PnE1o4/lvnz5zN//vywHEskkiI6xMLMcoBpQDLwhHPu/hr7xwAPAp8HNj3qnHsikjGJHGZmzJo1i3POOYcJEyawYMECNm7cyJQpUxg3bpxWrRCRiElLS2bGjCFhOVabNqm0afN1AbtyZQkVFd4Z39deK+Hii5vQuXMKM2e25C9/KWfUqIyQjnv++Y05//zwXmI7MzMzrMcTiZSIFchmlgzMAC4F8oF3zGyZc+6DGk2fcc7dHKk4RI6ne/fuLFq0iH79+lFeONqLKQAADWdJREFUXs71119P+/bteeCBB/wOTUTizJ49B5kyZTPt2mVw003nkpoamUvWX311C5YuLQZg5MivrwA6ZEg6/funsmjRbv75zzSys1uFdDY5nFasWAFATk5OVF9X5ERF8gzy+cAO59wnAGa2EBgO1CyQRXx1OFHffffdvP/++7z00ksaeywiYTd58nqWLt1JUpKRmdmUK6+MzJpjvXuns2WLNyut5iWlf/nLHSxatJvU1CTmzOnFwIEtIxLDsdx/v/dDsgpkaegiWSB3BHYFPc4HvltLuyvNbCDwEXCbc25XzQZmNg4YB9C5c+cIhCqJrrq6mj179nDjjTcydOhQv8MRkTjUpIk3DMIMGjeO7CJSNQvjwwoLvaXfqqocRUWVtbaJpIULF0b9NUXqI5Lf0Nq+nTWnwb4IPO2cKzeznwBPAZd840nOPQ48DtCvX7/wTKUVCZKUlMRjjz3mdxgiEsfuvvsCunVrRuvWjcnJ8WdB3l//+nTuvz+ZzMxGXHbZqVF//dNOOy3qrylSH5EskPOB4NH4nYAvghs45/YGPZwF/G8E4xERSThmNgcYBux2zvWuZb/hTaYeChwExjjn/hrdKI9WWFjKL36xhurqau69dzDbtn3F1q0F5OX1pGPHpn6GdlKaNEnlxz/u62sMmZnpzJhxtm+v/+KLLwLw/e9/37cYREIRyQL5HaCHmXXDW6XiB8A1wQ3MrL1z7svAw1zg7xGMR0QkEc0FHgXmHWP/ZUCPwO27wExqHw4XNbNnb2X58h0ApKen8vLLn1JeXsWrr37KihVX+xmanKSHH34YUIEsDV/ECmTnXKWZ3Qy8grfM2xzn3PtmNhnY5JxbBtxiZrlAJVAIjIlUPCIiicg594aZdT1Ok+HAPOecA9abWYsaJy+irlOnpqSkeMv0t27dGOe8MbXl5fW/JLM0DM8//7zfIYiEJKKzBJxzy4HlNbbdE3R/AjAhkjGIHMukSZM45ZRTKC4uZuDAgWRnZ/sdkogfaptQ3RH4RoEcrQnTeXnfonXrDKqrHZde2p2ePduwceOXjB3r7/AEOXmtW7f2OwSRkER2Gq1IDJg8ebLfIYj4KZQJ1d7GKE2YTkoyLr20+5HHI0eezciR/o2blfBZvHgxACNGjPA5EpHj06WmJaHce++9nHXWWWRnZ7N9+3YAxowZc+RnvzvvvJNevXrRp08fxo8fD0BBQQFXXHEFffv2pW/fvrz11lu+xS8SAXVOqBYJl+nTpzN9+nS/wxCpk84gS8LYvHkzCxcuZMuWLVRWVpKVlcV55513ZH9hYSFLlizhww8/xMwoKioC4JZbbmHQoEEsWbKEqqoqDhw44FcXRCJhGXBz4GJO3wX2+zn+WOLb0qVL/Q5BJCQqkCVhrFu3jiuuuIKMjAwAcnNzj9rfrFkz0tPTueGGG/je977HsGHDAFi9ejXz5nkLACQnJ+sqexJTzOxpYDDQ2szygYlAKoBz7jG8eSJDgR14y7xd50+kkgiUPyVWqECWhOIt+Vq7lJQUNm7cyKpVq1i4cCGPPvooq1evjmJ0IuHnnBtVx34H3BSlcCTBPfPMMwDk5eX5HInI8WkMsiSMgQMHsmTJEkpLSykpKTmyYP1hBw4cYP/+/QwdOpTf/e53bN26FYAhQ4Ywc+ZMAKqqqiguLo567CIi8WDmzJlH8qlIQ6YzyJIwsrKyyMvL49xzz6VLly5cfPHFR+0vKSlh+PDhlJWV4Zxj6tSpAEybNo1x48Yxe/ZskpOTmTlzJv379/ejCyIiMW358uV1NxJpAMz7dS129OvXz23atMnvMEREToiZbXbO9fM7jnBRLhaRWBRqLtYQCxEREYmKBQsWsGDBAr/DEKmThliIiIhIVDzxxBMAjB492udIRI5PBbKIiIhExcqVK/0OQSQkKpBFREQkKlJTU/0OQSQkGoMsIiIiUTF37lzmzp3rdxgidVKBLCIiIlGhAlliRcwt82Zme4B/RvhlWgNfRfg1oiVe+hIv/QD1pSGKRj+6OOfaRPg1osbMSoDtfsdxEmL9sxvL8cdy7KD4/Xay8YeUi2OuQI4GM9sUL+uVxktf4qUfoL40RPHSj2iK9b+Z4vdPLMcOit9v0YpfQyxERERERIKoQBYRERERCaICuXaP+x1AGMVLX+KlH6C+NETx0o9oivW/meL3TyzHDorfb1GJX2OQRURERESC6AyyiIiIiEgQFcgiIiIiIkESukA2sxwz225mO8zszlr2NzKzZwL7N5hZ1+hHGZoQ+nK7mX1gZu+a2Soz6+JHnHWpqx9B7a4yM2dmDXapmlD6YmZXB96X983sT9GOMRQhfLY6m9nrZrYl8Pka6kecdTGzOWa228zeO8Z+M7PpgX6+a2ZZ0Y6xoYn1HBnreTHW82Gs58BYzn2xnu9CiP+HgbjfNbO3zKxv2INwziXkDUgGdgLdgTTgb0CvGm3+G3gscP8HwDN+x30Sffk3ICNw/8aG2JdQ+hFo1xR4A1gP9PM77pN4T3oAW4CWgcdt/Y67nv14HLgxcL8X8KnfcR+jLwOBLOC9Y+wfCrwMGHABsMHvmGPgvW+wOTLW82Ks58NYz4GxnvtiPd+FEP+FQZ+byyIRfyKfQT4f2OGc+8Q5VwEsBIbXaDMceCpw/3lgiJlZFGMMVZ19cc697pw7GHi4HugU5RhDEcp7AvBr4AGgLJrBnaBQ+jIWmOGc2wfgnNsd5RhDEUo/HNAscL858EUU4wuZc+4NoPA4TYYD85xnPdDCzNpHJ7oGKdZzZKznxVjPh7GeA2M698V6vqsrfufcW4c/N0Tou5vIBXJHYFfQ4/zAtlrbOOcqgf3AqVGJ7sSE0pdgP8L7P8eGps5+mNm3gUzn3J+jGVg9hPKenAmcaWZvmtl6M8uJWnShC6Ufk4DRZpYPLAd+Gp3Qwu5Ev0fxLtZzZKznxVjPh7GeA+M998VTvovIdzcl3AeMIbWd5ai55l0obRqCkOM0s9FAP2BQRCOqn+P2w8ySgKnAmGgFdBJCeU9S8H5iHIz3f7/rzKy3c64owrGdiFD6MQqY65x72Mz6A/MD/aiOfHhhFSvf92iJ9RwZ63kx1vNhrOfAeM99Dfm7GzIz+ze8AnlAuI+dyGeQ84HMoMed+ObPI0famFkK3k8ox/vJwi+h9AUzywbuAnKdc+VRiu1E1NWPpkBvYI2ZfYo3bmpZQ5uYEhDq52upc+6Qc+4fwHa8fywaklD68SPgWQDn3NtAOtA6KtGFV0jfowQS6zky1vNirOfDWM+B8Z77Yj7fmVkf4AlguHNub7iPn8gF8jtADzPrZmZpeBNMltVoswy4NnD/KmC1C4wIb2Dq7Evgp7g/4P0j0JDGeQU7bj+cc/udc62dc12dc13xxh3lOuc2+RPucYXy+XoBb5IQZtYa7+fGT6IaZd1C6cdnwBAAM+uJ94/EnqhGGR7LgP8KzO6+ANjvnPvS76B8FOs5MtbzYqznw1jPgfGe+2I635lZZ2Ax8J/OuY8i8iLhnvUXSze8WZwf4c1UvSuwbTJekgHvw/4csAPYCHT3O+aT6MtrQAGwNXBb5nfM9elHjbZraECztuvxnhgwBfgA2Ab8wO+Y69mPXsCbeLO8twL/7nfMx+jH08CXwCG8syc/An4C/CTo/ZgR6Oe2hvzZakDvfYPOkbGeF2M9H8Z6Dozl3Bfr+S6E+J8A9gV9dzeFOwZdalpEREREJEgiD7EQEREREfkGFcgiIiIiIkFUIIuIiIiIBFGBLCIiIiISRAWyiIiIiEgQFcgSt8zMmdnDQY/Hm9mkwP1JZva5mW01s/fMLLeW7R+Y2aig5z9oZh+a2btmtsTMWkS9UyIiMc7MqoJy73NmllFj+9/M7K9mdmFge1czKw3sO3xL87cXEu9UIEs8KwdGBBagr81U59y5wEhgTuDSrcHbhwN/MLPUwPaVQG/nXB+8tTEnRDB2EZF4VeqcO9c51xuowFvfNnh7X7z8+tug5+wM7Dt8q4h20JJYVCBLPKsEHgduO14j59zfA21b19j+MXAQaBl4/KpzrjKwez3epTlFRKT+1gFn1LK9Gd6FIER8keJ3ACIRNgN418weOFYDM/suUE2NS4SaWRbwsav9ErTXA8+EM1ARkURiZinAZcCKwKbGZrYV7wqN7YFLgpqfHtgH8KZz7qboRSqJSAWyxDXnXLGZzQNuAUpr7L7NzEYDJUCec86Z2eHtY4HuQE7NY5rZXXhnnP8Y0eBFROJT46Bidx0wO3C/NDC8DTPrD8wzs96BfTsP7xOJBhXIkgh+B/wVeLLG9qnOuYdqaT/VOfeQmY3AS9CnO+fKAMzsWmAYMMTpOu0iIvVRWlex65x7OzB/pE2UYhI5isYgS9xzzhUCzwI/OsHnLQY2AdcCmFkO8HMg1zl3MNxxioiIx8zOBpKBvX7HIolJBbIkioepMQkvRJOB2wMrXDwKNAVWBpYZeiycAYqIJLjGh5dxw5vjca1zrsrvoCQxmX4lFhERERH5ms4gi4iIiIgEUYEsIiIiIhJEBbKIiIiISBAVyCIiIiIiQVQgi4iIiIgEUYEsIiIiIhJEBbKIiIiISJD/BwpyyZzl6aKCAAAAAElFTkSuQmCC
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing text_cell rendered"><div class="prompt input_prompt">
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="Fingerprinting-and-molecular-similarity"><a href="https://www.rdkit.org/docs/GettingStartedInPython.html#fingerprinting-and-molecular-similarity">Fingerprinting and molecular similarity</a><a class="anchor-link" href="#Fingerprinting-and-molecular-similarity">&#182;</a></h1><h2 id="click-here-for-a-more-detailed-explanation-of-the-theory-behind-fingerprints"><a href="https://www.daylight.com/dayhtml/doc/theory/theory.finger.html">click here for a more detailed explanation of the theory behind fingerprints</a><a class="anchor-link" href="#click-here-for-a-more-detailed-explanation-of-the-theory-behind-fingerprints">&#182;</a></h2><ul>
<li>in general, molecular substructures are converted into bitmaps that can be compared mathematically for similarity</li>
</ul>
<h2 id="Comparing-nearest-neighbor-similarity-between-two-libraries">Comparing nearest-neighbor similarity between two libraries<a class="anchor-link" href="#Comparing-nearest-neighbor-similarity-between-two-libraries">&#182;</a></h2><ul>
<li>example use case: would combining two different compound libraries lead to substantial redundancy? </li>
<li>in the example shown below, each compound fingerprint in one library is compared to each compound fingerprint in another and the highest similarity score is recorded</li>
<li>here, scoring ranges from 0.0 (no similarity) to 1.0 (structurally identical)</li>
<li>e.g. if a compound is associated with a score of 1.0, this means the same compound exists in both libraries</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">

<div class="output_area">




 
 
<div id="14506a4f-7d86-47f4-ac9d-848caef14824"></div>
<div class="output_subarea output_widget_view ">
<script type="text/javascript">
var element = $('#14506a4f-7d86-47f4-ac9d-848caef14824');
</script>
<script type="application/vnd.jupyter.widget-view+json">
{"model_id": "d186848af733423cac8fc1bc32a8247e", "version_major": 2, "version_minor": 0}
</script>
</div>

</div>

<div class="output_area">




 
 
<div id="fd33afb2-b34b-4a3e-86ed-c87770cf9601"></div>
<div class="output_subarea output_widget_view ">
<script type="text/javascript">
var element = $('#fd33afb2-b34b-4a3e-86ed-c87770cf9601');
</script>
<script type="application/vnd.jupyter.widget-view+json">
{"model_id": "edd477c9ce8a4516b3f128ce08aad2ce", "version_major": 2, "version_minor": 0}
</script>
</div>

</div>

<div class="output_area">



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
</div><div class="inner_cell">
<div class="text_cell_render border-box-sizing rendered_html">
<h1 id="2D-depictions-of-molecular-fingerprints:">2D depictions of molecular fingerprints:<a class="anchor-link" href="#2D-depictions-of-molecular-fingerprints:">&#182;</a></h1><ul>
<li>fingerprint bitmaps (here we used 2048 bits) can be decomposed using statistical techniques like <a href="https://en.wikipedia.org/wiki/Principal_component_analysis">Principle component analysis (PCA)</a> to allow for visualization and comparison of library diversity.</li>
<li>here we fit a <a href="https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.IncrementalPCA.html">pca model</a> on a set of ~348 million fragments (MW $\le$ 350 g/mol) downloaded from the <a href="http://zinc15.docking.org/tranches/home/#">ZINC database</a></li>
<li>the model (loaded here as 'ipca.pkl') is then used to project 2048 bit <a href="https://www.rdkit.org/docs/GettingStartedInPython.html#morgan-fingerprints-circular-fingerprints">Morgan Fingerprints</a> calculated from the compound libraries analyzed here onto two dimensions for visual comparison.</li>
</ul>

</div>
</div>
</div>
<div class="cell border-box-sizing code_cell rendered">

</div>
<div class="cell border-box-sizing code_cell rendered">

<div class="output_wrapper">
<div class="output">

<div class="output_area">



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

</div>
    </div>
  </div>
</body>

 


</html>
