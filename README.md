<html><head><meta http-equiv="Content-Type" content="text/html; charset=utf-8"/><title>1. Introducción a las redes</title><style>
/* cspell:disable-file */
/* webkit printing magic: print all background colors */
html {
	-webkit-print-color-adjust: exact;
}
* {
	box-sizing: border-box;
	-webkit-print-color-adjust: exact;
}

html,
body {
	margin: 0;
	padding: 0;
}
@media only screen {
	body {
		margin: 2em auto;
		max-width: 900px;
		color: rgb(55, 53, 47);
	}
}

body {
	line-height: 1.5;
	white-space: pre-wrap;
}

a,
a.visited {
	color: inherit;
	text-decoration: underline;
}

.pdf-relative-link-path {
	font-size: 80%;
	color: #444;
}

h1,
h2,
h3 {
	letter-spacing: -0.01em;
	line-height: 1.2;
	font-weight: 600;
	margin-bottom: 0;
}

.page-title {
	font-size: 2.5rem;
	font-weight: 700;
	margin-top: 0;
	margin-bottom: 0.75em;
}

h1 {
	font-size: 1.875rem;
	margin-top: 1.875rem;
}

h2 {
	font-size: 1.5rem;
	margin-top: 1.5rem;
}

h3 {
	font-size: 1.25rem;
	margin-top: 1.25rem;
}

.source {
	border: 1px solid #ddd;
	border-radius: 3px;
	padding: 1.5em;
	word-break: break-all;
}

.callout {
	border-radius: 3px;
	padding: 1rem;
}

figure {
	margin: 1.25em 0;
	page-break-inside: avoid;
}

figcaption {
	opacity: 0.5;
	font-size: 85%;
	margin-top: 0.5em;
}

mark {
	background-color: transparent;
}

.indented {
	padding-left: 1.5em;
}

hr {
	background: transparent;
	display: block;
	width: 100%;
	height: 1px;
	visibility: visible;
	border: none;
	border-bottom: 1px solid rgba(55, 53, 47, 0.09);
}

img {
	max-width: 100%;
}

@media only print {
	img {
		max-height: 100vh;
		object-fit: contain;
	}
}

@page {
	margin: 1in;
}

.collection-content {
	font-size: 0.875rem;
}

.column-list {
	display: flex;
	justify-content: space-between;
}

.column {
	padding: 0 1em;
}

.column:first-child {
	padding-left: 0;
}

.column:last-child {
	padding-right: 0;
}

.table_of_contents-item {
	display: block;
	font-size: 0.875rem;
	line-height: 1.3;
	padding: 0.125rem;
}

.table_of_contents-indent-1 {
	margin-left: 1.5rem;
}

.table_of_contents-indent-2 {
	margin-left: 3rem;
}

.table_of_contents-indent-3 {
	margin-left: 4.5rem;
}

.table_of_contents-link {
	text-decoration: none;
	opacity: 0.7;
	border-bottom: 1px solid rgba(55, 53, 47, 0.18);
}

table,
th,
td {
	border: 1px solid rgba(55, 53, 47, 0.09);
	border-collapse: collapse;
}

table {
	border-left: none;
	border-right: none;
}

th,
td {
	font-weight: normal;
	padding: 0.25em 0.5em;
	line-height: 1.5;
	min-height: 1.5em;
	text-align: left;
}

th {
	color: rgba(55, 53, 47, 0.6);
}

ol,
ul {
	margin: 0;
	margin-block-start: 0.6em;
	margin-block-end: 0.6em;
}

li > ol:first-child,
li > ul:first-child {
	margin-block-start: 0.6em;
}

ul > li {
	list-style: disc;
}

ul.to-do-list {
	padding-inline-start: 0;
}

ul.to-do-list > li {
	list-style: none;
}

.to-do-children-checked {
	text-decoration: line-through;
	opacity: 0.375;
}

ul.toggle > li {
	list-style: none;
}

ul {
	padding-inline-start: 1.7em;
}

ul > li {
	padding-left: 0.1em;
}

ol {
	padding-inline-start: 1.6em;
}

ol > li {
	padding-left: 0.2em;
}

.mono ol {
	padding-inline-start: 2em;
}

.mono ol > li {
	text-indent: -0.4em;
}

.toggle {
	padding-inline-start: 0em;
	list-style-type: none;
}

/* Indent toggle children */
.toggle > li > details {
	padding-left: 1.7em;
}

.toggle > li > details > summary {
	margin-left: -1.1em;
}

.selected-value {
	display: inline-block;
	padding: 0 0.5em;
	background: rgba(206, 205, 202, 0.5);
	border-radius: 3px;
	margin-right: 0.5em;
	margin-top: 0.3em;
	margin-bottom: 0.3em;
	white-space: nowrap;
}

.collection-title {
	display: inline-block;
	margin-right: 1em;
}

.page-description {
    margin-bottom: 2em;
}

.simple-table {
	margin-top: 1em;
	font-size: 0.875rem;
	empty-cells: show;
}
.simple-table td {
	height: 29px;
	min-width: 120px;
}

.simple-table th {
	height: 29px;
	min-width: 120px;
}

.simple-table-header-color {
	background: rgb(247, 246, 243);
	color: black;
}
.simple-table-header {
	font-weight: 500;
}

time {
	opacity: 0.5;
}

.icon {
	display: inline-block;
	max-width: 1.2em;
	max-height: 1.2em;
	text-decoration: none;
	vertical-align: text-bottom;
	margin-right: 0.5em;
}

img.icon {
	border-radius: 3px;
}

.user-icon {
	width: 1.5em;
	height: 1.5em;
	border-radius: 100%;
	margin-right: 0.5rem;
}

.user-icon-inner {
	font-size: 0.8em;
}

.text-icon {
	border: 1px solid #000;
	text-align: center;
}

.page-cover-image {
	display: block;
	object-fit: cover;
	width: 100%;
	max-height: 30vh;
}

.page-header-icon {
	font-size: 3rem;
	margin-bottom: 1rem;
}

.page-header-icon-with-cover {
	margin-top: -0.72em;
	margin-left: 0.07em;
}

.page-header-icon img {
	border-radius: 3px;
}

.link-to-page {
	margin: 1em 0;
	padding: 0;
	border: none;
	font-weight: 500;
}

p > .user {
	opacity: 0.5;
}

td > .user,
td > time {
	white-space: nowrap;
}

input[type="checkbox"] {
	transform: scale(1.5);
	margin-right: 0.6em;
	vertical-align: middle;
}

p {
	margin-top: 0.5em;
	margin-bottom: 0.5em;
}

.image {
	border: none;
	margin: 1.5em 0;
	padding: 0;
	border-radius: 0;
	text-align: center;
}

.code,
code {
	background: rgba(135, 131, 120, 0.15);
	border-radius: 3px;
	padding: 0.2em 0.4em;
	border-radius: 3px;
	font-size: 85%;
	tab-size: 2;
}

code {
	color: #eb5757;
}

.code {
	padding: 1.5em 1em;
}

.code-wrap {
	white-space: pre-wrap;
	word-break: break-all;
}

.code > code {
	background: none;
	padding: 0;
	font-size: 100%;
	color: inherit;
}

blockquote {
	font-size: 1.25em;
	margin: 1em 0;
	padding-left: 1em;
	border-left: 3px solid rgb(55, 53, 47);
}

.bookmark {
	text-decoration: none;
	max-height: 8em;
	padding: 0;
	display: flex;
	width: 100%;
	align-items: stretch;
}

.bookmark-title {
	font-size: 0.85em;
	overflow: hidden;
	text-overflow: ellipsis;
	height: 1.75em;
	white-space: nowrap;
}

.bookmark-text {
	display: flex;
	flex-direction: column;
}

.bookmark-info {
	flex: 4 1 180px;
	padding: 12px 14px 14px;
	display: flex;
	flex-direction: column;
	justify-content: space-between;
}

.bookmark-image {
	width: 33%;
	flex: 1 1 180px;
	display: block;
	position: relative;
	object-fit: cover;
	border-radius: 1px;
}

.bookmark-description {
	color: rgba(55, 53, 47, 0.6);
	font-size: 0.75em;
	overflow: hidden;
	max-height: 4.5em;
	word-break: break-word;
}

.bookmark-href {
	font-size: 0.75em;
	margin-top: 0.25em;
}

.sans { font-family: ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI Variable Display", "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol"; }
.code { font-family: "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace; }
.serif { font-family: Lyon-Text, Georgia, ui-serif, serif; }
.mono { font-family: iawriter-mono, Nitti, Menlo, Courier, monospace; }
.pdf .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI Variable Display", "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK JP'; }
.pdf:lang(zh-CN) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI Variable Display", "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK SC'; }
.pdf:lang(zh-TW) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI Variable Display", "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK TC'; }
.pdf:lang(ko-KR) .sans { font-family: Inter, ui-sans-serif, -apple-system, BlinkMacSystemFont, "Segoe UI Variable Display", "Segoe UI", Helvetica, "Apple Color Emoji", Arial, sans-serif, "Segoe UI Emoji", "Segoe UI Symbol", 'Twemoji', 'Noto Color Emoji', 'Noto Sans CJK KR'; }
.pdf .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK JP'; }
.pdf:lang(zh-CN) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK SC'; }
.pdf:lang(zh-TW) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK TC'; }
.pdf:lang(ko-KR) .code { font-family: Source Code Pro, "SFMono-Regular", Menlo, Consolas, "PT Mono", "Liberation Mono", Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK KR'; }
.pdf .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK JP'; }
.pdf:lang(zh-CN) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK SC'; }
.pdf:lang(zh-TW) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK TC'; }
.pdf:lang(ko-KR) .serif { font-family: PT Serif, Lyon-Text, Georgia, ui-serif, serif, 'Twemoji', 'Noto Color Emoji', 'Noto Serif CJK KR'; }
.pdf .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK JP'; }
.pdf:lang(zh-CN) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK SC'; }
.pdf:lang(zh-TW) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK TC'; }
.pdf:lang(ko-KR) .mono { font-family: PT Mono, iawriter-mono, Nitti, Menlo, Courier, monospace, 'Twemoji', 'Noto Color Emoji', 'Noto Sans Mono CJK KR'; }
.highlight-default {
	color: rgba(55, 53, 47, 1);
}
.highlight-gray {
	color: rgba(120, 119, 116, 1);
	fill: rgba(120, 119, 116, 1);
}
.highlight-brown {
	color: rgba(159, 107, 83, 1);
	fill: rgba(159, 107, 83, 1);
}
.highlight-orange {
	color: rgba(217, 115, 13, 1);
	fill: rgba(217, 115, 13, 1);
}
.highlight-yellow {
	color: rgba(203, 145, 47, 1);
	fill: rgba(203, 145, 47, 1);
}
.highlight-teal {
	color: rgba(68, 131, 97, 1);
	fill: rgba(68, 131, 97, 1);
}
.highlight-blue {
	color: rgba(51, 126, 169, 1);
	fill: rgba(51, 126, 169, 1);
}
.highlight-purple {
	color: rgba(144, 101, 176, 1);
	fill: rgba(144, 101, 176, 1);
}
.highlight-pink {
	color: rgba(193, 76, 138, 1);
	fill: rgba(193, 76, 138, 1);
}
.highlight-red {
	color: rgba(212, 76, 71, 1);
	fill: rgba(212, 76, 71, 1);
}
.highlight-default_background {
	color: rgba(55, 53, 47, 1);
}
.highlight-gray_background {
	background: rgba(241, 241, 239, 1);
}
.highlight-brown_background {
	background: rgba(244, 238, 238, 1);
}
.highlight-orange_background {
	background: rgba(251, 236, 221, 1);
}
.highlight-yellow_background {
	background: rgba(251, 243, 219, 1);
}
.highlight-teal_background {
	background: rgba(237, 243, 236, 1);
}
.highlight-blue_background {
	background: rgba(231, 243, 248, 1);
}
.highlight-purple_background {
	background: rgba(244, 240, 247, 0.8);
}
.highlight-pink_background {
	background: rgba(249, 238, 243, 0.8);
}
.highlight-red_background {
	background: rgba(253, 235, 236, 1);
}
.block-color-default {
	color: inherit;
	fill: inherit;
}
.block-color-gray {
	color: rgba(120, 119, 116, 1);
	fill: rgba(120, 119, 116, 1);
}
.block-color-brown {
	color: rgba(159, 107, 83, 1);
	fill: rgba(159, 107, 83, 1);
}
.block-color-orange {
	color: rgba(217, 115, 13, 1);
	fill: rgba(217, 115, 13, 1);
}
.block-color-yellow {
	color: rgba(203, 145, 47, 1);
	fill: rgba(203, 145, 47, 1);
}
.block-color-teal {
	color: rgba(68, 131, 97, 1);
	fill: rgba(68, 131, 97, 1);
}
.block-color-blue {
	color: rgba(51, 126, 169, 1);
	fill: rgba(51, 126, 169, 1);
}
.block-color-purple {
	color: rgba(144, 101, 176, 1);
	fill: rgba(144, 101, 176, 1);
}
.block-color-pink {
	color: rgba(193, 76, 138, 1);
	fill: rgba(193, 76, 138, 1);
}
.block-color-red {
	color: rgba(212, 76, 71, 1);
	fill: rgba(212, 76, 71, 1);
}
.block-color-default_background {
	color: inherit;
	fill: inherit;
}
.block-color-gray_background {
	background: rgba(241, 241, 239, 1);
}
.block-color-brown_background {
	background: rgba(244, 238, 238, 1);
}
.block-color-orange_background {
	background: rgba(251, 236, 221, 1);
}
.block-color-yellow_background {
	background: rgba(251, 243, 219, 1);
}
.block-color-teal_background {
	background: rgba(237, 243, 236, 1);
}
.block-color-blue_background {
	background: rgba(231, 243, 248, 1);
}
.block-color-purple_background {
	background: rgba(244, 240, 247, 0.8);
}
.block-color-pink_background {
	background: rgba(249, 238, 243, 0.8);
}
.block-color-red_background {
	background: rgba(253, 235, 236, 1);
}
.select-value-color-uiBlue { background-color: rgba(35, 131, 226, .07); }
.select-value-color-pink { background-color: rgba(245, 224, 233, 1); }
.select-value-color-purple { background-color: rgba(232, 222, 238, 1); }
.select-value-color-green { background-color: rgba(219, 237, 219, 1); }
.select-value-color-gray { background-color: rgba(227, 226, 224, 1); }
.select-value-color-transparentGray { background-color: rgba(227, 226, 224, 0); }
.select-value-color-translucentGray { background-color: rgba(0, 0, 0, 0.06); }
.select-value-color-orange { background-color: rgba(250, 222, 201, 1); }
.select-value-color-brown { background-color: rgba(238, 224, 218, 1); }
.select-value-color-red { background-color: rgba(255, 226, 221, 1); }
.select-value-color-yellow { background-color: rgba(253, 236, 200, 1); }
.select-value-color-blue { background-color: rgba(211, 229, 239, 1); }
.select-value-color-pageGlass { background-color: undefined; }
.select-value-color-washGlass { background-color: undefined; }

.checkbox {
	display: inline-flex;
	vertical-align: text-bottom;
	width: 16;
	height: 16;
	background-size: 16px;
	margin-left: 2px;
	margin-right: 5px;
}

.checkbox-on {
	background-image: url("data:image/svg+xml;charset=UTF-8,%3Csvg%20width%3D%2216%22%20height%3D%2216%22%20viewBox%3D%220%200%2016%2016%22%20fill%3D%22none%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%0A%3Crect%20width%3D%2216%22%20height%3D%2216%22%20fill%3D%22%2358A9D7%22%2F%3E%0A%3Cpath%20d%3D%22M6.71429%2012.2852L14%204.9995L12.7143%203.71436L6.71429%209.71378L3.28571%206.2831L2%207.57092L6.71429%2012.2852Z%22%20fill%3D%22white%22%2F%3E%0A%3C%2Fsvg%3E");
}

.checkbox-off {
	background-image: url("data:image/svg+xml;charset=UTF-8,%3Csvg%20width%3D%2216%22%20height%3D%2216%22%20viewBox%3D%220%200%2016%2016%22%20fill%3D%22none%22%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%3E%0A%3Crect%20x%3D%220.75%22%20y%3D%220.75%22%20width%3D%2214.5%22%20height%3D%2214.5%22%20fill%3D%22white%22%20stroke%3D%22%2336352F%22%20stroke-width%3D%221.5%22%2F%3E%0A%3C%2Fsvg%3E");
}
	
</style></head><body><article id="294d5a45-19e5-45e2-bcf1-d7cdd6812482" class="page sans"><header><div class="page-header-icon undefined"><span class="icon">📝</span></div><h1 class="page-title">1. Introducción a las redes</h1><p class="page-description"></p>	<table class="properties"><tbody><tr class="property-row property-row-status"><th><span class="icon property-icon"><svg role="graphics-symbol" viewBox="0 0 16 16" style="width:14px;height:14px;display:block;fill:rgba(55, 53, 47, 0.45);flex-shrink:0" class="typesStatus"><path d="M8.75488 1.02344C8.75488 0.613281 8.41309 0.264648 8.00293 0.264648C7.59277 0.264648 7.25098 0.613281 7.25098 1.02344V3.11523C7.25098 3.51855 7.59277 3.86719 8.00293 3.86719C8.41309 3.86719 8.75488 3.51855 8.75488 3.11523V1.02344ZM3.91504 5.0293C4.20215 5.31641 4.69434 5.32324 4.97461 5.03613C5.26855 4.74902 5.26855 4.25684 4.98145 3.96973L3.53906 2.52051C3.25195 2.2334 2.7666 2.21973 2.47949 2.50684C2.19238 2.79395 2.18555 3.28613 2.47266 3.57324L3.91504 5.0293ZM10.9629 4.01758C10.6826 4.30469 10.6826 4.79688 10.9697 5.08398C11.2568 5.37109 11.749 5.36426 12.0361 5.07715L13.4854 3.62793C13.7725 3.34082 13.7725 2.84863 13.4785 2.55469C13.1982 2.27441 12.7061 2.27441 12.4189 2.56152L10.9629 4.01758ZM15.0234 8.78906C15.4336 8.78906 15.7822 8.44727 15.7822 8.03711C15.7822 7.62695 15.4336 7.28516 15.0234 7.28516H12.9385C12.5283 7.28516 12.1797 7.62695 12.1797 8.03711C12.1797 8.44727 12.5283 8.78906 12.9385 8.78906H15.0234ZM0.975586 7.28516C0.56543 7.28516 0.223633 7.62695 0.223633 8.03711C0.223633 8.44727 0.56543 8.78906 0.975586 8.7.626H3.07422C3.48438 8.78906 3.83301 8.44727 3.83301 8.03711C3.83301 7.62695 3.48438 7.28516 3.07422 7.28516H0.975586ZM12.0361 10.9902C11.749 10.71 11.2568 10.71 10.9629 10.9971C10.6826 11.2842 10.6826 11.7764 10.9697 12.0635L12.4258 13.5127C12.7129 13.7998 13.2051 13.793 13.4922 13.5059C13.7793 13.2256 13.7725 12.7266 13.4854 12.4395L12.0361 10.9902ZM2.52051 12.4395C2.22656 12.7266 2.22656 13.2188 2.50684 13.5059C2.79395 13.793 3.28613 13.7998 3.57324 13.5127L5.02246 12.0703C5.31641 11.7832 5.31641 11.291 5.03613 11.0039C4.74902 10.7168 4.25684 10.71 3.96973 10.9971L2.52051 12.4395ZM8.75488 12.9658C8.75488 12.5557 8.41309 12.207 8.00293 12.207C7.59277 12.207 7.25098 12.5557 7.25098 12.9658V15.0576C7.25098 15.4609 7.59277 15.8096 8.00293 15.8096C8.41309 15.8096 8.75488 15.4609 8.75488 15.0576V12.9658Z"></path></svg></span>Estado</th><td><span class="status-value select-value-color-green"><div class="status-dot status-dot-color-green"></div>Listo</span></td></tr><tr class="property-row property-row-select"><th><span class="icon property-icon"><svg role="graphics-symbol" viewBox="0 0 16 16" style="width:14px;height:14px;display:block;fill:rgba(55, 53, 47, 0.45);flex-shrink:0" class="typesSelect"><path d="M8 15.126C11.8623 15.126 15.0615 11.9336 15.0615 8.06445C15.0615 4.20215 11.8623 1.00293 7.99316 1.00293C4.13086 1.00293 0.938477 4.20215 0.938477 8.06445C0.938477 11.9336 4.1377 15.126 8 15.126ZM8 13.7383C4.85547 13.7383 2.33301 11.209 2.33301 8.06445C2.33301 4.91992 4.84863 2.39746 7.99316 2.39746C11.1377 2.39746 13.6738 4.91992 13.6738 8.06445C13.6738 11.209 11.1445 13.7383 8 13.7383ZM7.62402 10.6348C7.79492 10.915 8.20508 10.9287 8.37598 10.6348L10.666 6.73145C10.8574 6.41016 10.7002 6.04102 10.3652 6.04102H5.62793C5.29297 6.04102 5.14941 6.43066 5.32031 6.73145L7.62402 10.6348Z"></path></svg></span>Dominio</th><td><span class="selected-value select-value-color-green">Alto</span></td></tr><tr class="property-row property-row-last_edited_time"><th><span class="icon property-icon"><svg role="graphics-symbol" viewBox="0 0 16 16" style="width:14px;height:14px;display:block;fill:rgba(55, 53, 47, 0.45);flex-shrink:0" class="typesCreatedAt"><path d="M8 15.126C11.8623 15.126 15.0615 11.9336 15.0615 8.06445C15.0615 4.20215 11.8623 1.00293 7.99316 1.00293C4.13086 1.00293 0.938477 4.20215 0.938477 8.06445C0.938477 11.9336 4.1377 15.126 8 15.126ZM8 13.7383C4.85547 13.7383 2.33301 11.209 2.33301 8.06445C2.33301 4.91992 4.84863 2.39746 7.99316 2.39746C11.1377 2.39746 13.6738 4.91992 13.6738 8.06445C13.6738 11.209 11.1445 13.7383 8 13.7383ZM4.54102 8.91211H7.99316C8.30078 8.91211 8.54004 8.67285 8.54004 8.37207V3.8877C8.54004 3.58691 8.30078 3.34766 7.99316 3.34766C7.69238 3.34766 7.45312 3.58691 7.45312 3.8877V7.83203H4.54102C4.2334 7.83203 4.00098 8.06445 4.00098 8.37207C4.00098 8.67285 4.2334 8.91211 4.54102 8.91211Z"></path></svg></span>Última edición</th><td><time>@25 de septiembre de 2024 17:44</time></td></tr></tbody></table></header><div class="page-body"><ul id="32f2a18e-e652-4f5f-b120-88c392c12a67" class="toggle"><li><details open=""><summary>Resumen del contenido</summary><ul id="9b31bc37-9e5c-458a-95bf-8e2e10d61a1c" class="bulleted-list"><li style="list-style-type:disc">Las redes LAN y WAN conectan usuarios dentro y fuera de la organización, permitiendo diversos tipos de comunicación</li></ul><ul id="4e66c5b9-4c9e-4591-b509-d47a339421ca" class="bulleted-list"><li style="list-style-type:disc">El modelo OSI divide la red en 7 capas para facilitar el desarrollo independiente de cada área</li></ul><ul id="a50b4785-589b-4dcc-a5d7-1ba57aa1c026" class="bulleted-list"><li style="list-style-type:disc">TCP/IP es un modelo de 4 capas creado por el Departamento de Defensa de EE.UU. para una red resistente</li></ul><ul id="4225ad63-202a-4336-b48e-1add6e7bbb99" class="bulleted-list"><li style="list-style-type:disc">Ethernet es la tecnología de acceso al medio más popular, escalable y económica</li></ul><ul id="c56e2dd4-b7d5-46f3-9acd-89f9eaa5fe95" class="bulleted-list"><li style="list-style-type:disc">El modelo jerárquico de Cisco consta de tres capas: acceso, distribución y núcleo</li></ul><ul id="ded9a0da-cc1b-46b1-8c6e-4800630ff6e9" class="bulleted-list"><li style="list-style-type:disc">El modelo de core colapsado combina las funciones de distribución y núcleo en un solo dispositivo para reducir costos</li></ul><ul id="98699bb5-0256-4c85-9202-c7af0e0d06de" class="bulleted-list"><li style="list-style-type:disc">Un procedimiento estructurado de troubleshooting ayuda a utilizar eficientemente los recursos y facilita la continuidad del trabajo</li></ul><ul id="0486811a-bc2f-47de-be84-b9260803a079" class="bulleted-list"><li style="list-style-type:disc">Es fundamental entender los modelos de red, protocolos principales y características de cada capa para el examen</li></ul></details></li></ul><nav id="a7536b15-1a6f-4f9a-8af7-ff4ed86c5891" class="block-color-gray table_of_contents"><div class="table_of_contents-item table_of_contents-indent-0"><a class="table_of_contents-link" href="#a5368344-2546-4888-9a1f-2fa55e03e591"><mark class="highlight-purple">1. Conceptos básicos</mark></a></div><div class="table_of_contents-item table_of_contents-indent-0"><a class="table_of_contents-link" href="#8d89d109-3afa-459f-b082-ab9c727d972d"><mark class="highlight-purple">2. Modelo de referencia OSI</mark></a></div><div class="table_of_contents-item table_of_contents-indent-1"><a class="table_of_contents-link" href="#137ac4de-c18d-46ff-96ef-8fb43ae4dfa6">2.1 Descripción de las siete capas</a></div><div class="table_of_contents-item table_of_contents-indent-2"><a class="table_of_contents-link" href="#6a241330-58ee-48c3-bb1c-5b9041a87c22"><mark class="highlight-blue"><strong>Capa aplicación</strong></mark></a></div><div class="table_of_contents-item table_of_contents-indent-2"><a class="table_of_contents-link" href="#d0b64d48-85dc-41ff-8598-86fca94f11c6"><mark class="highlight-blue"><strong>Capa presentación </strong></mark></a></div><div class="table_of_contents-item table_of_contents-indent-2"><a class="table_of_contents-link" href="#e8674043-0b10-4594-a3f5-6f7a3a4bc71e"><mark class="highlight-blue"><strong>Capa de sesión</strong></mark> </a></div><div class="table_of_contents-item table_of_contents-indent-2"><a class="table_of_contents-link" href="#835f6c57-d6b8-4c6e-a2fb-0a7cbce07f0c"><mark class="highlight-blue"><strong>Capa de transporte</strong></mark></a></div><div class="table_of_contents-item table_of_contents-indent-2"><a class="table_of_contents-link" href="#4396dcc8-bf4f-45a3-b64a-183dae2fc025"><mark class="highlight-blue"><strong>Capa de red</strong></mark></a></div><div class="table_of_contents-item table_of_contents-indent-2"><a class="table_of_contents-link" href="#9240ae04-dfd9-4884-a698-aef7e4865250"><mark class="highlight-blue"><strong>Capa de enlace de datos</strong></mark></a></div><div class="table_of_contents-item table_of_contents-indent-2"><a class="table_of_contents-link" href="#6ec303eb-cb46-4292-84d6-63e72a106b17"><mark class="highlight-blue"><strong>Capa física</strong></mark> </a></div><div class="table_of_contents-item table_of_contents-indent-0"><a class="table_of_contents-link" href="#8580d554-d30d-4894-9b5b-785889625e1b"><mark class="highlight-purple">3. Modelo TCP/IP</mark></a></div><div class="table_of_contents-item table_of_contents-indent-1"><a class="table_of_contents-link" href="#1fef00eb-628a-43e4-aa0e-5772f5680a5a">3.1 Protocolos de capa de aplicación</a></div><div class="table_of_contents-item table_of_contents-indent-1"><a class="table_of_contents-link" href="#4efd4522-6f05-409a-b200-4d1038f4a238">3.2 Protocolos de capa de transporte</a></div><div class="table_of_contents-item table_of_contents-indent-1"><a class="table_of_contents-link" href="#a5e47aa1-c2d6-4dcc-8885-bdf4e01f4963">3.3 Números de puertos</a></div><div class="table_of_contents-item table_of_contents-indent-1"><a class="table_of_contents-link" href="#e5f3908b-69a6-4438-9fa9-ae8e208b230f">3.4 Protocolos de capa de internet</a></div><div class="table_of_contents-item table_of_contents-indent-0"><a class="table_of_contents-link" href="#324a4402-c35a-4fb6-8efd-4a6d2eab4ef6"><mark class="highlight-purple">4. Ethernet</mark></a></div><div class="table_of_contents-item table_of_contents-indent-1"><a class="table_of_contents-link" href="#f7e7dadd-1fa2-4be6-a12b-95f131ffd4cf">4.1 Dominio de colisión</a></div><div class="table_of_contents-item table_of_contents-indent-1"><a class="table_of_contents-link" href="#6d706740-3250-4c3e-9914-73fe05dd1bf1">4.2 Dominio de difusión</a></div><div class="table_of_contents-item table_of_contents-indent-1"><a class="table_of_contents-link" href="#64025164-ca35-45b1-9f33-7768e2b4a90c">4.3 CSMA/CD</a></div><div class="table_of_contents-item table_of_contents-indent-1"><a class="table_of_contents-link" href="#049fef27-7d29-4d82-b5b2-9d7ef0a58ba6">4.4 Operación dúplex</a></div><div class="table_of_contents-item table_of_contents-indent-1"><a class="table_of_contents-link" href="#cb635444-a6b7-45fd-b57e-74c4bf1dd388">4.5 Formato básico de una trama Ethernet</a></div><div class="table_of_contents-item table_of_contents-indent-1"><a class="table_of_contents-link" href="#88c3470e-365c-4152-9aa8-60b16d2411b3">4.6 Proceso de encapsulación de los datos</a></div><div class="table_of_contents-item table_of_contents-indent-2"><a class="table_of_contents-link" href="#fff4020f-bd2c-803c-991c-f0ea2b488395">Secuencia de la encapsulación de datos:</a></div><div class="table_of_contents-item table_of_contents-indent-1"><a class="table_of_contents-link" href="#fff4020f-bd2c-807e-a7f5-f331afb01f7e"><mark class="highlight-purple">5. Modelo jerárquico</mark></a></div><div class="table_of_contents-item table_of_contents-indent-2"><a class="table_of_contents-link" href="#014ba287-ed2b-43de-8a7b-e768a484d967">5.1 Capa de acceso</a></div><div class="table_of_contents-item table_of_contents-indent-2"><a class="table_of_contents-link" href="#557c09df-42d2-45c0-90eb-ca5d323c8874">5.2 Capa de distribución</a></div><div class="table_of_contents-item table_of_contents-indent-2"><a class="table_of_contents-link" href="#c287537e-74c8-46c6-ab78-3b05a6c1fd84">5.3 Capa de núcleo</a></div><div class="table_of_contents-item table_of_contents-indent-0"><a class="table_of_contents-link" href="#ddcf5b78-1d2b-4035-9fd7-3a694c8a2b65"><mark class="highlight-purple">6. Modelo de core colapsado</mark></a></div><div class="table_of_contents-item table_of_contents-indent-0"><a class="table_of_contents-link" href="#7a2a7303-d729-43b3-96a7-1d281182ebb3"><mark class="highlight-purple">7. Procedimientos básicos de troubleshooting</mark></a></div><div class="table_of_contents-item table_of_contents-indent-0"><a class="table_of_contents-link" href="#1e2186a2-73b5-471e-beb1-8e9a54199526"><mark class="highlight-purple">8. Fundamentos para el examen</mark></a></div></nav><h1 id="a5368344-2546-4888-9a1f-2fa55e03e591" class=""><mark class="highlight-purple">1. Conceptos básicos</mark></h1><p id="78890861-69f6-40a1-a6a2-24a09527c85a" class="">Las redes LAN (Local Area Network) y las redes WAN (Wide Area<br/>Network), conectan a los usuarios dentro y fuera de la organización. Permiten<br/>gran cantidad y diversos tipos de comunicación.<br/></p><h1 id="8d89d109-3afa-459f-b082-ab9c727d972d" class=""><mark class="highlight-purple">2. Modelo de referencia OSI</mark></h1><p id="b4d225df-3e1a-4c36-8a67-71566e54bf44" class="">El modelo OSI (Open System Interconnection, no confundir con ISO) divide<br/>a la red en diferentes capas con el propósito de que cada desarrollador trabaje<br/>específicamente en su campo sin tener necesidad de depender de otras áreas.<br/></p><p id="2942b9bd-d138-4d6c-9cbd-40770652f70e" class="">7 Aplicación<br/>6 Presentación<br/>5 Sesión<br/>4 Transporte<br/>3 Red<br/>2 Enlace de datos<br/>1 Física<br/></p><p id="de9abdae-d631-465c-9a4f-b631a899a620" class="">Cada una de estas capas presta servicio a la capa inmediatamente superior,<br/>siendo la capa de aplicación la única que no lo hace ya que al ser la última<br/>capa su servicio está directamente relacionado con el usuario.<br/></p><h2 id="137ac4de-c18d-46ff-96ef-8fb43ae4dfa6" class="">2.1 Descripción de las siete capas</h2><h3 id="6a241330-58ee-48c3-bb1c-5b9041a87c22" class=""><mark class="highlight-blue"><strong>Capa aplicación</strong></mark></h3><p id="5d0fcb87-adf2-48eb-a495-4931c5b0fcec" class="">Es la única capa que no presta servicio a otra puesto que es la capa de nivel superior del modelo OSI directamente relacionada con el usuario.  Se accede a un procesador de textos por el servicio de transferencia de archivos de esta capa.</p><h3 id="d0b64d48-85dc-41ff-8598-86fca94f11c6" class=""><mark class="highlight-blue"><strong>Capa presentación </strong></mark></h3><p id="a333b66f-12d0-4a5c-8dac-2da6b2f39a4f" class="">Los datos formateados se proveen de diversas funciones de conversión y codificación que se aplican a los datos provenientes de la capa de aplicación.</p><p id="e3aa259c-04d7-421f-b0de-1faf408a31b3" class="">Un ejemplo de funciones de codificación sería el cifrado de datos una vez que éstos salen de una aplicación. Por ejemplo, los formatos de imágenes JPEG y GIF que se muestran en páginas web. Este formato asegura que todos los navegadores web puedan mostrar las imágenes, con independencia del sistema operativo utilizado.</p><h3 id="e8674043-0b10-4594-a3f5-6f7a3a4bc71e" class=""><mark class="highlight-blue"><strong>Capa de sesión</strong></mark> </h3><p id="7a7975a0-b1f6-4714-ada2-b7adfe87adf1" class="">Es la responsable de establecer, administrar y concluir las sesiones de comunicaciones entre entidades de la capa de presentación.</p><p id="0341b974-3c05-48a7-bb21-21914aa1310f" class="">Un ejemplo de este tipo de coordinación podría ser el que tiene lugar entre un servidor y un cliente de base de datos.</p><h3 id="835f6c57-d6b8-4c6e-a2fb-0a7cbce07f0c" class=""><mark class="highlight-blue"><strong>Capa de transporte</strong></mark></h3><p id="f442abe7-e695-4d15-b884-be5acb439720" class="">Es la encargada de la comunicación confiable entre host.  Los datos son divididos en segmentos identificados con un encabezado con un número de puerto que identifica la aplicación de origen. En esta capa funcionan protocolos como UDP y TCP</p><p id="381d5710-afc0-4f80-832c-45acdbb56854" class=""><mark class="highlight-yellow"><strong><span style="border-bottom:0.05em solid">Funciones de la capa de transporte</span></strong></mark></p><p id="a962e428-faa4-45c2-8ba2-1e830457c12b" class="">Para conectar dos dispositivos remotos es necesario establecer una conexión. La capa de transporte establece las reglas para esta interconexión. Permite que las estaciones finales ensamblen y reensamblen múltiples segmentos del mismo flujo de datos. Esto se hace por medio de identificadores que en TCP/IP reciben el nombre de números de puerto.</p><h3 id="4396dcc8-bf4f-45a3-b64a-183dae2fc025" class=""><mark class="highlight-blue"><strong>Capa de red</strong></mark></h3><p id="5371a628-d69e-4aa5-9e50-c6b1819aa3bd" class="">En esta capa se lleva a cabo el direccionamiento lógico.</p><p id="79130d25-d537-41bc-a91b-e91ed08d6be9" class="">Se selecciona la mejor ruta hacia el destino mediante el uso de tablas de enrutamiento a través del uso de protocolos de enrutamiento o por direccionamiento estático.</p><p id="1368fea2-1bfc-4bbc-a3b4-023a8f9fbd05" class=""><mark class="highlight-yellow"><strong><span style="border-bottom:0.05em solid">Funciones de la capa de enlace de red</span></strong></mark></p><p id="101dfe8e-3987-4a56-933a-a98a6a10d903" class="">La capa de red define cómo transportar el tráfico de datos entre dispositivos que no están conectados localmente en el mismo dominio de difusión, es decir, que pertenecen a diferentes redes. Para conseguir esta comunicación se necesita conocer las direcciones lógicas asociadas a cada puesto de origen y de destino y una ruta bien definida a través de la red para alcanzar el destino<br/>deseado.<br/></p><p id="d9cddf4a-80f6-4f22-a5ca-3b2795277735" class="">Una dirección lógica cuenta con dos partes bien definidas, una que identifica de forma única a la red dentro de un conjunto en la internetwork y la otra parte que representa al host dentro de estas redes. El router identifica dentro de la dirección lógica la porción perteneciente a la red con el fin de identificar la red donde enviar los paquetes.</p><p id="1d525b81-0fd7-4dd5-8206-4c2bfbbc970d" class=""><mark class="highlight-yellow"><strong><span style="border-bottom:0.05em solid">Dirección de capa tres</span></strong></mark></p><ul id="337d851c-34f1-4977-818f-66b8e744f438" class="bulleted-list"><li style="list-style-type:disc">Una dirección de 32 bits, dividida en cuatro octetos. Este direccionamiento identifica una porción perteneciente a la red y otra al host.</li></ul><ul id="c2e971bf-ef10-4fdf-b71d-1add66e1dd5d" class="bulleted-list"><li style="list-style-type:disc">A cada dirección IP le corresponde una máscara de red de 32 bits dividida en cuatro octetos. El router determina las porciones de red y host por medio de la máscara de red.</li></ul><ul id="a492c1b6-091d-47a0-9503-b4eefbfd943f" class="bulleted-list"><li style="list-style-type:disc">Las direcciones IP generalmente se representan en forma decimal para hacerlas más comprensibles. Esta forma se conoce como decimal punteado o notación decimal de punto.<p id="7df30f0b-8cf7-4c2d-830e-b230aa1e63db" class="">Dirección IP 172.16.1.3</p><p id="24681c4c-b562-4d94-b6be-1ed65989c73e" class="">Mascara 255.255.0.0</p><table id="08583029-87d4-450e-bad8-5d09c6252918" class="simple-table"><tbody><tr id="3afb61be-6359-4a14-bc81-f8fe22e10b35"><td id="x_{q" class="" style="width:76.5px">172</td><td id="AUMN" class="" style="width:77.5px">16</td><td id="kUtH" class="" style="width:88.5px">1</td><td id="c`VV" class="" style="width:80.5px">3</td></tr><tr id="189864de-c7ef-4bf3-804d-4c739d52e8c3"><td id="x_{q" class="" style="width:76.5px">10101100</td><td id="AUMN" class="" style="width:77.5px">00010000</td><td id="kUtH" class="" style="width:88.5px">00000001</td><td id="c`VV" class="" style="width:80.5px">00000011</td></tr><tr id="4ba0f613-414f-4ce7-9150-68f446324113"><td id="x_{q" class="" style="width:76.5px">255</td><td id="AUMN" class="" style="width:77.5px">255</td><td id="kUtH" class="" style="width:88.5px">0</td><td id="c`VV" class="" style="width:80.5px">0</td></tr><tr id="74742fe3-4c27-45ea-8221-3cf6b1eb63f2"><td id="x_{q" class="" style="width:76.5px">11111111</td><td id="AUMN" class="" style="width:77.5px">11111111</td><td id="kUtH" class="" style="width:88.5px">00000000</td><td id="c`VV" class="" style="width:80.5px">00000000</td></tr></tbody></table></li></ul><p id="655a9ef9-213a-4fa3-b1bb-d124af9915e6" class="">Las direcciones IPv6 miden 128 bits y son identificadores de interfaces individuales y conjuntos de interfaces. Las direcciones IPv6 se asignan a interfaces, no a nodos. Como cada interfaz pertenece a un solo nodo, cualquiera de las direcciones unicast asignada a las interfaces del nodo se pueden usar como identificadores del nodo. Las direcciones IPv6 se escriben en hexadecimal, separadas por dos puntos. Los campos IPv6 tienen una longitud de 16 bits.</p><p id="53e456a2-1788-41e3-bd04-e1b50e33cfdb" class="">Ejemplo de una dirección IPv6: 24ae:0000:f2f3:0000:0000:0687:a2ff:6184</p><p id="fff4020f-bd2c-8074-beeb-dd5f216c6a89" class=""><mark class="highlight-yellow"><strong><span style="border-bottom:0.05em solid">Comparación entre IPv4 y IPv6</span></strong></mark></p><p id="230ea212-968c-42e8-b6d8-c5527fd85813" class="">A mediados de los años noventa se comenzaron a detectar las siguientes<br/>dificultades sobre IPv4:<br/></p><ul id="2ae007bb-67b7-4d28-83d9-24f9949404ff" class="bulleted-list"><li style="list-style-type:disc">Agotamiento de las restantes direcciones de red IPv4 no asignadas. En ese entonces, el espacio de Clase B estaba a punto de agotarse.</li></ul><ul id="0568f466-7fcd-4e4b-acea-20c4af9f9b65" class="bulleted-list"><li style="list-style-type:disc">Se produjo un gran y rápido aumento en el tamaño de las tablas de enrutamiento de Internet a medida que las redes Clase C se conectaban en línea. La inundación resultante de nueva información en la red amenazaba la capacidad de los routers de Internet para ejercer una efectiva administración.</li></ul><p id="4d707f7f-be34-4ea2-9108-df972e998b63" class=""><mark class="highlight-yellow"><strong><span style="border-bottom:0.05em solid">Operación AND</span></strong></mark></p><p id="236a8cca-fd70-46ff-a29e-e7804a3ac883" class="">Los routers determinan la ruta de destino a partir de la dirección de red, estos comparan las direcciones IP con sus respectivas máscaras efectuando la operación booleana AND. Los routers ignoran el rango de host para encontrar la red destino a la que éste pertenece.</p><p id="bc9214ed-4074-4975-93ef-c36746cbec6f" class="">La operación AND consiste en comparar bit a bit la dirección IP y la máscara utilizando el siguiente razonamiento:</p><p id="8d259142-3ac6-4f03-b464-464d1d425265" class="">1x1=1<br/>1x0=0<br/>0x1=0<br/>0x0=0<br/></p><p id="046ac376-4c17-480e-bfe1-09fce2cdf599" class="">Binario:</p><p id="1fe6e68c-1293-4502-8bc9-5ed4541e8df8" class="">Dirección de host 10101100.00100000.00000001.00000011<br/>Máscara de red 11111111.11111111.00000000.00000000<br/>Dirección de red 10101100.00100000.00000000.00000000<br/></p><p id="b5d6d480-6026-4992-a064-54dc5039a2fb" class="">Decimal:</p><p id="fe07fdeb-1f45-4828-9dfe-92d2c77c251b" class="">Dirección de host 172. 16. 1. 3<br/>Máscara de red 255. 255. 0. 0<br/>Dirección de red 172. 16. 0. 0<br/></p><p id="5b56fe7f-693e-4800-88e0-382babecfa03" class=""><mark class="highlight-yellow"><strong><span style="border-bottom:0.05em solid">Dispositivos de la capa de red</span></strong></mark></p><p id="88f3b263-ec65-4b54-893d-068a2aef9737" class="">Los routers funcionan en la capa de red del modelo OSI separando los segmentos en dominios de colisión y difusión únicos. Estos segmentos están identificados por una dirección de red que permitirá alcanzar las estaciones finales.</p><p id="22e7bcdc-babc-4cf0-a130-e1db7cba22d5" class="">Los routers cumplen dos funciones básicas que son la de enrutar y conmutar los paquetes.</p><p id="64774d30-4a00-47c4-ba29-f5b35cfdbb94" class="">Además de identificar redes y proporcionar conectividad, los routers deben<br/>proporcionar estas otras funciones:<br/></p><ul id="f2a0709a-168f-476b-8c51-6fb07a2416e9" class="bulleted-list"><li style="list-style-type:disc">Los routers no envían difusiones de capa 2 ni tramas de multidifusión.</li></ul><ul id="472c40f7-22e6-4b13-8488-093a842cceef" class="bulleted-list"><li style="list-style-type:disc">Los routers intentan determinar la ruta óptima a través de una red enrutada basándose en algoritmos de enrutamiento.</li></ul><ul id="5a8e8e39-8cd1-400b-8f1e-ed699f546c1f" class="bulleted-list"><li style="list-style-type:disc">Los routers separan las tramas de capa 2 y envían paquetes basados en<br/>direcciones de destino capa 3.<br/></li></ul><ul id="afe3cbfa-29bf-49ec-a410-6bc20597ea97" class="bulleted-list"><li style="list-style-type:disc">Los routers asignan una dirección lógica de capa 3 individual a cada dispositivo de red; por tanto, los routers pueden limitar o asegurar el tráfico de la red basándose en atributos identificables con cada paquete. Estas opciones, controladas por medio de listas de acceso,<br/>pueden ser aplicadas para incluir o descartar paquetes.<br/></li></ul><ul id="af1dbc49-aa35-46c3-8906-63f167755059" class="bulleted-list"><li style="list-style-type:disc">Los routers pueden ser configurados para realizar funciones tanto de puenteado como de enrutamiento.</li></ul><ul id="981b5e36-fff1-4fb2-9fbd-39108e58c9cd" class="bulleted-list"><li style="list-style-type:disc">Los routers proporcionan conectividad entre diferentes LAN virtuales (VLAN) en entornos conmutados.</li></ul><ul id="3a76c123-485e-428d-9950-b7be779dd41b" class="bulleted-list"><li style="list-style-type:disc">Los routers pueden ser usados para desplegar parámetros de calidad de servicio para tipos específicos de tráfico de red.</li></ul><p id="0b717f57-e735-42ce-938b-dbe0dc83502c" class="">Los routers conocen los diferentes destinos manteniendo tablas de enrutamiento que contienen la siguiente información:</p><ul id="4977dca8-8335-48e7-b860-90bf25fdab1b" class="bulleted-list"><li style="list-style-type:disc"><strong>Dirección de red</strong>. Representa redes conocidas por el router. La dirección de red es específica del protocolo.</li></ul><ul id="74566c88-2b02-414c-9a5c-b9ce7aef1530" class="bulleted-list"><li style="list-style-type:disc"><strong>Interfaz</strong>. Se refiere a la interfaz usada por el router para llegar a una red dada. Esta es la interfaz que será usada para enviar los paquetes destinados a la red que figura en la lista.</li></ul><ul id="a38e84e7-b838-4c6d-b96b-f5b1357d0275" class="bulleted-list"><li style="list-style-type:disc"><strong>Métrica</strong>. Se refiere al coste o distancia para llegar a la red de destino. Se trata de un valor que facilita al router la elección de la mejor ruta para alcanzar una red dada. Entre las métricas más habituales figuran el número de redes que han de ser cruzadas para llegar al destino (conocido también como saltos), el tiempo que se tarda en atravesar todas las interfaces hasta una red dada (conocido también como retraso), o un valor asociado con la velocidad de un enlace (conocido también como ancho de banda).</li></ul><p id="4afd184a-8971-4b64-8183-cd9ec271a1ed" class="">En la siguiente salida del router se observa una tabla de enrutamiento con las direcciones IP de destino (172.25.25.6/32), la métrica ([120/2]) y la correspondiente interfaz de salida Serial 0.1.</p><script src="https://cdnjs.cloudflare.com/ajax/libs/prism/1.29.0/prism.min.js" integrity="sha512-7Z9J3l1+EYfeaPKcGXu3MS/7T+w19WtKQY/n+xzmw4hZhJ9tyYmcUS+4QqAlzhicE5LAfMQSF3iFTK9bQdTxXg==" crossorigin="anonymous" referrerPolicy="no-referrer"></script><link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/prism/1.29.0/themes/prism.min.css" integrity="sha512-tN7Ec6zAFaVSG3TpNAKtk4DOHNpSwKHxxrsiw4GHKESGPs5njn/0sMCUMl2svV4wo4BK/rCP7juYz+zx+l6oeQ==" crossorigin="anonymous" referrerPolicy="no-referrer"/><pre id="4929079a-df77-461f-af9e-193801ec50b6" class="code"><code class="language-XML">Router2#show ip route rip
R 172.21.0.0/16 [120/1] via 172.25.2.1, 00:00:01, Serial0.1
R 172.22.0.0/16 [120/1] via 172.25.2.1, 00:00:01, Serial0.1
172.25.0.0/16 is variably subnetted, 6 subnets, 3 masks
R 172.25.25.6/32 [120/2] via 172.25.2.1, 00:00:01, Serial0.1
R 172.25.25.1/32 [120/1] via 172.25.2.1, 00:00:01, Serial0.1
R 172.25.1.0/24 [120/1] via 172.25.2.1, 00:00:01, Serial0.1
R 172.25.0.0/16 [120/1] via 172.25.2.1, 00:00:01, Serial0.1</code></pre><p id="a6462429-a767-42e5-bc93-8db766178bf3" class="">Los Firewalls trabajan principalmente en la capa de Red del modelo OSI y generalmente se los considera dispositivos de esta capa. Sin embargo, algunos firewalls, analizan tráfico basándose en información de las capas 3, 4, 5 y 7 del modelo de referencia OSI, como protocolo y números de puerto de origen y destino. El filtrado de paquetes utiliza las ACL para determinar si permite o deniega tráfico basándose en direcciones IP de origen y destino, protocolo, tipo de paquete y números de puerto origen y destino. Los firewalls de filtrado de paquetes generalmente son parte de un router con funcionalidad de firewall.</p><h3 id="9240ae04-dfd9-4884-a698-aef7e4865250" class=""><mark class="highlight-blue"><strong>Capa de enlace de datos</strong></mark></h3><p id="5dc77cd3-9328-476d-9835-9376a2367fe8" class="">Proporciona las comunicaciones entre puestos de trabajo en una primera capa lógica, transforma los voltios en tramas y las tramas en voltios. El direccionamiento físico y la determinación de si deben subir un mensaje a la pila de protocolo ocurren en esta capa. Está dividida en dos subcapas, la LLC (Logical Link Control) y la subcapa MAC (Media Access Control).</p><p id="b9210b63-1927-46cf-936e-36065cfbadd0" class=""><mark class="highlight-yellow"><strong><span style="border-bottom:0.05em solid">Funciones de la capa de enlace de datos</span></strong></mark></p><p id="4ce92c6e-fe25-4d63-9022-0904dc5ae30e" class="">La finalidad de esta capa es proporcionar comunicación entre puestos de trabajo en una primera capa lógica que hay por encima de los bits del cable.</p><p id="fff4020f-bd2c-8053-bf6c-eccb770821d0" class="">La capa de enlace de datos da soporte a servicios basados en la conectividad y no basados en ella, y proporciona la secuencia y control de flujo. Tiene conocimiento de la topología a la que está afectada y donde se desempeña la tarjeta de red o NIC.</p><p id="84a3c7e7-b675-4b03-8a47-c45333de77b8" class="">Está dividida en dos subcapas, la LLC,  responsable de la identificación lógica de los distintos tipos de protocolos y el encapsulado posterior de los mismos para ser transmitidos a través de la red, y la subcapa MAC, responsable del acceso al medio, el direccionamiento físico, topología de la red, disciplina de la línea, notificación de errores, distribución ordenada de tramas y control óptimo de flujo.</p><h3 id="6ec303eb-cb46-4292-84d6-63e72a106b17" class=""><mark class="highlight-blue"><strong>Capa física</strong></mark> </h3><p id="c360aaa7-b5ba-4de1-b58b-9d62af7c95ab" class="">Los bits son transformados en pulsos eléctricos, en luz o en radiofrecuencia para ser enviados según sea el medio en que se propaguen.</p><p id="10fe9ba2-c22c-400b-8e27-ca53b74ed931" class=""><mark class="highlight-yellow"><strong><span style="border-bottom:0.05em solid">Funciones de la capa física</span></strong></mark></p><p id="0839d148-8fff-4026-81e9-d89bee7b961b" class="">La capa física define el medio, el conector y el tipo de señalización. Se<br/>especifican los requisitos necesarios para la correcta transmisión de los datos.<br/></p><p id="bd4e64c6-91fa-43bd-a714-f5540b72159e" class="">La capa física especifica también características tales como niveles de voltaje, tasas de transferencia de datos, distancias máximas de transmisión y conectores, cada medio de red posee a su vez su propio ancho de banda y unidad máxima de transmisión (MTU).</p><p id="a802facf-eb98-469a-98cd-9e9e4ff83672" class=""><mark class="highlight-yellow"><strong><span style="border-bottom:0.05em solid">Topologías</span></strong></mark><mark class="highlight-yellow"> </mark></p><ol type="1" id="f3170471-bc0c-4add-a745-34ac1cee8f09" class="numbered-list" start="1"><li><strong>Bus</strong>: esta topología permite que todas las estaciones reciban la<br/>información que se transmite, una estación transmite y todas las<br/>restantes escuchan.<br/></li></ol><ol type="1" id="4bc5d82b-f0a8-47ff-84d9-a2db28680ac1" class="numbered-list" start="2"><li><strong>Anillo</strong>: las estaciones están unidas unas con otras formando un círculo<br/>por medio de un cable común. El último nodo de la cadena se conecta<br/>al primero cerrando el anillo.<br/></li></ol><ol type="1" id="fff4020f-bd2c-802b-86c0-e136d30a42ec" class="numbered-list" start="3"><li><strong>Estrella</strong>: los datos en estas redes fluyen del emisor hasta un<br/>concentrador, que realiza las funciones de enviar y recibir las señales<br/>de red.<br/></li></ol><ol type="1" id="9452a04f-ec55-46ac-8e2e-4375adc51ab3" class="numbered-list" start="4"><li><strong>Estrella extendida</strong>: es la combinación de dos o más topologías en<br/>estrella unidas entre sí por sus respectivos concentradores.<br/></li></ol><ol type="1" id="1558f6d2-ba2e-412d-88b4-2470ee91f612" class="numbered-list" start="5"><li><strong>Híbridas</strong>: es una combinación de todas las anteriores.</li></ol><p id="5059e859-9de8-46c2-ad9f-9f905eaecc74" class="">
</p><table id="e261f1ac-e147-490c-965b-a25923617224" class="simple-table"><tbody><tr id="6ea47a38-007b-495c-bbf9-94d7e5bd7f6d"><td id="H&gt;RP" class="" style="width:35px">7</td><td id="Xoe&gt;" class="" style="width:224px">Aplicación</td><td id="?tJX" class="" style="width:310px">HTML, http, telnet, FTP, TFTP…</td></tr><tr id="77db697a-ce4c-498c-b733-15420e68d6bd"><td id="H&gt;RP" class="" style="width:35px">6</td><td id="Xoe&gt;" class="" style="width:224px">Presentación</td><td id="?tJX" class="" style="width:310px">JPEG, MIDI, MPEG, ASCII, Quicktime…</td></tr><tr id="68e01785-e877-4ff4-8f3c-8d0d360090f8"><td id="H&gt;RP" class="" style="width:35px">5</td><td id="Xoe&gt;" class="" style="width:224px">Sesión</td><td id="?tJX" class="" style="width:310px">Control de diálogo</td></tr><tr id="c0ca7dd9-3376-4c50-bf01-48567409e94c"><td id="H&gt;RP" class="" style="width:35px">4</td><td id="Xoe&gt;" class="" style="width:224px">Transporte</td><td id="?tJX" class="" style="width:310px">Control de flujo, TCP, UDP…</td></tr><tr id="f052bba9-cc50-42cf-9030-27f78692c0f6"><td id="H&gt;RP" class="" style="width:35px">3</td><td id="Xoe&gt;" class="" style="width:224px">Red</td><td id="?tJX" class="" style="width:310px">Enrutamiento, IP, IPX, RIP, IGRP, Apple Talk…</td></tr><tr id="5255ff59-69f8-413a-8189-66554e67b520"><td id="H&gt;RP" class="" style="width:35px">2</td><td id="Xoe&gt;" class="" style="width:224px">Enlace de datos</td><td id="?tJX" class="" style="width:310px">Ethernet, 802.2, 802.3, HDLC, Frame-Relay…</td></tr><tr id="0b9aef1b-cacb-44e1-84d7-c60891871704"><td id="H&gt;RP" class="" style="width:35px">1</td><td id="Xoe&gt;" class="" style="width:224px">Física </td><td id="?tJX" class="" style="width:310px">Bits, RJ45…</td></tr></tbody></table><h1 id="8580d554-d30d-4894-9b5b-785889625e1b" class=""><mark class="highlight-purple">3. Modelo TCP/IP</mark></h1><p id="068dc5e2-76a1-4cdb-9795-637025ca3efd" class="">El Departamento de Defensa de EE.UU. (DoD) creó el modelo de referencia TCP/IP porque necesitaba una red que pudiera sobrevivir ante cualquier circunstancia. Para tener una mejor idea, imagine un mundo, cruzado por numerosos tendidos de cables, alambres, microondas, fibras ópticas y enlaces<br/>satelitales.<br/></p><p id="2fa0ae70-a1b5-48a8-b673-870267d73c82" class="">El modelo TCP/IP tenía originalmente cuatro capas: la capa de aplicación, la capa de transporte, la capa de Internet y la capa de acceso de red (NAL). Posteriormente en una actualización del modelo la capa de acceso a la red se ha dividido en dos subcapas.</p><table id="18e46da0-f951-415c-a4b4-5d842d060faa" class="simple-table"><tbody><tr id="e08d7e85-999f-4f30-8d22-4181ec51fcee"><td id="EjH|" class="">TCP/IP Original</td><td id="xXm[" class="">TCP/IP Actualizado</td></tr><tr id="25877e40-0322-424c-9e48-26cfc618b2f6"><td id="EjH|" class="">Aplicación</td><td id="xXm[" class="">Aplicación </td></tr><tr id="6c58935b-1b11-425f-a693-084ab1bf8f36"><td id="EjH|" class="">Transporte</td><td id="xXm[" class="">Transporte</td></tr><tr id="5c2b4fce-ba9c-46fd-94cc-1ee0b1308546"><td id="EjH|" class="">Internet</td><td id="xXm[" class="">Red</td></tr><tr id="5d73dff8-668c-4e5f-b3ec-d54ed843dedd"><td id="EjH|" class="">Acceso a la red</td><td id="xXm[" class="">Enlace de datos</td></tr><tr id="ca499b0b-e20a-4cfe-947f-63012fe43778"><td id="EjH|" class=""></td><td id="xXm[" class="">Física</td></tr></tbody></table><p id="040417ec-c142-4c2f-9dc5-d24bda56553d" class="">Es importante observar que algunas de las capas del modelo TCP/IP poseen el mismo nombre que las capas del modelo OSI. Resulta fundamental no confundir las funciones de las capas de los dos modelos</p><table id="47976539-6a3b-4ef2-a458-29d6b6d7e885" class="simple-table"><tbody><tr id="67df8515-93c1-4038-ba44-d5b67c216ab3"><td id="uAGl" class="" style="width:107px">OSI</td><td id="q=tB" class="">TCP/IP</td><td id="HANK" class="">Protocolos</td></tr><tr id="83d25cf4-3144-456b-beee-deacc4e8697d"><td id="uAGl" class="" style="width:107px">Aplicación</td><td id="q=tB" class=""></td><td id="HANK" class="">Telnet, FTP, LPD,</td></tr><tr id="b2c43ff7-276b-4d78-be60-4e9f0f182e6b"><td id="uAGl" class="" style="width:107px">Presentación/Sesión</td><td id="q=tB" class="">Aplicación</td><td id="HANK" class="">SNMP,TFTP, SMTP,<br/>NFS, HTTP, X Windows<br/></td></tr><tr id="2d30555d-8424-4a7a-9d5c-860faf6d4914"><td id="uAGl" class="" style="width:107px">Transporte</td><td id="q=tB" class="">Transporte</td><td id="HANK" class="">TCP, UDP</td></tr><tr id="e5455e04-2586-4066-a829-d425ca922098"><td id="uAGl" class="" style="width:107px">Red</td><td id="q=tB" class="">Internet</td><td id="HANK" class="">ICMP, BOOTP, ARP,<br/>RARP, IP<br/></td></tr><tr id="ab96fd92-6ff1-4cd9-bf41-a44646461c1d"><td id="uAGl" class="" style="width:107px">Enlace de datos/Física</td><td id="q=tB" class="">Red</td><td id="HANK" class="">Ethernet,<br/>Fast-Ethernet,<br/>Token Ring, FDDI<br/></td></tr></tbody></table><h2 id="1fef00eb-628a-43e4-aa0e-5772f5680a5a" class="">3.1 Protocolos de capa de aplicación</h2><p id="404247a4-a8a6-452b-9463-6b1b85a3197f" class="">Los protocolos describen el conjunto de normas y convenciones que rigen la forma en que los dispositivos de una red intercambian información. Algunos de los protocolos de la capa de Aplicación del modelo TCP/IP son:</p><ul id="f3b4b82f-3296-4e97-ba45-084a6d0665b8" class="bulleted-list"><li style="list-style-type:disc"><strong>Telnet</strong>. Protocolo de emulación de terminal estándar que se usa para la conexión de terminales remotas, permitiendo que los usuarios se registren en dichos sistemas y utilicen los recursos como si estuvieran conectados localmente.</li></ul><ul id="a394f29d-bdc2-4cac-89b6-1390f8b05b24" class="bulleted-list"><li style="list-style-type:disc"><strong>FTP</strong>. Protocolo utilizado para transferir archivos entre host de red de manera confiable ya que utiliza un mecanismo orientado a conexión.</li></ul><ul id="b273f528-64ee-4bfb-8e3b-9af80ba30381" class="bulleted-list"><li style="list-style-type:disc"><strong>TFTP</strong>. Versión simplificada de FTP que permite la transferencia de archivos de un host a otro a través de una red de manera menos confiable.</li></ul><ul id="b2fee516-f2ed-4439-8f68-44c9503c7f52" class="bulleted-list"><li style="list-style-type:disc"><strong>DNS</strong>. El sistema de denominación de dominio es utilizado en Internet para convertir los nombres de los nodos de red en direcciones.</li></ul><ul id="79b36dcc-ce50-4f39-b6f2-9c33f3760d7d" class="bulleted-list"><li style="list-style-type:disc"><strong>SMTP</strong>. Protocolo simple de transferencia de correo basado en texto utilizado para el intercambio de mensajes de correo electrónico entre distintos dispositivos.</li></ul><ul id="05ed7289-3c0a-4355-acfa-0f0e50f01df3" class="bulleted-list"><li style="list-style-type:disc"><strong>SNMP</strong>. Protocolo de administración de redes utilizado casi con exclusividad en redes TCP/IP. El SNMP brinda una forma de monitorizar y controlar los dispositivos de red y de administrar configuraciones.</li></ul><ul id="654d8cd7-9509-4f73-aa7d-7be950a0d49b" class="bulleted-list"><li style="list-style-type:disc"><strong>DHCP.</strong> Protocolo de configuración dinámica del host. Protocolo que proporciona un mecanismo para asignar direcciones IP de forma dinámica.</li></ul><h2 id="4efd4522-6f05-409a-b200-4d1038f4a238" class="">3.2 Protocolos de capa de transporte</h2><p id="5ba9301e-3d77-44fc-a882-0c1e70edc0a3" class="">Los protocolos de la capa de transporte se encargan de dar soporte a la capa superior brindando apoyo enviando los datos sin importar el contenido de los mismos. Los dos protocolos extensamente conocidos para tal proceso son:</p><ul id="534c8fdc-b050-4b7f-a5ed-398769a214a5" class="bulleted-list"><li style="list-style-type:disc"><strong>TCP.</strong> Protocolo de control de transmisión, es básicamente el más utilizado, tiene control de flujo, reensamblado de paquetes y acuses de recibo. Es un protocolo orientado a conexión muy seguro que utiliza un saludo de tres vías antes del envío de los datos.<p id="984bf32d-6378-431c-8e35-d76bb4cca623" class="">
</p></li></ul><ul id="a7999d76-1372-4103-97ef-d9f225e8da71" class="bulleted-list"><li style="list-style-type:disc"><strong>UDP</strong>. El protocolo de datagrama del usuario es en general menos seguro que TCP, no tiene corrección de errores y es del tipo no orientado a conexión, los datos se envían sin verificar previamente el destino.</li></ul><p id="aea6c2e9-b071-45e7-89cb-22475038c765" class="">TCP utiliza una técnica llamada ventanas, donde se establece la cantidad de envío de paquetes antes de transmitir; mientras que en el windowing  el flujo de envío de datos es negociado dinámicamente<br/>entre el emisor y el receptor. En las ventanas deslizantes o windowing cada acuse de recibo ACK (acknowledgement) confirma la recepción y el envío siguiente.<br/></p><figure class="block-color-gray_background callout" style="white-space:pre-wrap;display:flex" id="f2d34d31-ac9a-4ec5-941b-ba83c2443db3"><div style="font-size:1.5em"><span class="icon">💡</span></div><div style="width:100%">TCP, protocolo confiable de capa de transporte orientado a conexión.<br/>UDP, protocolo NO confiable de capa de transporte NO orientado a conexión.<br/><p id="5b138414-2c88-48db-b0c5-66bef5503054" class="">Un protocolo orientado a conexión es el que previamente establece un saludo antes de enviar los datos.</p></div></figure><h2 id="a5e47aa1-c2d6-4dcc-8885-bdf4e01f4963" class="">3.3 Números de puertos</h2><p id="79b2c727-b26a-447b-8fdb-5058f75adb49" class="">Los números de puerto son utilizados por TCP y UDP para identificar sesiones de diferentes aplicaciones, los números de puertos ocupan rangos definidos que van desde puertos bien conocidos hasta puertos específicos determinados por los usuarios.</p><p id="3b27aa02-17f0-4afd-b65b-1621d04916c9" class="">
</p><figure id="5a39df03-645f-4cae-8ccd-059d8264a551" class="image"><a href="image.png"><img style="width:281px" src="image.png"/></a></figure><p id="6fd419f2-a775-415f-85cd-2760d2cf97aa" class="">
</p><p id="1bd33d5d-36b0-4fae-9382-1401848ac282" class="">A continuación, se detallan los números de puertos más comunes:</p><table id="5bbe29f2-0255-4a2d-bb30-e62e96bc82cd" class="simple-table"><tbody><tr id="e7b2951b-eb11-4f38-a4f7-f781031ee8b8"><td id=":vf_" class="" style="width:62px">Nº de puerto</td><td id="LS}[" class="">Protocolo</td></tr><tr id="1a56b61b-552d-47fd-9281-99801499de0b"><td id=":vf_" class="" style="width:62px">7</td><td id="LS}[" class="">Echo</td></tr><tr id="7f3b894c-65ca-41ae-8bb3-6dc8697d91f9"><td id=":vf_" class="" style="width:62px">9</td><td id="LS}[" class="">Discard</td></tr><tr id="0be3d01c-5310-4b1e-b679-3870de723d63"><td id=":vf_" class="" style="width:62px">13</td><td id="LS}[" class="">Daytime</td></tr><tr id="29224966-d53e-49e5-a51f-dce930a0e8ec"><td id=":vf_" class="" style="width:62px">19 </td><td id="LS}[" class="">Character Generator</td></tr><tr id="6af96b7a-8067-40ef-b305-3db18818698d"><td id=":vf_" class="" style="width:62px">20</td><td id="LS}[" class="">FTP Data Connections</td></tr><tr id="eed92709-ed5f-4bb2-9243-ec8206924044"><td id=":vf_" class="" style="width:62px">21</td><td id="LS}[" class="">File Transfer Protocol</td></tr><tr id="9309a8c7-b50a-434a-88e4-6db9642b4fa1"><td id=":vf_" class="" style="width:62px">23</td><td id="LS}[" class="">Telnet</td></tr><tr id="135f0642-ab77-4aec-9ad1-befccfea8773"><td id=":vf_" class="" style="width:62px">25</td><td id="LS}[" class="">Simple Mail Transport Protocol</td></tr><tr id="4067a419-db1d-4851-846b-d064853b919d"><td id=":vf_" class="" style="width:62px">37</td><td id="LS}[" class="">Time</td></tr><tr id="356a6d99-c5cc-4fc4-b62e-02169b9f0d88"><td id=":vf_" class="" style="width:62px">53</td><td id="LS}[" class="">Domain Name Service</td></tr><tr id="d2d9e674-7e13-496f-af8b-af90beffbec2"><td id=":vf_" class="" style="width:62px">43</td><td id="LS}[" class="">Nicname</td></tr><tr id="89d28164-6da0-4cd9-b803-4d864d6da79d"><td id=":vf_" class="" style="width:62px">49</td><td id="LS}[" class="">TAC Access Control System</td></tr><tr id="2c4d66c7-d525-4ba8-9bf7-330d2351f8a7"><td id=":vf_" class="" style="width:62px">69</td><td id="LS}[" class="">Trivial File Transfer Protocol</td></tr><tr id="349855d6-7041-4ce8-a3ef-acdbdf9c5013"><td id=":vf_" class="" style="width:62px">70</td><td id="LS}[" class="">Gopher</td></tr><tr id="f4e34903-a70f-48dc-a684-a403b879c014"><td id=":vf_" class="" style="width:62px">79</td><td id="LS}[" class="">Finger</td></tr><tr id="aabc074a-3425-400f-b8fb-e41c7254bed9"><td id=":vf_" class="" style="width:62px">80</td><td id="LS}[" class="">World Wide Web</td></tr><tr id="735a4778-f58a-47d2-9c76-57b6fa52ca91"><td id=":vf_" class="" style="width:62px">101</td><td id="LS}[" class="">NIC hostname server</td></tr><tr id="bd325fa3-1114-471d-a4f3-51bef00b5754"><td id=":vf_" class="" style="width:62px">109</td><td id="LS}[" class="">Post Office Protocol v2</td></tr><tr id="94f4b698-c901-45aa-80b4-2fd2778105ec"><td id=":vf_" class="" style="width:62px">110</td><td id="LS}[" class="">Post Office Protocol v3</td></tr><tr id="12d49cf8-3ca0-47e3-b3dc-24521c71fba4"><td id=":vf_" class="" style="width:62px">111</td><td id="LS}[" class="">Sun Remote Procedure Call</td></tr><tr id="ba1583c4-bdd7-4a7a-a998-000e88fd6a87"><td id=":vf_" class="" style="width:62px">113</td><td id="LS}[" class="">Ident Protocol</td></tr><tr id="76bf0886-c052-45a4-be78-9505de759f04"><td id=":vf_" class="" style="width:62px">119</td><td id="LS}[" class="">Network News Transport Protocol</td></tr><tr id="fa1779d6-0511-45ce-a53c-22b47b31b989"><td id=":vf_" class="" style="width:62px">179</td><td id="LS}[" class="">Border Gateway Protocol</td></tr></tbody></table><h2 id="e5f3908b-69a6-4438-9fa9-ae8e208b230f" class="">3.4 Protocolos de capa de internet</h2><p id="91e7109b-7919-4e0a-95c1-60fa818d654d" class="">Estos son algunos de los protocolos más usados que operan en la capa de Internet del modelo TCP/IP:</p><ul id="6fbbe34e-8d12-4f89-a601-24161ba36e8c" class="bulleted-list"><li style="list-style-type:disc"><strong>IP</strong>. Protocolo de Internet, proporciona un enrutamiento de paquetes no orientado a conexión de máximo esfuerzo. IP no se ve afectado por el contenido de los paquetes, sino que busca una ruta hacia el destino.</li></ul><ul id="0be5ebdc-83fb-4ba3-965b-45c8cc30175e" class="bulleted-list"><li style="list-style-type:disc"><strong>ARP</strong>. Protocolo de resolución de direcciones, determina la dirección de la capa de enlace de datos, la dirección MAC, para las direcciones IP conocidas.</li></ul><ul id="8589d7a9-5938-407e-8a67-4a664b84d78c" class="bulleted-list"><li style="list-style-type:disc"><strong>RARP</strong>. Protocolo de resolución inversa de direcciones, determina las direcciones IP cuando se conoce la dirección MAC.</li></ul><ul id="e1caceba-d4f4-4c41-ae98-7d9f6d3e0345" class="bulleted-list"><li style="list-style-type:disc"><strong>ICMP</strong>. Protocolo de mensajes de control en Internet, suministra capacidades de control y envío de mensajes. Herramientas tales como PING y tracert utilizan ICMP para poder funcionar, enviando un paquete a la dirección destino específica y esperando una determinada respuesta. ICMP se describe con más detalle más adelante.</li></ul><figure class="block-color-gray_background callout" style="white-space:pre-wrap;display:flex" id="2e6129c9-8ece-493e-8dbc-2d613ba7fdff"><div style="font-size:1.5em"><span class="icon">💡</span></div><div style="width:100%">La capa de Acceso a la Red está dividida en dos subcapas: Enlace de datos y Física. La capa de Internet también es llamada capa de Interred o capa de red.</div></figure><h1 id="324a4402-c35a-4fb6-8efd-4a6d2eab4ef6" class=""><mark class="highlight-purple">4. Ethernet</mark></h1><p id="0940cf21-d005-4dc0-a406-51cea0d73b0d" class="">Ethernet es la tecnología de acceso al medio más popular, es escalable, económica y fácilmente integrable a nuevas aplicaciones, se pueden obtener arquitecturas de LAN a velocidades de Gigabit sobre cobre y la resolución de fallos suele ser simple y rápida.</p><p id="d9ee7b2b-5385-4589-953e-ac8c23bf94bf" class="">Ethernet es una tecnología conflictiva de máximo esfuerzo, todos los equipos de trabajo que se conectan al mismo medio físico reciben las señales enviadas por otros dispositivos. Si dos estaciones transmiten a la vez, se genera una colisión. Si no existieran mecanismos que detectasen y corrigiesen los errores de estas colisiones, Ethernet no podría funcionar.</p><p id="df765613-9c08-478f-9d8d-3eb14796d147" class="">El uso más adecuado del ancho de banda permite casi duplicarse al poder transmitir y recibir al 100% de capacidad.</p><p id="8572106f-31c4-4e40-b305-2774187ab3a5" class="">En el diseño de una red Ethernet se debe tener especial cuidado con los llamados dominios de colisión y dominios de difusión (broadcast) debido a que la excesiva cantidad de colisiones o de broadcast (tormentas de broadcast) harían inaceptable el funcionamiento de Ethernet.</p><h2 id="f7e7dadd-1fa2-4be6-a12b-95f131ffd4cf" class="">4.1 Dominio de colisión</h2><p id="faa30b25-3b93-4766-8e4a-03ef8b943986" class="">Grupo de dispositivos conectados al mismo medio físico, de tal manera que, si dos dispositivos acceden al medio al mismo tiempo, el resultado será una colisión entre las dos señales. Como resultado de estas colisiones se produce un consumo inadecuado de recursos y de ancho de banda.</p><h2 id="6d706740-3250-4c3e-9914-73fe05dd1bf1" class="">4.2 Dominio de difusión</h2><p id="05bba5d8-0602-413e-a6ad-3762e783df86" class=""> Grupo de dispositivos de la red que envían y reciben mensajes de difusión entre ellos. Una cantidad excesiva de estos mensajes de difusión (broadcast) provocará un bajo rendimiento en la red, una cantidad exagerada (tormenta de broadcast) dará como resultado el mal funcionamiento de la red hasta tal punto de poder dejarla completamente congestionada.</p><p id="5d52889a-96ee-4895-bb5a-a507403c7750" class="">Los hubs o concentradores tienen un único dominio de colisión, eso quiere decir que si dos equipos provocan una colisión en un segmento asociado a un puerto del hub, todos los demás dispositivos aun estando en diferentes puertos se verán afectados.</p><p id="0c627fd3-9d39-4855-b76b-1318100303bf" class="">
</p><figure id="42d7ace0-4adb-4de8-b90f-bd77b8914544" class="image"><a href="image%201.png"><img style="width:624px" src="image%201.png"/></a></figure><figure id="3503b6f6-d041-4435-9c9e-fd05bb754cc3" class="image"><a href="image%202.png"><img style="width:624px" src="image%202.png"/></a></figure><figure id="ef9aa7ef-ae7a-4c9a-b90a-5a0484fb4679" class="image"><a href="image%203.png"><img style="width:528px" src="image%203.png"/></a></figure><p id="58014f3a-af61-440e-ba65-802cde65be46" class="">
</p><p id="c4608b54-a788-4d83-8959-3b1ba76b4603" class="">Comparativa entre dominios de colisión y dominios de difusión en dispositivos de tres capas diferentes</p><figure class="block-color-gray_background callout" style="white-space:pre-wrap;display:flex" id="0c1eedbe-5605-40ef-a284-622d00c269b4"><div style="font-size:1.5em"><span class="icon">💡</span></div><div style="width:100%">Asocie a los routers como los dispositivos que crean dominios de difusión y a los switches<br/>como los que crean dominios de colisión.<br/></div></figure><h2 id="64025164-ca35-45b1-9f33-7768e2b4a90c" class="">4.3 CSMA/CD</h2><p id="cf4dd6cd-614f-4ca4-8c4c-7a739d8e0065" class="">En la práctica, esto significa que varios puestos pueden tener acceso al medio y que, para que un puesto pueda acceder a dicho medio, deberá detectar la portadora para asegurarse de que<br/>ningún otro puesto esté utilizándolo. Si el medio se encuentra en uso, el puesto procederá a mantener en suspenso el envío de datos. En caso de que haya dos puestos que no detectan ningún otro tráfico, ambos tratarán de transmitir al mismo tiempo, dando como resultado una colisión.<br/></p><p id="b1092145-77a5-498e-a7c0-c0bbcbd1487f" class="">A partir de esta colisión las estaciones emiten una señal de congestión para asegurarse de que existe una colisión y se genera un algoritmo de espera.</p><figure class="block-color-gray_background callout" style="white-space:pre-wrap;display:flex" id="b97cd08b-aaf7-44d2-9b46-6ac3ea2e84b0"><div style="font-size:1.5em"><span class="icon">💡</span></div><div style="width:100%">El ejemplo más claro de CSMA/CD es el de “escucho y luego transmito”.</div></figure><p id="3c1b19aa-411b-4adf-8345-b8633ee2d204" class="">
</p><figure id="cc482c9a-d581-4917-a89f-c65252be4150" class="image"><a href="image%204.png"><img style="width:624px" src="image%204.png"/></a></figure><h2 id="049fef27-7d29-4d82-b5b2-9d7ef0a58ba6" class="">4.4 Operación dúplex</h2><p id="280aa9d1-4c65-440e-8cbb-3ed5426a0186" class="">En las comunicaciones de datos, dúplex se refiere a la dirección de transmisión de los datos entre dos dispositivos.</p><ul id="8a3ffb6d-4a8e-4714-96ea-474386312207" class="bulleted-list"><li style="list-style-type:disc"><strong>Half-duplex:</strong> la comunicación se limita al intercambio de datos en una dirección a la vez.</li></ul><ul id="394619db-3664-489f-becd-44f8c4e76e4a" class="bulleted-list"><li style="list-style-type:disc"><strong>Full-dúplex</strong>: la comunicación es simultánea y permite al envío y recepción de datos al mismo tiempo.</li></ul><p id="9b77e478-9d06-472e-81a8-0c79b0c5ffbd" class="">Los dispositivos interconectados deben funcionar en el mismo modo dúplex para evitar problemas en el enlace.</p><p id="68b309ac-6077-4516-8f16-494ed86b34cb" class="">Los dúplex mismatches son desajustes en el modo dúplex y producen problemas de comunicación<br/>entre los dispositivos. Pueden ser difíciles de solucionar porque pueden no ser evidentes incluso cuando se utilizan herramientas como ping.<br/></p><h2 id="cb635444-a6b7-45fd-b57e-74c4bf1dd388" class="">4.5 Formato básico de una trama Ethernet</h2><p id="ab81e06b-82dd-4055-bbd6-a221339b4cac" class="">El formato de la trama del estándar IEEE 802.3 y el de Ethernet creado por Xerox son muy similares y compatibles, solo difieren en algunas pequeñas cuestiones de concepto.</p><p id="a9ad2836-a6e0-4dd9-b758-27e88306b67e" class="">
</p><figure id="7f5707b2-bbb7-4471-9903-058634b1236a" class="image"><a href="image%205.png"><img style="width:441px" src="image%205.png"/></a></figure><p id="35a4373c-4fc8-49c5-bc6a-9e4dbf7af07f" class="">
</p><ul id="d212fc1d-5e83-41b4-bed2-f577bec2b4a5" class="bulleted-list"><li style="list-style-type:disc"><strong>Preámbulo</strong>. Secuencia de valores alternados 1 y 0 usados para la sincronización y para detectar la presencia de señal, indica el inicio de la trama.</li></ul><ul id="e9eb4960-36a0-4262-adda-bc6810544a22" class="bulleted-list"><li style="list-style-type:disc"><strong>Dirección de destino</strong>. Este campo identifica la dirección MAC del dispositivo que debe recibir la trama. La dirección de destino puede especificar una dirección individual o una dirección multicast destinada a un grupo de estaciones.</li></ul><ul id="a1dda06e-6d58-4549-904c-1bbde6794f22" class="bulleted-list"><li style="list-style-type:disc"><strong>Dirección de origen</strong>. Este campo identifica la dirección MAC del dispositivo que debe enviar la trama.</li></ul><ul id="f6aedaaa-7e92-4679-8fe9-ea24898603b3" class="bulleted-list"><li style="list-style-type:disc"><strong>Tipo</strong>. Indica el tipo de protocolo de capa superior.</li></ul><ul id="90955b9b-0811-45ae-b0c0-16857035c5f8" class="bulleted-list"><li style="list-style-type:disc"><strong>Datos</strong>. Este campo contiene los datos transferidos desde el origen hasta el destino. El tamaño máximo de este campo es de 1500 bytes. Si el tamaño de este campo es menor de 46 bytes, entonces es necesario el uso del campo siguiente (Pad) para añadir bytes hasta que el tamaño de la trama alcance el valor mínimo.</li></ul><h2 id="88c3470e-365c-4152-9aa8-60b16d2411b3" class="">4.6 Proceso de encapsulación de los datos</h2><p id="925de0a2-b179-4400-909b-967bd4f9f2d3" class="">El proceso desde que los datos son incorporados al ordenador hasta que se transmiten al medio se llama encapsulación. Estos datos son formateados, segmentados, identificados con el direccionamiento lógico y físico para finalmente ser enviados al medio. A cada capa del modelo OSI le corresponde una PDU (Unidad de Datos) que se puede abreviar con el formato LxPDU, donde la x representa el número de la capa correspondiente.</p><p id="f80f6a09-298d-48f5-8b65-4e80866edeee" class="">Por ejemplo, para la capa de red la abreviatura correspondiente será L3PDU. Siguiendo por lo tanto el siguiente orden de encapsulamiento:</p><ol type="1" id="babe02ba-4337-4fb1-9f36-fb761b54b27e" class="numbered-list" start="1"><li><strong>Datos</strong>. Los datos son incorporados al ordenador por el usuario a través de una determinada aplicación. Los datos son formateados de tal manera que puedan ser leídos por la capa de aplicación de otro ordenador en el destino.</li></ol><ol type="1" id="4bddae34-8903-4ab1-a28f-19494823e7f0" class="numbered-list" start="2"><li><strong>Segmentos</strong>. Debido a que posiblemente la cantidad de los datos sea demasiada, la capa de transporte desde el origen se encarga de segmentarlos para así ser empaquetados debidamente, esta misma capa en el destino se encargará de reensamblar los datos y colocarlos en forma secuencial, ya que no siempre llegan a su destino en el orden en que han sido segmentados.</li></ol><ol type="1" id="a1644a58-8841-48d8-b577-31d9b80c9f16" class="numbered-list" start="3"><li><strong>Paquetes</strong>. Los segmentos son empaquetados en paquetes o datagramas e identificados en la capa de red con la dirección lógica o IP correspondiente al origen y destino.</li></ol><ol type="1" id="f7ee756d-7afa-4ff4-8065-9edb391a6b22" class="numbered-list" start="4"><li><strong>Tramas</strong>. En la capa de enlace de datos se añade una cabecera con la dirección MAC y el campo de comprobación de la trama formándose las tramas, o trames, para ser transmitidos a través de alguna interfaz.</li></ol><ol type="1" id="0a3ee22e-4ef1-45e5-bf69-42c0a9519039" class="numbered-list" start="5"><li><strong>Bits</strong>. Finalmente, las tramas son enviadas al medio desde la capa física, en forma de pulsos eléctricos, luz o radiofrecuencia.</li></ol><p id="b54cb680-3e4e-403d-8068-daac9b1783e5" class="">
</p><figure id="313fc357-36fb-441b-9712-3b6e3d40fbbf" class="image"><a href="image%206.png"><img style="width:336px" src="image%206.png"/></a></figure><p id="33b74313-fc23-4fbc-a88d-cc8a5683a98a" class="">                                   Relación entre capas del modelo OSI y su correspondiente PDU</p><p id="afd5446a-01f0-4aa0-8428-dbb201c0d489" class="">
</p><h3 id="fff4020f-bd2c-803c-991c-f0ea2b488395" class="">Secuencia de la encapsulación de datos:</h3><figure id="3fb0bd72-decf-4199-b4e4-219dc02a4acd" class="image"><a href="image%207.png"><img style="width:624px" src="image%207.png"/></a></figure><p id="14d084e9-8ac6-4def-892b-701426d41079" class="">
</p><figure class="block-color-gray_background callout" style="white-space:pre-wrap;display:flex" id="f49283d2-51fb-4e4a-8920-3451a15dd732"><div style="font-size:1.5em"><span class="icon">💡</span></div><div style="width:100%">El proceso inverso se realiza en el destino y se llama desencapsulación de datos.</div></figure><h2 id="fff4020f-bd2c-807e-a7f5-f331afb01f7e" class=""><mark class="highlight-purple">5. Modelo jerárquico</mark></h2><p id="3b526865-0fbb-4a52-a15d-1fbe0c123911" class="">Con el fin de simplificar el diseño, implementación y administración de las redes, Cisco utiliza un modelo jerárquico para describir la red. Aunque la práctica de este método suele estar asociada con el proceso de diseño de una red, es importante comprender el modelo para poder determinar el equipo y características que van a necesitar en la red. Un modelo jerárquico acelera la convergencia, mantiene posibles problemas aislados por capas y reduce la sobrecarga en los dispositivos.</p><p id="616eb8c8-6da4-4a40-a02d-2cd7fd5b3eea" class="">El modelo se compone de tres capas o niveles:</p><ul id="bb24dec4-563a-425a-9100-c0d924f4b150" class="bulleted-list"><li style="list-style-type:disc">Capa o nivel de acceso.</li></ul><ul id="d137093d-bb83-4781-b427-1395436e2552" class="bulleted-list"><li style="list-style-type:disc">Capa o nivel de distribución.</li></ul><ul id="464fa293-d48e-4153-9fd1-58b944f3ab61" class="bulleted-list"><li style="list-style-type:disc">Capa o nivel de núcleo.</li></ul><p id="b0975ba5-713a-48c5-a62c-3434150736c7" class="">
</p><figure id="58dbfab0-0898-4ed2-b64d-286c8af2523c" class="image"><a href="image%208.png"><img style="width:576px" src="image%208.png"/></a></figure><p id="09f6f0f5-2690-480d-b060-7a6b0f9db299" class="">
</p><h3 id="014ba287-ed2b-43de-8a7b-e768a484d967" class="">5.1 Capa de acceso</h3><p id="3893a72f-8c19-4c2d-b739-a8c4aac36ce2" class="">La capa de acceso de la red es el punto en el que cada usuario se conecta a la red. Esta es la razón por la cual la capa de acceso se denomina a veces capa de puesto de trabajo, capa de escritorio o de usuario. Los usuarios, así como los recursos a los que estos necesitan acceder con más frecuencia están disponibles a nivel local. El tráfico hacia y desde recursos locales está confinado entre los recursos, switches y usuarios finales. En muchas redes no es posible proporcionar a los usuarios un acceso local a todos los servicios, como archivos de bases de datos, almacenamiento centralizado o acceso telefónico a la Web. En estos casos, el tráfico de usuarios que demandan estos servicios se desvía a la siguiente capa del modelo: la capa de distribución.</p><p id="d9906690-e2ce-40ea-a774-04f4bf3efd31" class="">Algunas de las funciones de la capa de acceso son:</p><ul id="6e530217-0982-40fd-856d-ee66b98c2964" class="bulleted-list"><li style="list-style-type:disc">Interconexión de los diferentes grupos de trabajo hacia la capa de<br/>distribución.<br/></li></ul><ul id="a461362c-6e62-4d52-86b4-e1f0ef55ada9" class="bulleted-list"><li style="list-style-type:disc">Segmentación en múltiples dominios de colisión.</li></ul><ul id="90f5981b-08ae-4030-9a65-83abf58c025f" class="bulleted-list"><li style="list-style-type:disc">Brinda soporte a tecnologías como Ethernet y Wireless.</li></ul><ul id="319eee6a-4e9d-4066-9f64-90547f390249" class="bulleted-list"><li style="list-style-type:disc">Implementación de redes virtuales (VLAN).</li></ul><h3 id="557c09df-42d2-45c0-90eb-ca5d323c8874" class="">5.2 Capa de distribución</h3><p id="9c67e4e5-b99c-414a-ac83-e98b37ab1e8a" class="">La capa de distribución marca el punto medio entre la capa de acceso y los servicios principales de la red. La función primordial de esta capa es realizar funciones tales como enrutamiento, filtrado y acceso a WAN.</p><p id="91fa9aa8-3e28-4fa4-8111-d53095d239dd" class="">En un entorno de campus, la capa de distribución abarca una gran diversidad de funciones, entre las que figuran las siguientes:</p><ul id="a490343d-2765-4bc1-ac12-633c29923ccc" class="bulleted-list"><li style="list-style-type:disc">Servir como punto de concentración para acceder a los dispositivos de capa de acceso.</li></ul><ul id="e2c6e56b-d1bf-49a1-95b2-c63581449d09" class="bulleted-list"><li style="list-style-type:disc">Enrutar el tráfico para proporcionar acceso a los departamentos o grupos de trabajo y entre las diferentes VLAN.</li></ul><ul id="0f3a06b2-8d53-4c31-85ed-383eebb5c975" class="bulleted-list"><li style="list-style-type:disc">Segmentar la red en múltiples dominios de difusión/multidifusión.</li></ul><ul id="50429fb1-0dee-47dc-b306-61a7380831fd" class="bulleted-list"><li style="list-style-type:disc">Traducir los diálogos entre diferentes tipos de medios, como Token Ring y Ethernet.</li></ul><ul id="db121c7f-7de6-45ce-9918-7a853916d1dc" class="bulleted-list"><li style="list-style-type:disc">Proporcionar servicios de seguridad y filtrado.</li></ul><p id="ae108e51-9763-456f-b7e5-9ec0b9f380d9" class="">La capa de distribución puede resumirse como la capa que proporciona una conectividad basada en una determinada política, dado que determina cuándo y cómo los paquetes pueden acceder a los servicios principales de la red. La capa de distribución determina la forma más rápida para que la petición de un usuario (como un acceso al servidor de archivos) pueda ser remitida al servidor.</p><h3 id="c287537e-74c8-46c6-ab78-3b05a6c1fd84" class="">5.3 Capa de núcleo</h3><p id="94daa81a-013f-4eb5-970a-471bd8bd109d" class="">La capa del núcleo o core se encarga de desviar el tráfico lo más rápidamente posible hacia los servicios apropiados. Normalmente, el tráfico transportado se dirige o proviene de servicios comunes a todos los usuarios. Estos servicios se conocen como servicios globales o corporativos.</p><p id="a093acc5-7eec-4426-9063-b3794ea65da4" class="">Cuando un usuario necesita acceder a un servicio corporativo, la petición se procesa al nivel de la capa de distribución. El dispositivo de la capa de distribución envía la petición del usuario al núcleo. Este se limita a proporcionar un transporte rápido hasta el servicio corporativo solicitado. El dispositivo de la capa de distribución se encarga de proporcionar un acceso controlado a la capa de núcleo.</p><p id="bd55b667-eb74-4f96-8f0f-836cfe9892e2" class="">Para la capa de <strong>core </strong>se deben tomar en cuenta los siguientes conceptos:</p><ul id="a4b2aa63-c921-4356-8f5d-ada7f14ba433" class="bulleted-list"><li style="list-style-type:disc">Esta capa debe ser diseñada para una alta velocidad de transferencia y mínima latencia.</li></ul><ul id="834cc3b0-ed6b-43cf-a7fa-c1830ba87596" class="bulleted-list"><li style="list-style-type:disc">No se debe dar soporte a grupos de trabajo ni enrutamiento entre VLAN.</li></ul><ul id="565ecc63-dd91-4ad7-ac81-eb627d79d23b" class="bulleted-list"><li style="list-style-type:disc">El tráfico debe haber sido filtrado en la capa anterior.</li></ul><ul id="d7124db0-d128-4bf0-929b-04cc294cdcc9" class="bulleted-list"><li style="list-style-type:disc">Los protocolos de enrutamientos utilizados deben ser de rápida convergencia y redundantes.</li></ul><p id="b0fc2c4d-632f-4541-89dc-e1b5d063acc4" class="">
</p><figure id="5f827b5c-262b-4480-b8dc-3c6cc31c06a9" class="image"><a href="image%209.png"><img style="width:672px" src="image%209.png"/></a></figure><h1 id="ddcf5b78-1d2b-4035-9fd7-3a694c8a2b65" class=""><mark class="highlight-purple">6. Modelo de core colapsado</mark></h1><p id="705e6af9-1e5b-41a6-8401-d6b3e2b14ac8" class="">El diseño jerárquico de tres niveles maximiza el rendimiento, la disponibilidad de la red y la capacidad de escalar el diseño de la red. La principal motivación para el diseño de núcleo colapsado es la reducción de costos de la red, manteniendo al mismo tiempo la mayor parte de los beneficios del modelo jerárquico de tres niveles.</p><p id="10af14c3-33ed-479e-8639-c526ac62868e" class="">La implementación principal de un modelo colapsado reside en que las funciones de la capa de distribución y la capa de core están aplicadas en un solo dispositivo.<br/>El dispositivo de núcleo-distribución colapsado debe proporcionar lo siguiente:<br/></p><ul id="e79f0e46-c8fa-499f-b315-a56a38b08f9d" class="bulleted-list"><li style="list-style-type:disc">Rutas físicas y lógicas de alta velocidad de conexión a la red.</li></ul><ul id="7eb1f2d4-8b01-47eb-81a8-fa4ea7225dcf" class="bulleted-list"><li style="list-style-type:disc">Servir como punto de demarcación entre acceso y núcleo y de concentración de capa 2.</li></ul><ul id="a8812a40-b7b1-47e4-ae14-0b95a57ff140" class="bulleted-list"><li style="list-style-type:disc">Definir las políticas de acceso y de enrutamiento.</li></ul><ul id="c16af68c-e4c0-4112-a871-8b779a59baf6" class="bulleted-list"><li style="list-style-type:disc">Proveer calidad de servicio (QoS), virtualización de red, etc.</li></ul><p id="c669fa84-3422-4bd8-bd00-168056729595" class="">
</p><figure id="a68dad8f-87be-4bef-a711-165adeff4633" class="image"><a href="image%2010.png"><img style="width:480px" src="image%2010.png"/></a></figure><p id="5e26eaef-7a8b-48d4-95e5-c3f9ef968d70" class="">
</p><h1 id="7a2a7303-d729-43b3-96a7-1d281182ebb3" class=""><mark class="highlight-purple">7. Procedimientos básicos de troubleshooting</mark></h1><p id="c34fcc9d-d279-484f-88b8-d5ecfe3cc562" class="">Un buen procedimiento de troubleshooting estructurado ayuda a utilizar de manera más eficiente los recursos de una empresa, además, en caso de que un administrador deba continuar el trabajo de otro será más fácil de asumir.</p><p id="af879e3f-d911-474f-9e2c-1a08b70e2267" class="">Los siguientes pasos siguen un correcto mecanismo de troubleshooting estructurado:</p><ol type="1" id="f8f65782-8ce6-433b-a794-b48810b94af3" class="numbered-list" start="1"><li><strong>Informe del problema</strong>. Normalmente viene dado por alguien que hace uso de los recursos de la red y casi siempre será información poco precisa, e incluso errónea. El que alguien reporte un problema tiene que servir, sobre todo, para ser capaz de identificar qué parte de la red ha sido afectada, qué dispositivos, o qué grupo es responsable de la avería.</li></ol><ol type="1" id="cbcce27d-4021-4b31-b6af-329976365767" class="numbered-list" start="2"><li><strong>Recopilación de información</strong>. Una vez que el error ha sido reportado y se piensa haber identificado la parte de la red que tiene el problema, se ha de recopilar tanta información como sea posible, tanto de los dispositivos afectados, como logs, histórico de cambios realizados, etc.</li></ol><ol type="1" id="5431a292-21f5-4025-827c-282e10726d45" class="numbered-list" start="3"><li><strong>Examinar la información recopilada</strong>. Una vez recopilada toda la información necesaria se debe analizar exhaustivamente, estando siempre pendientes de:<ul id="d857584e-3d02-43b8-9396-88eb66e7bfa9" class="bulleted-list"><li style="list-style-type:disc">Identificar causas que apunten al problema raíz.</li></ul><ul id="0b27fa80-d86c-4a59-9ef9-7217565207d9" class="bulleted-list"><li style="list-style-type:disc">Eliminar información que sea innecesaria.</li></ul><p id="984f9314-5838-455b-8269-f790e416e154" class="">Dependiendo del grado de experiencia del administrador se deben efectuar seguidamente algunas preguntas que se contestarán de manera<br/>más o menos rápida.<br/></p><ul id="042da972-3930-4b17-9c93-d86d45da5df3" class="bulleted-list"><li style="list-style-type:disc">¿Qué es lo que está pasando en la red?</li></ul><ul id="5cc74605-12d2-40e5-b12a-b4f4b03fd02c" class="bulleted-list"><li style="list-style-type:disc">¿Qué debería estar pasando?, ¿cómo debería estar funcionando?</li></ul></li></ol><ol type="1" id="496565c1-a061-4639-9ef0-22edc8bc9ac5" class="numbered-list" start="4"><li><strong>Eliminar causas potenciales</strong>. Una vez examinados los datos se debe descartar la información relativa a causas que no sean propias del problema y, lo que es muy importante, no imaginar ni querer formular hipótesis basadas en datos que no están en la información recopilada.</li></ol><ol type="1" id="374f5499-306a-49df-8883-2f2fe4fd384c" class="numbered-list" start="5"><li><strong>Crear una hipótesis de la causa</strong>. Una vez eliminadas las causas potenciales, centrarse únicamente en la que se crea sea la definitiva. En caso de que se tenga acceso al dispositivo se procederá a intentar solucionar el problema. En caso de que no tener acceso al dispositivo<br/>se deberá buscar una solución alternativa a través del administrador de red correspondiente.<br/></li></ol><ol type="1" id="a89fbb69-e89b-4273-ac17-9e636dfe4acd" class="numbered-list" start="6"><li><strong>Verificación de la hipótesis</strong>. Una vez conocida la causa se puede intentar resolverla. Es importante pensar cómo actuar debido a que el hecho de implementar la solución inmediatamente puede provocar cortes en la red, entonces quizás sea mejor planificar la intervención para un momento más adecuado: por la noche o cuando el impacto sea mínimo.<p id="94a84794-5c0b-450f-bacc-614a9920e3e9" class="">Es de vital importancia documentar todos los cambios que se apliquen para que, en caso de que la solución pensada no resuelva el problema.</p></li></ol><ol type="1" id="9d9f0466-54b5-45de-b7ec-21c749627f45" class="numbered-list" start="7"><li><strong>Resolución del problema</strong>. Una vez resuelto el problema se debe dejar claramente documentado y todas las partes implicadas han de recibir una explicación de lo ocurrido y cómo se resolvió.</li></ol><h1 id="1e2186a2-73b5-471e-beb1-8e9a54199526" class=""><mark class="highlight-purple">8. Fundamentos para el examen</mark></h1><p id="cc6f9f65-4984-4265-9f67-2f9711a4c722" class="">Es fundamental entender el principio de la división en capas de una red, los modelos utilizados y los protocolos principales que resultan básicos y primordiales. Conocer el modelo OSI le ayudará a identificar problemas e incluso le ayudarán a determinar a qué departamento corresponde la solución de la incidencia.</p><ul id="fc1bbdaa-c2c6-4ceb-b89c-5ddfb7827519" class="bulleted-list"><li style="list-style-type:disc">Tenga una idea clara sobre las siete capas del modelo OSI, las funciones en la red para que se usan y los protocolos asociados a cada una.</li></ul><ul id="1a660bba-b99e-431f-a4a4-f79bbc40779d" class="bulleted-list"><li style="list-style-type:disc">Analice las diferencias entre los dispositivos de cada capa del modelo OSI, cuáles son sus funciones y para qué se aplican en cada caso.</li></ul><ul id="a6ebc74e-e560-43f3-a488-79d9d6006e05" class="bulleted-list"><li style="list-style-type:disc">Recuerde las posibles causas que pueden generar congestión en una LAN. Cómo, de ser posible, evitarlo.</li></ul><ul id="92bdb3ff-1b5f-4c02-bccc-16eb117a4c30" class="bulleted-list"><li style="list-style-type:disc">Tenga en cuenta las diferencias entre dominio de colisión y dominio de broadcast y los dispositivos asociados a cada uno.</li></ul><ul id="17ce72e3-02d9-46ac-b875-bbb7a5b0d312" class="bulleted-list"><li style="list-style-type:disc">Recuerde la diferencia entre orientado a conexión y no orientado a conexión y los protocolos a que hacen referencia.</li></ul><ul id="7ed28319-51fb-4513-a2bd-69d6df136a5f" class="bulleted-list"><li style="list-style-type:disc">Sepa diferenciar entre los tipos de cableado Ethernet y sus estándares, además de saber distinguir en cada caso cuál utilizar según los dispositivos a conectar.</li></ul><ul id="f744ca48-c88c-44ff-8fe2-a1d724ba0160" class="bulleted-list"><li style="list-style-type:disc">Tenga en cuenta las características, campos y tamaño de la trama Ethernet.</li></ul><ul id="7a02cc7d-84df-4bdf-acce-91ce10380b99" class="bulleted-list"><li style="list-style-type:disc">Recuerde las funciones de cada capa del modelo jerárquico de Cisco, para qué se aplican y los dispositivos asociados.</li></ul><ul id="bbfbe13c-d6f9-4569-ae25-ab93ad10ea14" class="bulleted-list"><li style="list-style-type:disc">Recuerde las cuatro capas del modelo TCP/IP, sus funciones y los protocolos asociados a cada una.</li></ul><ul id="ddf8b776-b4e7-4579-a8e9-46c050994776" class="bulleted-list"><li style="list-style-type:disc">Sepa cuáles son las diferencias entre el modelo TCP/IP y el modelo OSI. Analice y compare sus capas.</li></ul><ul id="636a9bd1-3b84-4ec2-8cb7-45c7be20472a" class="bulleted-list"><li style="list-style-type:disc">Tenga en cuenta las diferencias fundamentales entre TCP y UDP, control de flujo, ACK, ventanas y ventanas deslizantes.</li></ul><ul id="4f086976-ee50-4eab-a373-1284a292c089" class="bulleted-list"><li style="list-style-type:disc">Recuerde las diferencias entre el modelo de tres capas y el modelo de core colapsado.</li></ul><ul id="d89485a6-e78e-44af-a449-183093985afe" class="bulleted-list"><li style="list-style-type:disc">Analice y recuerde los pasos para un procedimiento de troubleshooting.</li></ul></div></article><span class="sans" style="font-size:14px;padding-top:2em"></span></body></html>
