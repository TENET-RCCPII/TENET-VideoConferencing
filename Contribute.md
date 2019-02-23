# Contributing

When contributing to this repository, please first discuss 
the change you wish to make via [issue](https://github.com/TENET-RCCPII/TENET-VideoConferencing/issues),
email, or any other method with the owners of this 
repository before making a change. 

Please note we have a [code of conduct](CodeConduct.md),
 please follow it in all your interactions with the project.
 
Also note that you will not be able to change the website directly, so will have to make a copy of the repository and make changes in the copy. Once you are happy with your changes you can create a [`Pull Request`](https://help.github.com/en/articles/about-pull-requests) which will notify the project owner of your suggestions and will allow them to add it to the website.
 
## Creating a Github Account

- To contribute to this website, you will need to sign up for a free Github account.
- Please visit the [Github website](https://github.com/) and follow the instructions for creating an account
- Remember to confirm your email address by clicking on the link that will be sent to the address that was used to create the Github account.

## Making a Copy of the Repository to Contribute Content

- Log into your Github account.
- Navigate to the [TENET-VideoConferencing repository](https://github.com/TENET-RCCPII/TENET-VideoConferencing/) on Github.
- To make a copy of this repository, click on `Fork` in the top right corner. This will create a copy of the repository under your username.
- Once the copying process is finished follow these steps under your username's copy of the website repository.
- Make sure you are on the `gh-pages` branch. Learn more 
   [about branches here](https://help.github.com/en/articles/viewing-branches-in-your-repository).

## Creating an Issue

1. Visit the [Github website](https://guides.github.com/features/issues/)
 to learn more about issues if you are new to this.
2. Go to the [issues tab in the Github repository](https://github.com/TENET-RCCPII/TENET-VideoConferencing/issues).
3. Look through existing issues to see if your question, concern, or suggestion
has already been raised.
4. If your question, suggestion, or concern is new, create a new issue 
as follows:

 - Github offers a guide for [creating an issue](https://help.github.com/en/articles/creating-an-issue).
 - Make sure the issue title gives clear indication of the topic.
 - Provide enough context in the body of the issue for the project team
   to have a clear idea of what is suggested.

## Contributing a Blog Post (or news article)

We want to hear about solutions implemented by our users as well as interesting
activities related to our video conferencing services. As such, you are 
welcome to publish short blog posts on this website to tell others how you've
solved problems related to video conferencing or how you are using video 
conferencing at your institution.

To contribute a blog post, please follow these steps:

1. If you are not familiar with Github, you are welcome to send us your story
[via email](mailto:vidyo@tenet.ac.za).
2. If you are familiar with Github, follow these steps:

 - Log into Github (or [create your free acount](#creating-a-github-account).
 - Navigate to the [_posts folder](_posts).
 - If the topic you want to publish a blog post on already exists, click
   on the relevent link.
 - If you are writing about a new topic, create a new directory by clicking 
   `Create new file`.

   - You will create the new topic folder together with the new file in one
     go.
   - In the empty box that appears next to `_posts/` type the name of your topic
     followed by a `/` followed by the name of your file for the post.
   
     - Folder naming conventions: all small letters, no spaces. Keep it short
     - File naming conventions: `yyyy-mm-dd-file-name.md`.
     - It is critical to name the files and folders correctly to ensure 
       your blog post will appear on the website.
     - An exammple of what you may enter in the step above is:
       `large-events/2028-10-20-largest-vidyo-event-held.md`
     - The extension `md` is to show that this file will be written in
       [markdown](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf).
   
   - In the big open box you can type your blog post. 
   - The post should always start with the header in the format:

      ```
      ---
      layout: page
      subheadline: fixme
      title:  "fixme"
      teaser: "fixme"
      meta_teaser: ""
      breadcrumb: true
      categories:
         - fixme - name of folder in which the post is created
      header:
         image_fullwidth: "whitebackground.png"
      tags:
         - fixme
         - fixme
         - fixme
         - fixme
      author: fixme
      ---
      ```
    - Replace the `fixme` in every line with the relevant text. Where you see `""` being used, please do not delete these as it is critical for rendering the website correctly.
    - Add any number of tags (four is just an example).
    - Keep the spacing exactly like this example.
    - Do not remove the `---` at the beginning and end of the header.
    - Here is an example:
      ```
      ---
      layout: page
      subheadline: Carpentries Instructor Training
      title:  "First Carpentry Instructor Training for 2018"
      teaser: "From 21 to 23 February 2018 researchers, postgraduate students, IT, and library staff
      will be able to learn how to teach programming at the fourth in-person Software and Data Carpentry 
      Instructor Training workshop in South Africa."
      meta_teaser: ""
      breadcrumb: true
      categories:
          - carpentries
      header:
          image_fullwidth: "whitebackground.png"
      tags:
          - Software Carpentry
          - Data Carpentry
          - Instructor Training
          - Train-the-Trainer
      author: Anelda van der Walt
      ---
      ```
      
   - Below the closing `---` you can type the blog post in Markdown format. Learn more about [Markdown](https://www.markdownguide.org/basic-syntax). Don't be afraid of Markdown. It is a relatively easy-to-use markup language.
   - For more examples on the formatting, look at previous blog posts in the repository's [`_posts` folder](_posts).
   - Remember to add a short commit message at the bottom of the page and click on `Commit changes` once you are happy with your contributions.
   - When you are done with your changes, click on `Pull Requests` at the top of the page.
   - Click on `New Pull Request`.
   - Make sure you are comparing the `gh-pages branch` copy of the website repository under your username with the original website repostiory's `gh-pages`.
   - Leave a short message to describe what you'd like to contribute to the website.
   - Click on `Create Pull Request`
   
## Changing the Navigation Menu

- There are two steps to changing the navigation menu:

  - Adding or removing an item on the menu itself
  - Creating or deleting a page that is linked to from the relevant navigation menu item
  
### To add or remove an item on the navigation menu:

- Navigate to the [`_data/navigation.yml`](_data/navigation.yml) folder in the repository.
- Click on the little pencil icon to edit the file.
- Each individual navigation menu item is listed in this file with its relevant information e.g. link, submenu items, their links, etc.
- Make very sure that the spacing remains the same when deleting or adding an item.
- To add a main menu item to the file simply add the following lines (replace the example text with your desired title, and url, also note whether this menu item should appear on the left of the page or on the right):
  ```
  - title: "Video Conferencing Platform"
    url: "/video-conferencing/"
    side: left
   ```
- To add a submenu item simply add the following lines underneath an existing main menu item after adding `dropdown`. Our submenu example is added to the existing `News & Updates` main menu item:
  ```
  - title: "News & Updates"
    url: "/blog/"
    side: left
    dropdown:
    - title: "News Archive"
      url: "/blog/archive/"
  ```
- Remember to add a short commit message at the bottom of the page and click on `Commit changes` once you are happy with your contributions.

### To create a new file for the new navigation menu or submenu item

- Navigate to the [`pages`](pages) folder in the repository.
- Create a new file with the same name as the url that was used in the `navigation.yml` file in the previous step. 
- Remember that you are creating a Markdown file, so the file extension will be `.md`.
- For example, in the previous step we added a dropdown menu item `archive` to the existing `blog` menu item. When we create the file to which this new menu item will link, it is called `archive.md` and is created directly in the `pages` folder.
- Every new page that is created here, have to include the following header:
   ```
   ---
   layout: page
   title: "fixme"
   teaser: "fixme"
   permalink: "/blog/archive"
   ---
   ```
 - Do not change the `layout: page` as this will ensure the page is formatted correctly
 - Add a title inside the `""` 
 - Add a teaser inside the `""` - this is a short sentence that will tell readers what information this page will contain.
 - Add the permalink - this is the URL to the page and is the same as the URL that was added to the `navigation.yml` page in the previous step. Do not add a trailing `/` in this header though.
 - Remember the leading and trailing `---` to denote the header.

- The rest of the page can now be created in [Markdown](https://www.markdownguide.org/basic-syntax). Markdown is a simple, easy-to-use markup language used in many contexts to format documents. 
- Remember to add a short commit message at the bottom of the page and click on `Commit changes` once you are happy with your contributions.

## Adding Images to Blog Posts or Pages

- Upload the image to the repository's [`images`](images) folder.
 - First navigate to the [`images`](images) folder.
 - Click on `Upload file`.
 - Select the file or files you want to add to the `images` folder and wait for it to upload.
 - Remember to add a short commit message at the bottom of the page and click on `Commit changes` once you are happy with your contributions.
 
- Link to the image in the relevant page or blog post using markdown and the following relative link: 
`![description of image]({{ site.url }}{{ site.baseurl }}/images/your_image_name.png)`.
- Remember to add a short commit message at the bottom of the page and click on `Commit changes` once you are happy with your contributions.


## Changing the Home Page Layout, Images or Text

- The file that creates the homepage is in [`pages/pages_root_folder/`](pages/pages_root_foler) and is called [`index.md`](pages/pages_root_folder/index.md).
- You can easily edit the following elements:

 - The header image (this points to an image that is available in the [`images`](images) folder).
 - The three widgets' image, title, text, and URL to which it points.
 - The "call for action" and where it links to.

 - Remember to add a short commit message at the bottom of the page and click on `Commit changes` once you are happy with your contributions.
 
 ## Changing Content on Existing Pages
 
 - All the pages (except for the homepage) is available in the [`pages`](pages) folder.
 - To find out which file links to which menu item in order to modify the correct file, visit the [`_data/navigation.yml`](_data/navigation.yml) folder.
 - Click on the filename of the file that you'd like to edit.
 - Then click on the pencil icon.
 - Remember to add a short commit message at the bottom of the page and click on `Commit changes` once you are happy with your contributions.
 
## Changing the Website Logo, Slogan, Description, etc.

- The website general setup is found in [`config.yml`](config.yml).
- Make sure that the spacing and general formatting of this file stays exactly as it is to ensure correct rendering.
- Once you've made your changes, add a short commit message at the bottom of the page and click on `Commit Changes`.
