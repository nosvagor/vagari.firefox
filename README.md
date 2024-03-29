<!-- ☄️  Heading {{{ -->
<h1 align="center">
   ☄️ vagari.firefox 🦊
</h1>

<p align="center">
<a href="https://github.com/nosvagor/vagari.firefox/discussions">
    <img
        src="https://img.shields.io/github/discussions/nosvagor/vagari.firefox?color=7492ef&logo=github&labelColor=222536&logoColor=7492ef&style=for-the-badge"
        title="alright then, keep your secrets"
    >
</a>
&nbsp;
<a href="https://github.com/nosvagor/vagari.firefox/network/members">
    <img
        src="https://img.shields.io/github/forks/nosvagor/vagari.firefox?color=a188df&logo=git&labelColor=222536&logoColor=a188df&style=for-the-badge"
        title="I am tormented with an everlasting itch for things remote. I love to sail forbidden seas..."
    >
</a>
&nbsp;
<a href="https://github.com/nosvagor/vagari.firefox/contributors">
    <img
        src="https://img.shields.io/github/contributors/nosvagor/vagari.firefox?color=85ba6d&logo=gitea&labelColor=222536&logoColor=85ba6d&style=for-the-badge"
        title="gotta do the cooking by the book"
    >
</a>
&nbsp;
<a href="https://github.com/nosvagor/vagari.firefox/issues">
    <img
        src="https://img.shields.io/github/issues/nosvagor/vagari.firefox?color=f2a170&logo=fireship&labelColor=222536&logoColor=f2a170&style=for-the-badge"
        title="this is not fine!!"
    >
</a>
</p>

<hr>
<blockquote>
    <img src="https://img.shields.io/static/v1?color=aeb9f8&logo=firefox&labelColor=222536&logoColor=aeb9f8&style=flat&message=βeta (0.1)&label=vagari.firefox"><br>
    &emsp;&emsp;&rarr; a port of the <a href="https://github.com/nosvagor/vagari"><i>vagari</i></a> color
    scheme / design framework for firefox custom css.
</blockquote>
<hr>
<!-- }}} --->

<br>

## Video showcase

with commentary:

[with commentary](https://user-images.githubusercontent.com/59071534/231578016-8804afa3-1abc-4597-87fa-dc8442fd3af3.mp4)

<br>

no audio: 

[no commentary](https://user-images.githubusercontent.com/59071534/230798554-90d9cbff-9594-4f7b-84d3-99e614165211.webm)

<br>
<br>

## 🧭 Design Direction

At this time, the goal is to create a sleek keyboard-centric
interface. Many clickable elements are purposely removed in order force
adoption of keyboard shortcuts, rather than relying on the mouse.

Anything not culled is mostly just basic themeing... colors, transitions, sizing, and such.

Eventually, a GTK port of vagari will be made, which will prompt a refactor in
order priortize GTK settings, only falling backt to legacy toolkit when
necessary. For that reason, much of the css is hardcoded, obtuse, and probably
could be done in a much better way.

Frankly put, I have little need for most of the UI elements I just want it to
match my theme for the time being.

> Additionally, long ago I copied the work from this [Moonlight userChrome](https://github.com/eduardhojbota/moonlight-userChrome) theme.
>
> Definitely check it out, as it might be easier to modify than mine, as
> I haved disable/hidden many elements. I don't think it's been maintained
> though, so keep that in mind.

Also, check out [/r/FirefoxCSS](https://www.reddit.com/r/FirefoxCSS/) for more guideance/ideas!

**Note:** updates often break stylesheets. Stay vigilant!

<br>

## 🧰 Installation

<ol>
    <li><strong>Find Profile Directory &darr;</strong></li>
<ul>
    <li>In the URL bar type: <code>about:profiles</code> </li>
    <li>Under <strong>Default Proile</strong>, locate <strong>Root Directory</strong> </li>
    <li>Click <strong>Open Directory</strong></li>
    <li>E.g., on linux, <code>~/.mozilla/firefox/{some unique identifier here}.default</code></li>
</ul>
<br>
    <li><strong>Clone repository into the <em>Chrome</em> directory</strong></li>

```sh
# in the directory mentioed above
mkdir chrome && cd chrome
dir=$(pwd)

# clone repo in your preferred locatation
git clone https://github.com/nosvagor/vagari.firefox.git
ln -sfn path/to/vagari.firefox/css/* $dir
```
> One could simply extract contents from repo into said chrome directory under
> firefox profile, but linking the files symbolically allows one to easily
> track updates.

  <br>
  <li><strong>Make sure legacy toolkit is enabled</strong></li>
  <ul>
    <li>In the URL bar type: <code>about:config</code> </li>
    <li><code>toolkit.legacyUserProfileCustomizations.stylesheets = true</code></li>
    <li>Restart the browser</li>
  </ul>
  <br>
  <li><strong>(Optional) Enable live debug</strong></li>
  <ul>
      <li>Open developer window (F12)</li>
      <li>Go to Settings (F1)</li>
      <li>Under Advance settings:</li>
      <ul>
          <li>Enable browser chrome and add-on debugging toolboxes</li>
          <li>Enable remote debugging</li>
      </ul>
      <li>Restart the browser</li>
      <li>Adjust style on the fly using Ctrl + Alt + Shift + I</li>
      <li>Custom settings can be edited and in these two files under the <strong>style editor</strong> tab:</li>
      <ul>
          <li>userChrome.css</li>
          <li>userContent.css</li>
      </ul>
      <li>Additional custom files are denoted with a preceding udnerscore
      (e.g., _tab-bar.css). This is for organizational reasons; they are simply
      imported into userChrome.css. Feel free to edit, create, ignore, or reorganize
      these to your liking. Pull requests are welcome.</li>
  </ul>
</ol>

<br>

**bonus preview** _(whole desktop)_ **⚠ loud ⚠️**:

https://user-images.githubusercontent.com/59071534/231580855-9419fc55-9913-4319-8864-2c3b3a99c2e4.mp4

<br> 

<p align="center">
    <a href="https://github.com/nosvagor/vagari.firefox/stargazers">
        <img
            src="https://img.shields.io/github/stars/nosvagor/vagari.firefox?color=ecc45d&logo=apachespark&labelColor=24283b&logoColor=ecc45d&style=for-the-badge"
            title="what is love, baby don't hurt me"
        >
    </a>
    &nbsp;
    <!-- <a href="https://cullyn.eth/"> -->
    <!--     <img -->
    <!--         src="https://img.shields.io/github/sponsors/nosvagor?color=dc60bf&logo=githubsponsors&labelColor=24283b&logoColor=dc60bf&style=for-the-badge" -->
    <!--         title="github sponsors not set up, pref ETH to cullyn.eth for now" -->
    <!--     > -->
    <!-- </a> -->
</p>
