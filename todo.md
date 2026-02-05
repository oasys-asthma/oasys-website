# todo

- [x] help / documentation pages
- [x] link checker, css linter, html linter
- [ ] contact page. have started this, need to sort out the css to work with the html
- [ ] more styling
 - [ ]  check all of the documentation pages, a lot of them look pretty bad at the moment
- [ ] team page
- [ ] download / install page
- [ ] favicon
- [ ] do something with home page 
- [ ] privacy policy
- [ ] terms and conditions maybe
- [ ] link to app store in footer probably / or link to download page
- [ ] add an oasys linkedin page, and use the link
- [ ] Accesibility, put the axe tools on it
- [ ] Remove unused css
 - [ ] all the span stuff i think
 - [ ] ...
- [ ] create oasys organisation on github and put the repo there
- [ ] have some sort of ci, probably netlify
- [ ] deploy to netlify with a weird url and send round to people
- [ ] do new domain in azure if poss, and link to it

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
