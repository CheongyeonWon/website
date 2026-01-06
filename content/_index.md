---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: skills
    content:
      title: Skills
      text: ''
      # Choose a user to display skills from (a folder name within `content/authors/`)
      username: admin
    design:
      columns: '1'
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Assistant Professor
          company: Soongsil University
          company_url: 'https://ensb.ssu.ac.kr/'
          company_logo: ''
          location: Seoul, South Korea
          date_start: '2024-09-01'
          date_end: ''
          description: Department of Entrepreneurship and Small Business
        - title: Research Associate
          company: KDI
          company_url: ''
          company_logo: KDI_Logo
          location: Sejong, South Korea
          date_start: '2014-10-21'
          date_end: '2020-02-10'
    design:
      columns: '1'
  - block: collection
    id: publications
    content:
      title: Publications
      #text: |-
      #  {{% callout note %}}
      #  Quickly discover relevant content by [filtering publications](./publication/).
      #  {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: ture 
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Cliometrics
          tag: Cliometrics
        - name: Labour and Industry
          tag: Labour and Industry
        - name: Others 
          tag: Others
    design:
      columns: '2'
      view: citation
  - block: portfolio
    id: projects
    content:
      title: Working Paper
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Cliometrics
          tag: Cliometrics
        - name: Labour and Industry
          tag: Labour and Industry
        - name: Others 
          tag: Others
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      view: citation
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
#  - block: tag_cloud
#    content:
#      title: Popular Topics
#    design:
#      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        E-mail.
      # Contact (add or remove contact options as necessary)
      email: clearlake@ssu.ac.kr
      address:
        street: 369 Sangdo-ro
        city: Dongjak-gu
        region: Seoul
        postcode: '06978'
        country: South Korea
        country_code: KR
     # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
#      office_hours:
#        - 'Monday 10:00 to 13:00'
#        - 'Wednesday 09:00 to 10:00'
#      # Choose a map provider in `params.yaml` to show a map from these coordinates
#     # coordinates:
#      #  latitude: '37.4275'
#      #  longitude: '-122.1697'  
#      contact_links:
#        - icon: twitter
#          icon_pack: fab
#          name: DM Me
#          link: 'https://twitter.com/Twitter'
#        - icon: skype
#          icon_pack: fab
#          name: Skype Me
#          link: 'skype:echo123?call'
#        - icon: video
#          icon_pack: fas
#          name: Zoom Me
#          link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: false
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
