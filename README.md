# Introduction

안녕하세요 !
저는 비트캠프에서 네이버 클라우드 AIaaS개발자 양성과정을 수강중인 차민주 라고 합니다.

이 페이지는 수강 과정 중의 저의 과제와 기록이 남겨질 예정입니다.




## Markdown

### Markdown이란?

Markdown은 일반 텍스트 문서의 양식을 편집하는 문법이다. README 파일이나 온라인 문서, 혹은 일반 텍스트 편집기로 문서 양식을 편집할 때 쓰인다. Markdown을 이용해 작성된 문서는 HTML등 다른 문서 형태로 쉽게 변환이 가능하다.


### Markdown을 작성하는 방법




### Configuration variables




```

For further customization of the sidebar, go to [sidebar.html](https://github.com/BDHU/minimalist/blob/main/_includes/sidebar.html) in this repo and modify it however you like. The [link-mobile.html](https://github.com/BDHU/minimalist/blob/main/_includes/links-mobile.html) customizes the sidebar's look on mobile devices. This example uses fonts from [font awesome](https://fontawesome.com) and [Iconify](https://iconify.design/). Feel free to explore/find other sources.

### Stylesheet

If you'd like to add your own custom styles:

1. Create a file called `/assets/css/style.scss` in your site
2. Add the following content to the top of the file, exactly as shown:

    ```scss
    ---
    ---

    @import "{{ site.theme }}";
    ```

3. Add any custom CSS (or Sass, including imports) you'd like immediately after the `@import` line

*Note: If you'd like to change the theme's Sass variables, you must set new values before the `@import` line in your stylesheet.*

### Layouts

If you'd like to change the theme's HTML layout:

1. For some changes such as a custom `favicon`, you can add custom files in your local `_includes` folder. The files [provided with the theme](https://github.com/BDHU/minimalist/tree/master/_includes) provide a starting point and are included by the [original layout template](https://github.com/BDHU/minimalist/blob/master/_layouts/default.html).
2. For more extensive changes, [copy the original template](https://github.com/BDHU/minimalist/blob/master/_layouts/default.html) from the theme's repository<br/>(*Pro-tip: click "raw" to make copying easier*)
3. Create a file called `/_layouts/default.html` in your site
4. Paste the default layout content copied in the first step
5. Customize the layout as you'd like

For example, this [repository](https://github.com/BDHU/bdhu.github.io) shows how customizations are made on the original theme.

### Customizing Google Analytics code

Google has released several iterations to their Google Analytics code over the years since this theme was first created. If you would like to take advantage of the latest code, paste it into `_includes/head-custom-google-analytics.html` in your Jekyll site.

## Previewing the theme locally

If you'd like to preview the theme locally (for example, in the process of proposing a change):

1. Clone down the theme's repository (`git clone https://github.com/BDHU/minimalist`)
2. `cd` into the theme's directory
3. Run `script/bootstrap` to install the necessary dependencies
4. Run `bundle exec jekyll serve` to start the preview server
5. Visit [`localhost:4000`](http://localhost:4000) in your browser to preview the theme

## Running tests

The theme contains a minimal test suite, to ensure a site with the theme would build successfully. To run the tests, simply run `script/cibuild`. You'll need to run `script/bootstrap` once before the test script will work.

## Contributors

Special thanks to [@godalming123](https://github.com/godalming123) for adding dark mode support. Also thank [@solvaholic](https://github.com/solvaholic), [@tildehacker](https://github.com/tildehacker), and other contributors for making multiple bug fixes and improvements. All contributions are welcome.
