# ThopBlog - Creating New Posts & Using Images

## Creating a New Post
1. Navigate to your Hugo project directory.
2. Run the following command to create a new post:

```bash
hugo new posts/your-post-title.md
```

3. Open the newly created `.md` file inside `content/posts/`.
4. Add your content inside the file and modify the front matter as needed. For example:

```markdown
---
title: "My Awesome Post"
date: {{< now >}}
description: "A brief description of the post."
image: "https://postimages.com/example-image.jpg"
tags: ["web development", "hugo"]
---
```

## Adding Images
### Using PostImage for Free Hosting
1. Upload your image to [PostImage](https://postimages.org/).
2. Copy the **Direct Link** URL.
3. Insert the image in your post like this:

```markdown
![Image Description](https://postimages.com/example-image.jpg)
```

### Adding a Featured Image
In the front matter of your post, add:

```markdown
image: "https://postimages.com/example-image.jpg"
```

This will display the image as the featured post image on the homepage.



