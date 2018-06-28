## Mailings during the AV102 course

1. Export the folks from the AV102 course using the Instructor --> Data Download --> Download profile information as a CSV

![](https://dl.dropboxusercontent.com/s/wbrsqfxos2lu8gj/Screenshot%202017-09-21%2011.32.10.png?dl=0)

2. Wait for the export process to complete:

![](https://dl.dropboxusercontent.com/s/3yd3a1f4i2hdf20/Screenshot%202017-09-21%2011.33.01.png?dl=0)

3. Open that CSV file in some spreadsheet app, and go to the "Create list" functionality in mailchimp (or alternatively "replicate" one of the existing lists):

![](https://dl.dropboxusercontent.com/s/kthfjoxiwc1h434/Screenshot%202017-09-21%2011.34.54.png?dl=0)

4.  Fill in the list details appropriately, and save :

![](https://dl.dropboxusercontent.com/s/57qib5irkcno6zd/Screenshot%202017-09-21%2011.36.44.png?dl=0)

5. Now we need to import subscribers

![](https://dl.dropboxusercontent.com/s/bwq17zsola63xvk/Screenshot%202017-09-21%2011.37.26.png?dl=0)

6. I find copy and pasting from an existing file easiest:

![](https://dl.dropboxusercontent.com/s/2bb45zgivqctl1j/Screenshot%202017-09-21%2011.37.58.png?dl=0)

7. However it want's first and last names that we don't get from edX, so in google spreadsheets I clean up the data a little and then use the following formulas to extract first and last names:

```
=LEFT(A1, FIND(" ", A1)) 
```
```
=TRIM( RIGHT( SUBSTITUTE( TRIM( A1 ) , " " , REPT( " " , 100 ) ) , 100 ) )
```
and paste the re-organised data into MailChimp that requires me to press confirm many times and finally we have the current members of the course in the list.

8. So now it's time to replicate the first week intro mail from the previous run of the course:

![](https://dl.dropboxusercontent.com/s/cv2rtag6fexbzqb/Screenshot%202017-09-21%2011.46.39.png?dl=0)

9. Make sure we are sending to the correct list:

![](https://dl.dropboxusercontent.com/s/mzii1rsuonevasl/Screenshot%202017-09-21%2011.47.29.png?dl=0)

10. Adjust the campaign name and the email subject line:

![](https://dl.dropboxusercontent.com/s/bawtt4k7b4rkige/Screenshot%202017-09-21%2011.49.07.png?dl=0)

11. Now we need to edit the message appropriately - in particular updating links to the course

![](https://dl.dropboxusercontent.com/s/2icubmdkkj9zfsd/Screenshot%202017-09-21%2011.51.35.png?dl=0)

12. Then we send a test email to check how it looks in an email client and that all the links are working:

![](https://dl.dropboxusercontent.com/s/lixgm5yone01ifp/Screenshot%202017-09-21%2011.52.19.png?dl=0)

13. Here's how it looks in my email client:

![](https://dl.dropboxusercontent.com/s/qwars1fkp3enkbb/Screenshot%202017-09-21%2011.55.15.png?dl=0)

14. Clicking through on each of the four links in the email I can see that they are pointing to the correct places in *the correct version of the course*!

15. We can also test the names are being merged correctly, in the preview mode:

![](https://dl.dropboxusercontent.com/s/y5n0cue4uggnp22/Screenshot%202017-09-21%2011.56.43.png?dl=0)

16. And I see I screwed that up, we don't have a `*|FULLNAME|*` tag, we have `*|FNAME|*`, so I went back through and updated that, and time to get it sent:

![](https://dl.dropboxusercontent.com/s/9acktzar7h1km1m/Screenshot%202017-09-21%2012.24.58.png?dl=0)



## Mailings during the MOOC

1. Go to MailChimp, login as AgileVentures

2. Click on campaigns in top nav to get previous campaigns:

![](https://dl.dropboxusercontent.com/s/v5rfi3fbl8svvs6/Screenshot%202017-07-11%2016.07.18.png?dl=1)

3. check what week is visible to learners in the AV102 course:

![](https://dl.dropboxusercontent.com/s/hesf1e10sexce4e/Screenshot%202017-07-12%2016.10.10.png?dl=1)

![](https://dl.dropboxusercontent.com/s/8lbp47z4qs3wcv3/Screenshot%202017-07-12%2016.10.23.png?dl=1)

I have to say that I've got these all kind of confused.  Right now I'm about to send out part 9 (which corresponds to week 1 of the 2nd MOOC - I really need to sort all these numbers out - but then not that many people even get to this point).

But anyway the idea is to get a link to the specific week that the TAs should be submitting the efforts to:

https://edge.edx.org/courses/course-v1:AgileVentures+AV102+Spring_2017/courseware/276cd2cb381545c28e4ec61c5047f202/5d2e7083f00a4d109a458c7d5cd0361a/

4. Clone the appropriate previous emailing

![](https://dl.dropboxusercontent.com/s/76kyy9xw5ddvt9r/Screenshot%202017-07-12%2016.24.02.png?dl=1)

![](https://dl.dropboxusercontent.com/s/ufmf57c7exw991l/Screenshot%202017-07-12%2018.17.27.png?dl=1)

5. Then switch to the correct group of email addresses:

![](https://dl.dropboxusercontent.com/s/qryn6x71mudgo5h/Screenshot%202017-07-12%2018.18.16.png?dl=1)

6. Adjust the campagign name appropriately

![](https://dl.dropboxusercontent.com/s/ihkgq1isazuzvgq/Screenshot%202017-07-12%2018.19.55.png?dl=1)

7. Adjust the text of the campaign appropriately

![](https://dl.dropboxusercontent.com/s/7y9mqd2qpd6c4o4/Screenshot%202017-07-29%2012.01.46.png?dl=1)

including updating the link to the relevant part of the AV102 course.

8. Then send it out - although usually we should send a test email first to check the links are working etc ...
