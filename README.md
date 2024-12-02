# touying-flow

Discard irrelevant decorative elements, aiming to better immerse the audience into a state of flow.

Inspired by [Dewdrop](https://github.com/touying-typ/touying.git), made by [OrangeX4](https://github.com/OrangeX4)

A [Typst](https://github.com/typst/typst) template created based on [Touying](https://github.com/touying-typ/touying), designed for academic presentations in university settings.

## Example

See [content/example/main.pdf](content/example/main.pdf) for a sample PDF output. While the project is already complete, the example content is still under development.

## Installation

These steps assume that you already have [Typst](https://typst.app/) installed and running. If not, please refer to [github.com/typst/typst/releases/](https://github.com/typst/typst/releases/) for installation instructions.Alternatively, you can use VS Code for editing by installing the Tinymist Typst extension (*recommended*).

### Import from Typst Universe

```typst
// #import "@preview/touying-flow:1.0.1":*
#show: flow-theme.with(
  aspect-ratio: "16-9",
  footer: self => self.info.title,
  footer-alt: self => self.info.subtitle,
  navigation: "mini-slides",
  primary:rgb(0,108,57),//rgb("#006c39"),
  secondary:rgb(161,63,61),//rgb("#a13f3d"),
  // text-font: ("Libertinus Serif"),
  // text-size: 20pt,
  // code-font: ("Jetbrains Mono NL","PingFang SC"),
  // code-size: 16pt,

  config-info(
    title: [Title],
    subtitle: [Subtitle],
    author: [Quaternijkon],
    date: datetime.today(),
    institution: [USTC],
  ),
)

#title-slide()

= #smallcaps("Slide")

== New slide
```
