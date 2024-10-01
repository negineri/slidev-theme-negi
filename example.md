---
theme: ./
colorSchema: light
selectable: true
---

# タイトル

サブタイトル

<div class="mt-auto">
  <div class="text-11px font-bold">
  所属
  </div>
  <div class="text-16px font-bold">
  氏名
  </div>
</div>

---
layout: section
---

# タイトル

## サブタイトル

---
layout: section
---

# タイトル<br>２行

## サブタイトル

---

# タイトル

## サブタイトル

- 箇条書き[^1]
- 箇条書き

[^1]: https://example.com

---

# Content with Image

## 画像サイズは固定

高さは固定のため必要に応じてCSSで調整をする

![/sample1.drawio.svg](/sample1.drawio.svg)

<style>
  img {
    @apply !h-86;
  }
</style>

---
layout: two-cols-header
---

# Tow cols header

## ２列にしたい場合

::left::

![/sample1.drawio.svg](/sample1.drawio.svg)

::right::

画像を使う場合はこちらを使った方が納まりが良い

- 主体となるコンテンツを左に配置する

---
layout: two-cols-header
---

# Tow cols header

## ２列にしたい場合

画像を2枚並べたりも出来る

::left::

![/sample1.drawio.svg](/sample1.drawio.svg)

::right::

![/sample2.drawio.svg](/sample2.drawio.svg)

<style>
  img{
    @apply !object-cover !h-84
  }
</style>

---
layout: two-cols-header
---

# Tow cols header

## ２列にしたい場合

::left::

### 画像の`height`の目安

- defaultで１行加える場合は `!h-86`
- tow-cols-headerで1行加える場合は `!h-84`
- 画像を広げる場合は`!object-cover`

::right::

![/sample1.drawio.svg](/sample1.drawio.svg)

---

# What is Slidev?

## Subtitle

Slidev is a slide maker and presentation tool designed for developers. It includes the following features:

- 📝 **Text-based** - focus on your content with Markdown, then style it later
- 🎨 **Themable** - themes can be shared and reused as npm packages
- 🧑‍💻 **Developer Friendly** - code highlighting, live coding with autocompletion
- 🤹 **Interactive** - embed Vue components to enhance your expressions
- 🎥 **Recording** - built-in recording and camera view
- 📤 **Portable** - export to PDF, PPTX, PNGs, or even a hostable SPA
- 🛠 **Hackable** - virtually anything that's possible on a webpage is possible in Slidev

<br>
<br>

Read more about [Why Slidev?](https://sli.dev/guide/why)

---

# Navigation

Hover on the bottom-left corner to see the navigation's controls panel

## Keyboard Shortcuts

|     |     |
| --- | --- |
| <kbd>space</kbd> / <kbd>tab</kbd> / <kbd>right</kbd> | next animation or slide |
| <kbd>left</kbd>  / <kbd>shift</kbd><kbd>space</kbd> | previous animation or slide |
| <kbd>up</kbd> | previous slide |
| <kbd>down</kbd> | next slide |

---
layout: image-right
image: https://cover.sli.dev
---

# Code

Use code snippets and get the highlighting directly!

```ts
interface User {
  id: number
  firstName: string
  lastName: string
  role: string
}

function updateUser(id: number, update: Partial<User>) {
  const user = getUser(id)
  const newUser = { ...user, ...update }
  saveUser(id, newUser)
}
```

---
layout: center
class: "text-center"
---

# Learn More

[Documentation](https://sli.dev) / [GitHub Repo](https://github.com/slidevjs/slidev)

---
layout: end
---
