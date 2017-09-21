ADuRoR Emailings
================

1. Find relevant update from previous run of course, e.g. 

https://studio.edx.org/course_info/course-v1:BerkeleyX+CS169.1x+3T2015SP

Click the edit button

![](https://dl.dropboxusercontent.com/s/qox70kw8xou7pxy/Screenshot%202017-07-01%2011.25.10.png?dl=1)

to access the raw HTML:

![](https://dl.dropboxusercontent.com/s/1n5ewgwpclmfqld/Screenshot%202017-07-01%2011.25.40.png?dl=1)

copy and paste that to a text editor so you can update the text and links

```
<section class="update-description">
<p>Almost finished!</p>
<p>The last week of new material is now available in the <a href="https://courses.edx.org/courses/course-v1:BerkeleyX+CS169.1x+3T2015SP/courseware/7ae5048e43664f2991f69feb03fda55d/13953c675b0d4d29b3cf1adfa3d03d29/">courseware section!</a> You've made it through the majority of the course now and we very much look forward to seeing you in the advanced course coming this fall! Dave and Armando have recorded another screencast on TDD and the testing pyramid:</p>
<br><center><object width="420" height="315"><param name="movie" value="//www.youtube.com/v/eMdYbvl2mNQ?hl=en_US&amp;version=3"><param name="allowFullScreen" value="true"><param name="allowscriptaccess" value="always"><embed src="//www.youtube.com/v/eMdYbvl2mNQ?hl=en_US&amp;version=3" type="application/x-shockwave-flash" width="420" height="315" allowscriptaccess="always" allowfullscreen="true" wmode="transparent"></object></center><br>
<p>We're on the cusp or releasing assignment 5. Keep up the great work in the pairing sessions! Also it's been great to see several of you joining Agile Ventures standups and non-profit open source projects. Note that you can usually catch Professor Sam Joseph in the "Martin Fowler" (08:15 UTC) and "Kent Beck" (15:45 UTC) Scrums Monday to Friday if you want a fast on ramp to the Agile development method process in a real life Ruby or Rails Project:</p>
<p><a href="http://agileventures.org/about-us">http://agileventures.org/about-us</a></p>
<p>-- Armando, Dave, Sam, and the ADuRoR Course Team</p>
<p>As always if you have any questions please don't hesitate to ask in the <a href="https://courses.edx.org/courses/course-v1:BerkeleyX+CS169.1x+3T2015SP/discussion/forum">Discussion Forums</a>.</p>
</section>
```


Update the text as appropriate for the current course, in particular, ensure that all the hyperlinks are to the current run of the course rather than the old run of the course.  The fastest way to go is to navigate to the new course itself, i.e.:

![](https://www.dropbox.com/s/epqgi8rfkw8mgm9/Screenshot%202017-07-01%2011.28.29.png?dl=1)

and grab the relevant hyperlinks from there, e.g. 

```
https://courses.edx.org/courses/course-v1:BerkeleyX+CS169.1x+1T2017SP/courseware/7ae5048e43664f2991f69feb03fda55d/13953c675b0d4d29b3cf1adfa3d03d29/?activate_block_id=block-v1%3ABerkeleyX%2BCS169.1x%2B1T2017SP%2Btype%40sequential%2Bblock%4013953c675b0d4d29b3cf1adfa3d03d29
```

where you'll probably need to remove the "activate" portion like so:

```
https://courses.edx.org/courses/course-v1:BerkeleyX+CS169.1x+1T2017SP/courseware/7ae5048e43664f2991f69feb03fda55d/13953c675b0d4d29b3cf1adfa3d03d29/
```

and then you can create the new update with the correct links like so:

```
<section class="update-description">
<p>Almost finished!</p>
<p>The last week of new material is now available in the <a href="https://courses.edx.org/courses/course-v1:BerkeleyX+CS169.1x+1T2017SP/courseware/7ae5048e43664f2991f69feb03fda55d/13953c675b0d4d29b3cf1adfa3d03d29/">courseware section!</a> You've made it through the majority of the course now and we very much look forward to seeing you in the advanced course coming this fall! Dave and Armando have recorded another screencast on TDD and the testing pyramid:</p>
<br><center><object width="420" height="315"><param name="movie" value="//www.youtube.com/v/eMdYbvl2mNQ?hl=en_US&amp;version=3"><param name="allowFullScreen" value="true"><param name="allowscriptaccess" value="always"><embed src="//www.youtube.com/v/eMdYbvl2mNQ?hl=en_US&amp;version=3" type="application/x-shockwave-flash" width="420" height="315" allowscriptaccess="always" allowfullscreen="true" wmode="transparent"></object></center><br>
<p>Assignment 5 is also available. Keep up the great work in the pairing sessions! Also it's been great to see several of you joining Agile Ventures standups and non-profit open source projects. Note that you can usually catch Professor Sam Joseph in the "Martin Fowler" (12:00 UTC) and "Kent Beck" (15:15 UTC) Scrums Monday to Friday if you want a fast on ramp to the Agile development method process in a real life Ruby or Rails Project:</p>
<p><a href="http://agileventures.org/about-us">http://agileventures.org/about-us</a></p>
<p>-- Armando, Dave, Sam, and the ADuRoR Course Team</p>
<p>As always if you have any questions please don't hesitate to ask in the <a href="https://courses.edx.org/courses/course-v1:BerkeleyX+CS169.1x+1T2017SP/discussion/forum/</a>.</p>
</section>
```

Also, don't forget to update the any links to the forum and chat:

```
https://courses.edx.org/courses/course-v1:BerkeleyX+CS169.1x+1T2017SP/discussion/forum/
```

```
https://courses.edx.org/courses/course-v1:BerkeleyX+CS169.1x+1T2017SP/58ea5c0e789a4b1cb3df5371e25615cd/
```

Then you'll need to navigate to the updates section in the current course, e.g. 

https://studio.edx.org/course_info/course-v1:BerkeleyX+CS169.1x+1T2017SP

and click the "new update" button:

![](https://dl.dropboxusercontent.com/s/gcnrtlrvf7lby9m/Screenshot%202017-07-01%2011.31.59.png?dl=1)

and paste the new update text in:

![](https://dl.dropboxusercontent.com/s/4swtnw5zsumc7qv/Screenshot%202017-07-01%2011.32.17.png?dl=1)

That update will now immediately become live in the main site:

![](https://dl.dropboxusercontent.com/s/jfjlvl5tu3zzwz7/Screenshot%202017-07-01%2011.32.47.png?dl=1)

Do check that it displays correctly in the main site, and that every link operates as expected etc.  You'll be able to see it on the "Home" page:

https://courses.edx.org/courses/course-v1:BerkeleyX+CS169.1x+1T2017SP/info

![](https://dl.dropboxusercontent.com/s/g1j0kkeawwnu132/Screenshot%202017-07-01%2011.34.03.png?dl=1)

Assuming that's all good, and in a really rigorous run of things we would get the update out a day in advance of the mailing and leave it there for any uncaught issues to be flagged up before we distributed the mailing to thousands of people.  

Either way, to send an email, you want to navigate to the instructor portion of the course, which has an email sub-heading:

![](https://dl.dropboxusercontent.com/s/i8pa6l1ngoq22i4/Screenshot%202017-07-01%2011.35.43.png?dl=1)

Start by sending a test email to yourself with an appropriate subject:

![](https://dl.dropboxusercontent.com/s/jufuqw8jwy0jygq/Screenshot%202017-07-01%2011.36.25.png?dl=1)

Probably the easiest thing to do is to press the "HTML" button to edit the message:

![](https://dl.dropboxusercontent.com/s/cq1cak8uphrzv6f/Screenshot%202017-07-01%2011.37.19.png?dl=1)

In order to copy and paste in the update you'll need to avoid using Ctrl-A and use the mouse cursor to select the ```<p></p>``` default, and then you can paste in the same update HTML code that you put in the update section.  Note however that while video embeds will appear to display correctly here, they do not work in emails, so the text will need to be edited to show links to videos rather than embeds:

```
<section class="update-description">
<p>Almost finished!</p>
<p>The last week of new material is now available in the <a href="https://courses.edx.org/courses/course-v1:BerkeleyX+CS169.1x+1T2017SP/courseware/7ae5048e43664f2991f69feb03fda55d/13953c675b0d4d29b3cf1adfa3d03d29/">courseware section!</a> You've made it through the majority of the course now and we very much look forward to seeing you in the advanced course coming this fall! Dave and Armando have recorded another screencast on TDD and the testing pyramid:</p>

<p><a href='http://www.youtube.com/v/eMdYbvl2mNQ'>http://www.youtube.com/v/eMdYbvl2mNQ</p>

<p>Assignment 5 is also available. Keep up the great work in the pairing sessions! Also it's been great to see several of you joining Agile Ventures standups and non-profit open source projects. Note that you can usually catch Professor Sam Joseph in the "Martin Fowler" (12:00 UTC) and "Kent Beck" (15:15 UTC) Scrums Monday to Friday if you want a fast on ramp to the Agile development method process in a real life Ruby or Rails Project:</p>
<p><a href="http://agileventures.org/about-us">http://agileventures.org/about-us</a></p>
<p>-- Armando, Dave, Sam, and the ADuRoR Course Team</p>
<p>As always if you have any questions please don't hesitate to ask in the <a href="https://courses.edx.org/courses/course-v1:BerkeleyX+CS169.1x+1T2017SP/discussion/forum/</a>.</p>
</section>
```

You'll then see the email displayed like so:

![](https://dl.dropboxusercontent.com/s/9abnd877n48xqac/Screenshot%202017-07-01%2011.40.48.png?dl=1)

Check that it is as intended, and then send the test email to yourself.  Make sure you receive the email and that all the links work as expected.  Note in the one above I've got the link to the youtube video wrong, it's going straight to download.  It  should be `https://www.youtube.com/watch?v=eMdYbvl2mNQ` so I fix that:

![](https://dl.dropboxusercontent.com/s/uocbd9d4j979pdo/Screenshot%202017-07-01%2011.44.10.png?dl=1)

and re-test.  With the above link update the youtube video worked, but the link to the forum had an extra quote that broke it, so I had to make one more test email send to get all the links working.  I also find it helpful to read the text again in the email arriving in my inbox and can sometimes find text mistakes there that I don't otherwise see.

If there's something new in the email about a new partner or sponsor (Mooqita, Mentive etc.) then it can be good to do another round of testing with the test email sent to all staff and admins and wait for their input:

![](https://dl.dropboxusercontent.com/s/0t9vqiywjg42vz4/Screenshot%202017-07-01%2011.47.49.png?dl=1)

but if nothing much has changed or been added and you're happy with the result you can go straight to distributing to all learners.  If you're doing this for the first time, please do send one to "staff & admins" and get sign off from at least one other admin.

I was just about to send and saw another error related to when the next course is coming up - I fixed that in the email - and retroactively in the main update on the site.  

Whenever you send an email the site will pop up a warning about who you are sending it to.  Please always double check that you are sending to the right set of people, and if you are sending to all students do remember to remove the word `[TEST]` from the subject line.


