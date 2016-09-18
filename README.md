maker-site
==========

DDPSC Maker Site

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
<p>- ...</p>
<p>img: post01.jpg       #place image (850x450) with this name in /assets/img/blog/</p>
<p>thumb: thumb01.jpg    #place thumbnail (70x70) with this name in /assets/img/blog/thumbs/</p>
<p>---</p>
<p>This text will appear in the excerpt "post preview" on the Blog page that lists all the posts.</p>
<p><!--more--></p>
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
<p>img: portfolio_10.jpg #place image (600x450) with this name in /assets/img/project/</p>
<p>carousel:</p>
<p>- single01.jpg        #place image (1280x600) with this name in /assets/img/project/carousel/</p>
<p>- single02.jpg  </p>
<p>- ...</p>

<p>lab: lab of project</p>
<p>website: webpage of lab</p>
<p>---</p>

<p>This is a regular paragraph. Write as much as you like.</p>

=======================================================
