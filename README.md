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

[output.webm](https://user-images.githubusercontent.com/59071534/230798554-90d9cbff-9594-4f7b-84d3-99e614165211.webm)

<br>

## 🧭 Design Direction

At this time, the goal is to create a sleek keyboard-centric
interface. Many clickable elements are purposely removed in order force
adoption of keyboard shortcuts, rather than relying on the mouse.

Anything not culled is mostly just basic themeing... colors, transitions, sizing, and such.

Eventually, a GTK port of vagari will be made, which will prompt a refactor in order priortize GTK settings.

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
