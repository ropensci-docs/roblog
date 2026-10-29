# Check your post

Functions to be run on the path to your blog post (rendered, not the
Rmd).

## Best practice

[`ro_lint_md()`](https://docs.ropensci.org/roblog/reference/ro_lint_md.md)
should identify some potential problems and enforce:

- the use of (possibly empty) alternative descriptions for image;

- the use of Title Case for the title;

- the use of Sentence case for other headings;

- the absence of “click here” as text for links;

- the proper case (lowerCamelCase) for rOpenSci name;

- the use of Hugo shortcodes for figures;

- the use of relative links for links to rOpenSci website.

You need to run `render_one` on the path to the Markdown file. Some
Markdown examples and the corresponding messages below.

------------------------------------------------------------------------

/github/home/R/x86_64-pc-linux-gnu-library/4.6/roblog/examples/absolute-links.md

``` markdown

---
slug: "post-template"
title: Wonderful title
package_version: 0.1.0
authors:
  - Author Name
date: 2019-06-04
categories: blog
topicid:
tags:
  - Software Peer Review
  - R
  - community
# delete the line below
# if you have no preferred image
socialImg: img/blog-images/2019-06-04-post-template/name-of-image.png
---

 [rOpenSci blog](https://ropensci.org/blog)
```

  

------------------------------------------------------------------------

/github/home/R/x86_64-pc-linux-gnu-library/4.6/roblog/examples/allgood.md

``` markdown

---
slug: "post-template"
title: Wonderful Title
package_version: 0.1.0
authors:
  - Author Name
date: 2019-06-04
categories: blog
topicid:
tags:
  - Software Peer Review
  - R
  - community
# delete the line below
# if you have no preferred image
socialImg: img/blog-images/2019-06-04-post-template/name-of-image.png
---

Save this file under /content/blog/YEAR-MONTH-DAY-slug.md in the local copy of your roweb2 fork.
{{< figure src="orange-mug-near-macbook-3219546.jpg" width="300" link="https://www.pexels.com/photo/orange-mug-near-macbook-3219546/" alt="Laptop keyboard with a tree leaf beside it" class="center" caption="Another type of leaf. [Engin Akyurt on Pexels](https://www.pexels.com/photo/orange-mug-near-macbook-3219546/)." >}}
s
{{< figure src="orange-mug-near-macbook-3219546.jpg" width="300" link="https://www.pexels.com/photo/orange-mug-near-macbook-3219546/" alt="Laptop keyboard with a tree leaf beside it" >}}
### Heading in sentence case

#### Another sentence as heading
```

  

------------------------------------------------------------------------

/github/home/R/x86_64-pc-linux-gnu-library/4.6/roblog/examples/bad-no-alt.md

``` markdown

---
slug: "post-template"
title: Wonderful title
package_version: 0.1.0
authors:
  - Author Name
date: 2019-06-04
categories: blog
topicid:
tags:
  - Software Peer Review
  - R
  - community
# delete the line below
# if you have no preferred image
socialImg: img/blog-images/2019-06-04-post-template/name-of-image.png
---

Save this file under /content/blog/YEAR-MONTH-DAY-slug.md in the local copy of your roweb2 fork.

[Cool blog](/blog/)

[http](http://masalmon.eu/)

[Broken blog](https://masalmon.eu/40004)

[Broken blog again](https://masalmon.eu/400040)

Beware! If you want to generate this post from R Markdown, use the R Markdown template instead!

  Everywhere in this template (YAML, paths to images), you should change "post-template" to the slug of your post, and "2019-06-04" to the publication date.

Introduction including outline of the post.

### First awesome section

I like Hugo[^1]. Yes, that is how you add a footnote.

#### First awesome subsection of the first awesome section

Here's how to use a Hugo shortcode to add an image.

{{< figure src = "/img/blog-images/2019-06-04-post-template/name-of-image.png" width = "200">}}

{{< figure src = "/img/blog-images/2019-06-04-post-template/name-of-image.png" width = "200" alt = "too short">}}
```

  

------------------------------------------------------------------------

/github/home/R/x86_64-pc-linux-gnu-library/4.6/roblog/examples/clickhereissue.md

``` markdown

---
slug: "post-template"
title: Wonderful Title
package_version: 0.1.0
authors:
  - Author Name
date: 2019-06-04
categories: blog
topicid:
tags:
  - Software Peer Review
  - R
  - community
# delete the line below
# if you have no preferred image
socialImg: img/blog-images/2019-06-04-post-template/name-of-image.png
---

Save this file under /content/blog/YEAR-MONTH-DAY-slug.md in the local copy of your roweb2 fork.

### Heading in sentence case

#### Another sentence as heading

[Good link](https://ropensci.org), [Click here](https://ropensci.org), [here](https://ropensci.org).
```

  

------------------------------------------------------------------------

/github/home/R/x86_64-pc-linux-gnu-library/4.6/roblog/examples/code-no-functions.md

``` markdown

---
slug: "post-template"
title: Wonderful title
package_version: 0.1.0
authors:
  - Author Name
date: 2019-06-04
categories: blog
topicid:
tags:
  - Software Peer Review
  - R
  - community
# delete the line below
# if you have no preferred image
socialImg: img/blog-images/2019-06-04-post-template/name-of-image.png
---

```r
1

</details>
<br>


----

<details closed>
<summary> <span title='Click to Expand'> /github/home/R/x86_64-pc-linux-gnu-library/4.6/roblog/examples/figureissue.md </span> </summary>

```Markdown

---
slug: "post-template"
title: Wonderful Title
package_version: 0.1.0
authors:
  - Author Name
date: 2019-06-04
categories: blog
topicid:
tags:
  - Software Peer Review
  - R
  - community
# delete the line below
# if you have no preferred image
socialImg: img/blog-images/2019-06-04-post-template/name-of-image.png
---

Save this file under /content/blog/YEAR-MONTH-DAY-slug.md in the local copy of your roweb2 fork.

### Heading in sentence case

#### Another sentence as heading

![altbabla](imagepath/on/laptop.png)
```

  

------------------------------------------------------------------------

/github/home/R/x86_64-pc-linux-gnu-library/4.6/roblog/examples/links.md

``` markdown

---
slug: "post-template"
title: Wonderful title
package_version: 0.1.0
authors:
  - Author Name
date: 2019-06-04
categories: blog
topicid:
tags:
  - Software Peer Review
  - R
  - community
# delete the line below
# if you have no preferred image
socialImg: img/blog-images/2019-06-04-post-template/name-of-image.png
---

Save this file under /content/blog/YEAR-MONTH-DAY-slug.md in the local copy of your roweb2 fork.

[Cool blog](/blog/)

[bad](http://localhost:1313/blog)

[http](http://masalmon.eu/)

[Broken blog](https://masalmon.eu/40004)

[Broken blog again](https://masalmon.eu/400040)

[Broken local link](/4000004/)

[Missing slash](blog)

[Bad email link](maelle@ropensci.org)

[Good email link](mailto:yabellini@ropensci.org)
```

  

------------------------------------------------------------------------

/github/home/R/x86_64-pc-linux-gnu-library/4.6/roblog/examples/multi-bad.md

``` markdown

---
slug: "post-template"
title: Wonderful title
package_version: 0.1.0
authors:
  - Author Name
date: 2019-06-04
categories: blog
topicid:
tags:
  - Software Peer Review
  - R
  - community
# delete the line below
# if you have no preferred image
socialImg: img/blog-images/2019-06-04-post-template/name-of-image.png
---

 [rOpenSci blog](https://ropensci.org/blog)

#### First awesome subsection of the first awesome section

Here's how to use a Hugo shortcode to add an image.

{{< figure src = "/img/blog-images/2019-06-04-post-template/name-of-image.png" width = "200">}}

{{< figure src = "/img/blog-images/2019-06-04-post-template/name-of-image.png" width = "200" alt = "too short">}}
```

  

------------------------------------------------------------------------

/github/home/R/x86_64-pc-linux-gnu-library/4.6/roblog/examples/require.md

``` markdown

---
slug: "post-template"
title: Wonderful title
package_version: 0.1.0
authors:
  - Author Name
date: 2019-06-04
categories: blog
topicid:
tags:
  - Software Peer Review
  - R
  - community
# delete the line below
# if you have no preferred image
socialImg: img/blog-images/2019-06-04-post-template/name-of-image.png
---

```r
require(blop)
```

``` md
require(bla)
require(lala)

</details>
<br>

## URL validity

`ro_check_urls()` will identify possibly broken URLs.



``` r
path1 <- system.file(file.path("examples", "bad-no-alt.md"), package = "roblog")

roblog::ro_check_urls(path1)
#>  [31m• [39m Possibly broken URLs: https://masalmon.eu/40004, https://masalmon.eu/400040.
#>  [31m• [39m Replace http with https for: http://masalmon.eu/.
```
