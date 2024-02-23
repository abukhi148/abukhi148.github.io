# hugo-shortcode-sponsor-log

A Hugo theme component with `sponsor-log` shortcode.

## Installation

Clone this git repository into your theme folder and add it as a submodule of your website directory.

```bash
git submodule add https://github.com/Lruihao/hugo-shortcode-sponsor-log.git themes/shortcode-sponsor-log
```

Next edit `config.toml` of your project and add this theme component to your themes:

```bash
theme = ["your-main-theme", "shortcode-sponsor-log"]
```

To learn about theme components of hugo and how to use them, check out <https://gohugo.io/hugo-modules/theme-components/>.

## Usage

First, create the `sponsor_log.yml` file and edit your data:

```
cp themes/shortcode-sponsor-log/sponsor_log.yml.example data/sponsor_log.yml
```

Next, use the `sponsor-log` shortcode in any page:

```markdown
{{< sponsor-log >}}
```
