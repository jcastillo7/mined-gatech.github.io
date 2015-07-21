#Add a News Post
To add a new news post to the homepage of [mined.gatech.edu](http://www.mined.gatech.edu), visit the Github repo by clicking [here](https://github.com/mined-gatech/mined-gatech.github.io).

##Create Post
Navigate to the `_posts` folder. Then navigate to the `news` folder. Once inside, add a new file by clicking the plus button. 

To obtain the correct format, copy the template code below and paste it into your file:

    ---
    layout: post
    title: "This is the Title of Your News"
	modified: 
	categories: news
	excerpt: This can be a short sentence describing the news post, although this is optional.
	tags: 
	date: 2015-07-21
	link: http://www.example-link.com
	---

##Edit Post
Once you have pasted the above code, the only variables that you need to edit are `title`, `excerpt`, `date`, and `link`. Details are described below.

1. `title`: This is simply the title of your news post.
2. `excerpt`: This is an optional variable that will display a short sentence or description of what the news is about below the title.
3. `date`: The date should be formatted as year-month-day. For example: `date: 2015-07-21`.
4. `link`: This is an optional variable that when provided will send the viewer to another website. If you news post does not need a link, then delete the variable. 

##Name Post
In the Github text field that says "Name your file" type the following: `2015-07-21-my-template-news-post.md`, where the date you chose in the previous section is used at the beginning and an appropriate title for your news is used at the end.

##Commit Changes
At the bottom of the page the "Commit changes" text fields should have auto-filled a title and description. Feel free to change those. Otherwise, click the "Commit changes" button.

Now visit [mined.gatech.edu](https://www.mined.gatech.edu) to see your new news! You may need to refresh the page for it to appear.
