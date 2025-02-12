{
  "menus": "main",
  "title": "Home",
  "date": "2025-02-12T16:17:40-06:00",
  "paige": {
    "site": {
      "disable_menu": true
    },
    "pages": {
      "disable_title": true,
      "disable_collections": true,
      "disable_pages": true,
      "disable_sections": true
    }
  }
}

Absolute path (without processing renders fine):

{{< paige/gallery align="start" >}}
{{< paige/image src="/img/logo_notext.png" maxheight="10rem" loading="lazy" >}}
{{< /paige/gallery >}}

Absolute url (with processing renders fine):

{{< paige/gallery align="start" >}}
{{< paige/image breakpoints=true linked="unprocessed" src="https://images.unsplash.com/photo-1490604001847-b712b0c2f967?w=1296" maxheight="10rem" loading="lazy" >}}
{{< /paige/gallery >}}

Absolute path (causes failure to render):

{{< paige/gallery align="start" >}}
{{< paige/image breakpoints=true linked="unprocessed" src="/img/logo_notext.png" maxheight="10rem" loading="lazy" >}}
{{< /paige/gallery >}}
