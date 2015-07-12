# jekyll-media

this is a set of jekyll includes for embedding media.

## usage

### include

    {% if post.media %}
      {% include media/media.html media=post.media %}
    {% endif %}

### yaml frontmatter

media embeds will show up in the order in which they're listed here

    media:
      -
        type: image
        url: "/images/pfe.jpg"
        title: "Photo by David R. Gammons"
      -
        type: bandcamp
        bandcamp-type: album
        id: 457390215
      -
        type: soundcloud
        soundcloud-type: track
        id: 214014828
      -
        type: vimeo
        id: 84020611
        16by9: true
      -
        type: images
        images:
          -
            alt: Collage 1
            url: /images/collage/1.jpg
          -
            alt: Collage 2
            url: /images/collage/2.jpg
          -
            alt: Collage 3
            url: /images/collage/3.jpg
