---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth: "header-webconf.jpg"
widget1:
  title: "User Resources"
  url: 'https://tenet-rccpii.github.io/TENET-VideoConferencing/users'
  image: users.jpg
  text: 'Want to try Vidyo for your next online meeting or presentation? Trying to connect but getting stuck? The team at TENET is working hard to develop resources that will answer all your questions. Learn more here...'
widget2:
  title: "Administrator Resources"
  url: 'https://tenet-rccpii.github.io/TENET-VideoConferencing/admins'
  image: admins.jpg
  text: 'TENET is working with video conferencing professionals around the world, to help administrators at institutions provide better support to end users. Please read more here...'
widget3:
  title: "News & Updates"
  url: 'https://tenet-rccpii.github.io/TENET-VideoConferencing/blog'
  image: news.jpg
  text: 'We are building a vibrant community of video conferencing administrators, users, and support staff across South Africa. Learn about training opportunities, new resources, and updates. We also want to hear from you about your Vidyo experience. Read our blog.'
#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
callforaction:
  url: https://tenet-rccpii.github.io/TENET-VideoConferencing/institutions
  text: Find out if your institution offers Vidyo ›
  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---

<div id="videoModal" class="reveal-modal large" data-reveal="">
  <div class="flex-video widescreen vimeo" style="display: block;">
    <iframe width="1280" height="720" src="https://www.youtube.com/embed/3b5zCFSmVvU" frameborder="0" allowfullscreen></iframe>
  </div>
  <a class="close-reveal-modal">&#215;</a>
</div>
