+++
draft = false
title = '{{ replace .File.ContentBaseName "-" " " | title }}'
link = ""
image = ""
type = "" {{add subfolder name}}
category = [] {{add subnav tag name}}
tags = [] {{add tags for: "sub category" , "artist", "secondary category" , "material/ingredient" , "3d" , "multimedia" }}
+++

<!--
    The <category> must match what is in the navigation.md. They should also be single word, lowercase. 
    Include tags for singular materials to enable search by material. They should also be single word, lowercase.
     ***The <category> supercedes the tags and will prevent them from showing up in the quick filter even if they share mediums.
     ***The search bar supercedes all categories and subnav buttons to allow search by 'ingredient'. At this level, categories will be treated as tags. Items should also be tagged by a secondary category if any apply.

    Example:
        Activity: Jean/hans Arp
        Category: Painting
        Sub category: watercolor
        Component materials: pencil, crayon, markers
        Misc. tags: multimedia, paint, drawing
      
        * This activity will show up when clicking the <painting> category, then the <watercolor> subnav. 
        * When switched back to all, it will also show up with all items with singular tag "pencil", "painting" and secondary category tags "drawing", "multimedia" using the search bar

    Exceptions include:
        *If the tag is meant to link it to a subnav button
        *If the tag containts a <name> that is not found in the title

    SPECIFIC TAGGING CONVENTIONS AND SPECIAL TAGS:
        * 1day -> single day projects
        * Xday -> multi-day projects
        * acrylictempera -> for subnav under <painting>
        * pencilcrayon -> for subnav under <drawing>
        * multimedia -> for subnav under <tactile>
        * teambased -> for subnav under <outdoors>
        * artist -> artist based activities
        * 3d -> for relevant projects with raised surfaces
        * <medium> -> enables search in <All> regardless of category or subnav
            - tags: paint, acrylic, watercolor, pencils, crayons, clay
        * <material/ingredient> -> enables search in <All> by single component
            - tags: paper, foil, cardboard, etc.
-->