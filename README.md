# imqiuyezhang.github.io

My personal site: research, dance and writing. It is built by GitHub Pages
with Jekyll, so there is nothing to install. Push to `main` and the live site
updates a minute or two later.

## Write a new post

1. Add a file to `_posts/` named `YYYY-MM-DD-a-short-title.md`.
2. Start it with this block, then write underneath in plain text:

   ```
   ---
   layout: post
   title: The title of the post
   date: 2026-11-21 21:00
   tags: [reflection]
   ---

   First paragraph.

   Second paragraph.
   ```

3. Commit and push. The post appears on the home page and the Writing page.

A post dated in the future stays hidden until that date. For a post in
Chinese, add the line `lang: zh` to the block at the top.

## Add photos to a post

Resize each photo to about 1600 pixels on its long edge first (Preview: Tools,
Adjust Size), save it as a JPEG in `assets/img/posts/`, then use one of these:

```
A full-width photo:
![Describe the photo here]({{ '/assets/img/posts/my-photo.jpg' | relative_url }})

A smaller photo beside the paragraph that follows it:
![Describe the photo here]({{ '/assets/img/posts/my-photo.jpg' | relative_url }}){: .right}
The paragraph starts on the next line.
```

## Change the other pages

| To change | Edit |
| --- | --- |
| Home page text and portrait | `index.html` |
| Research projects, posters, training, education, publications | `_data/research.yml` |
| Dance photos | `_data/gallery.yml` and `assets/img/dance/` |
| Favourite places to dance, run and swim | `_data/places.yml` |
| Dance page text and the swimming video | `dance.html` |
| The introduction on the Writing page | `writing.html` |
| CV | replace `assets/Qiuye_Zhang_CV.pdf`, keeping the same file name |
| Colours and fonts | the first block of `assets/css/main.css` |
| Email, site title and description | `_config.yml` |

## The `_originals` folder

Full-size photos, the original video and the old site's files live in
`_originals/` on this computer. Git ignores that folder, so it is never
uploaded or published.
