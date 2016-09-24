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

<p><b>---</b></p>
<p><b>layout: post</b>          #important: don't change this</p>
<p><b>title:</b> "Name of post like this"</p>
<p><b>date:</b> yyyy-mm-dd hh:mm:ss</p>
<p><b>author:</b> Name</p>
<p><b>categories:</b></p>
<p><b>- blog</b>                #important: leave this here</p>
<p><b>-</b> category1</p>
<p><b>-</b> category2</p>
<p><b>img:</b> post01.jpg       #place image (850x450) with this name in /assets/img/blog/</p>
<p><b>thumb:</b> thumb01.jpg    #place thumbnail (70x70) with this name in /assets/img/blog/thumbs/</p>
<p><b>---</b></p>
<p>This text will appear in the excerpt "post preview" on the Blog page that lists all the posts.</p>

<p><b><
!--more--></b></p>
<p>This text will not be shown in the excerpt because it is after the excerpt separator.</p>

=======================================================


<h3>Project post</h3>

<p>Create a Project post to go in your Portfolio by creating a file called yyyy-mm-dd-name-of-the-project.markdown in the /_posts/project/ directory with the following template:</p>


<p><b>---</b></p>
<p><b>layout: project</b>       #important: don't change this</p>
<p><b>title:</b>  "Name of the project"</p>
<p><b>date:</b> yyyy-mm-dd hh:mm:ss</p>
<p><b>author:</b> Name</p>
<p><b>categories:</b></p>
<p><b>- project</b>             #important: leave this here</p>
<p><b>-</b> category1</p>
<p><b>-</b> category2</p>
<p><b>img:</b> portfolio_10.jpg #place image (600x450) with this name in /assets/img/project/</p>
<p><b>carousel:</b></p>
<p><b>-</b> single01.jpg        #place image (1280x600) with this name in /assets/img/project/carousel/</p>
<p><b>-</b> single02.jpg  </p>

<p><b>lab:</b> lab of project</p>
<p><b>website:</b> webpage of lab</p>
<p><b>---</b></p>

<p>This is a regular paragraph. Write as much as you like.</p>

<p><b><
!--more--></b></p>
<p>This text will not be shown in the excerpt because it is after the excerpt separator.</p>

=======================================================

<h3>Tutorial post</h3>

<p>Create a Tutorial post to go in tutorial by creating a file called yyyy-mm-dd-name-of-the-project.markdown in the /_posts/tutorial/ directory with the following template:</p>


<p><b>---</b></p>
<p><b>layout: tutorial_post</b>      #important: don't change this</p>
<p><b>title:</b>  "Name of the tutorial"</p>
<p><b>date:</b> yyyy-mm-dd hh:mm:ss</p>
<p><b>author:</b> Name</p>
<p><b>categories:</b></p>
<p><b>- tutorial</b>             #important: leave this here</p>
<p><b>-</b> category1</p>
<p><b>-</b> category2</p>
<p><b>img:</b> tutorial_10.jpg #place image (600x450) with this name in /assets/img/tutorial/</p>
<p><b>thumb:</b> thumb01.jpg    #place thumbnail (70x70) with this name in /assets/img/blog/thumbs/</p>

<p><b>---</b></p>

<p>This is a regular paragraph. Write as much as you like.</p>

<p><b><
!--more--></b></p>
<p>This text will not be shown in the excerpt because it is after the excerpt separator.</p>

=======================================================

<h3>Outreach post</h3>

<p>Create a Outreach post to go in outreach by creating a file called yyyy-mm-dd-name-of-the-project.markdown in the /_posts/outreach/ directory with the following template:</p>


<p><b>---</b></p>
<p><b>layout: outreach_post</b>      #important: don't change this</p>
<p><b>title:</b>  "Name of the post"</p>
<p><b>date:</b> yyyy-mm-dd hh:mm:ss</p>
<p><b>author:</b> Name</p>
<p><b>categories:</b></p>
<p><b>-</b> category1</p>
<p><b>-</b> category2</p>
<p><b>- outreach</b>             #important: leave this here</p>
<p><b>img:</b> outreach_10.jpg #place image (600x450) with this name in /assets/img/outreach/</p>
<p><b>thumb:</b> thumb01.jpg    #place thumbnail (70x70) with this name in /assets/img/blog/thumbs/</p>

<p><b>---</b></p>

<p>This is a regular paragraph. Write as much as you like.</p>

<p><b><
!--more--></b></p>
<p>This text will not be shown in the excerpt because it is after the excerpt separator.</p>