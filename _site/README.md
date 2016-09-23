maker-site
==========

DDPSC Maker Site

<p>Welcome to the Donald Danforth Plant Science Center Maker Group webpage on GitHub!</p>

<p>To create a new blog, project, tutorial, or outreach post please follow the guide lines below. All thumbnail images are saved in the assets/img/blog/thumbs folder.</p>

<p>For the categories section of each post you can have any number of categories listed but please look at what current categories exist and how they are listed to make sure they link correctly!</p>

<p>For the Project Post you can load as many images as you want in the carousel but please limit to 5 or less images!<p/>

=======================================================

<h3>Blog post</h3>

<p>Create a Blog post by creating a file called yyyy-mm-dd-name-of-post-like-this.markdown in the /_posts/blog/ directory with the following template:</p>

<p>---</p>
<p>layout: post          #important: don't change this</p>
<p>title: "Name of post like this"</p>
<p>date: yyyy-mm-dd hh:mm:ss</p>
<p>author: Name</p>
<p>categories:</p>
<p>- blog                #important: leave this here</p>
<p>- category1</p>
<p>- category2</p>
<p>img: post01.jpg       #place image (850x450) with this name in /assets/img/blog/</p>
<p>thumb: thumb01.jpg    #place thumbnail (70x70) with this name in /assets/img/blog/thumbs/</p>
<p>---</p>
<p>This text will appear in the excerpt "post preview" on the Blog page that lists all the posts.</p>

<p><
!--more--></p>
<p>This text will not be shown in the excerpt because it is after the excerpt separator.</p>

=======================================================


<h3>Project post</h3>

<p>Create a Project post to go in your Portfolio by creating a file called yyyy-mm-dd-name-of-the-project.markdown in the /_posts/project/ directory with the following template:</p>


<p>---</p>
<p>layout: project       #important: don't change this</p>
<p>title:  "Name of the project"</p>
<p>date: yyyy-mm-dd hh:mm:ss</p>
<p>author: Name</p>
<p>categories:</p>
<p>- project             #important: leave this here</p>
<p>- category1</p>
<p>- category2</p>
<p>img: portfolio_10.jpg #place image (600x450) with this name in /assets/img/project/</p>
<p>carousel:</p>
<p>- single01.jpg        #place image (1280x600) with this name in /assets/img/project/carousel/</p>
<p>- single02.jpg  </p>

<p>lab: lab of project</p>
<p>website: webpage of lab</p>
<p>---</p>

<p>This is a regular paragraph. Write as much as you like.</p>

<p><
!--more--></p>
<p>This text will not be shown in the excerpt because it is after the excerpt separator.</p>

=======================================================

<h3>Tutorial post</h3>

<p>Create a Tutorial post to go in tutorial by creating a file called yyyy-mm-dd-name-of-the-project.markdown in the /_posts/tutorial/ directory with the following template:</p>


<p>---</p>
<p>layout: tutorial_post      #important: don't change this</p>
<p>title:  "Name of the tutorial"</p>
<p>date: yyyy-mm-dd hh:mm:ss</p>
<p>author: Name</p>
<p>categories:</p>
<p>- tutorial             #important: leave this here</p>
<p>- category1</p>
<p>- category2</p>
<p>img: tutorial_10.jpg #place image (600x450) with this name in /assets/img/tutorial/</p>
<p>thumb: thumb01.jpg    #place thumbnail (70x70) with this name in /assets/img/blog/thumbs/</p>

<p>---</p>

<p>This is a regular paragraph. Write as much as you like.</p>

<p><
!--more--></p>
<p>This text will not be shown in the excerpt because it is after the excerpt separator.</p>

=======================================================

<h3>Outreach post</h3>

<p>Create a Outreach post to go in outreach by creating a file called yyyy-mm-dd-name-of-the-project.markdown in the /_posts/outreach/ directory with the following template:</p>


<p>---</p>
<p>layout: outreach_post      #important: don't change this</p>
<p>title:  "Name of the post"</p>
<p>date: yyyy-mm-dd hh:mm:ss</p>
<p>author: Name</p>
<p>categories:</p>
<p>- category1</p>
<p>- category2</p>
<p>- outreach             #important: leave this here</p>
<p>img: outreach_10.jpg #place image (600x450) with this name in /assets/img/outreach/</p>
<p>thumb: thumb01.jpg    #place thumbnail (70x70) with this name in /assets/img/blog/thumbs/</p>

<p>---</p>

<p>This is a regular paragraph. Write as much as you like.</p>

<p><
!--more--></p>
<p>This text will not be shown in the excerpt because it is after the excerpt separator.</p>