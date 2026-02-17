# todo

pics
- fix inline images
Homepage
- [ ] do something with home page 
 - [ ] add links to the cards on the home page
Header
- [ ] add links to download, team, and references
- [ ] ?Match baseline of Oasys h1 in header and nav links
- [ ] references
- [ ] download / install page. link to microsoft store
Footer
- [?] privacy policy
- [?] terms and conditions maybe
References page
 - [ ] add some details about the oasys references, probably a shortcode for a reference makes sense.
  - https://www.occupationalasthma.com/oasysreferences.aspx
Team page
  - [ ] get images from people and add these
Misc
- [ ] have some sort of ci, probably netlify
- [ ] deploy to netlify with a weird url and send round to people

- [ ] do new domain in azure if poss, and link to it
- [ ] maybe add shortcodes for FEV1 or something to subscript the 1. not sure if thats how it looks though
- [ ] Accesibility, put the axe tools on it
- [ ] new image for oasys_audit_center_report_2011.jpg. Probably ask sam or vicky
- [ ] Remove unused css
 - [ ] all the span stuff i think
 - [ ] ...

## Reference

Quite a good colour finding thing
https://coolors.co/b93c3c

browserling can be used to work out oldest supported version

stats for which browsers are used
https://www.statista.com/statistics/268299/most-popular-internet-browsers/


## every layout

https://api.every-layout.dev/view?email=ceddlyburge@gmail.com

## Another plan for menu items

```
        <!-- Could do something like this instead to read a list of menus from the config. not sure i need it.
        {{ range .Site.Menus.main }}
        <a class="nav-link" href="{{ .URL }}">
        {{ if .Pre }}
        {{ $icon := printf "<i data-feather=\"%s\"></i> " .Pre | safeHTML }}
        {{ $icon }}
        {{ end }}
        {{ $text := print .Name | safeHTML }}
        {{ $text }}
        </a>

        It needs something like this in config.toml

[menu]
  [[menu.main]]
    name = "Home"
    pre = "home"
    url = "/"
    weight = 1
  [[menu.main]]
    name = "Posts"
    pre = "pen-tool"
    url = "/posts/"
    weight = 2
  [[menu.main]]
    name = "Tags"
    pre = "tag"
    url = "/tags/"
    weight = 3
        {{ end }}
```

## robots.txt

https://gohugo.io/templates/robots/
https://www.ditig.com/robots-txt-template

Can use this to test
https://en.ryte.com/free-tools/robots-txt

Lighthouse wrongly states that search engines are not allowed to crawl the site
