# Digital Skills Tool 2022
A website to provide prototyped forms to support classes for people to learn digital skills

The code base was initially here: [DigitalSkillsTool](https://github.com/stephanie-K/DigitalSkillsTool)

_The GOV.UK prototype version used to run it was old and it would have been hard to update it. It's deployed and hosted by Heroku who changed their support model in November 2022. Without updating the prototype kit, it could not be deployed anymore This new codebase is now using a more recent version of the kit and reuse most of the previous views._
_It's not used to support classes anymore but I'm keeping it to be able to show how it worked._


# Previous description of this work

This is the code for a website to support classes to help refugees and other participants to improve their digital skills by training on prototyped forms of exisiting services.


**There is about 1 in 7 people in Scotland who can’t get online** (that’s about 800,000 people)

The course is developed for the **East Renfrewshire Council** and the website supporting the classes is the result of the work of many people who either: mapped the forms, coded them, or tested them:

- [Alexandria Rocks](https://www.linkedin.com/in/alexandria-rocks/)
- [Anastasia Moneva](https://www.linkedin.com/in/anastasia-moneva-6b192189/)
- [Ashir Qureshi](https://www.linkedin.com/in/ashir-qureshi/)
- [Craig Barratt](https://www.linkedin.com/in/craig-barratt-softdev/)
- [Paul Marshall](https://www.linkedin.com/in/paulkmarshall/)



This is using the [**GOV.UK Prototype kit**](https://prototype-kit.service.gov.uk/docs/)

You can [**learn more about the project in this blog post**](https://blog.chezleskrus.com/2020/08/01/improving-digital-skills-a-tool-using-the-gov-uk-prototype-kit-part-2/)

## How we are using the tool

Different forms are needed to support the classes. Some are Council forms, some are GOVUK form and others are Scottish Government forms.

Different layouts have to be created for each and even among each category, there is a variety of layouts:

For example, the DVLA have a different layout and style compared to HMRC, or the Social Security Scotland have it's own style.

## Important files and paths

### Layout files in app>views>layouts>

- **layout.html** - default GOV.UK layout
- **layout_erc.html** - customised for Council forms
- **layout_sg.html** - customised for Scottish Government
- **layout_sss.html** - customised for Social Security Scotland
- **layout_tool.html** - look like the council one but for high level pages of the tool

### CSS/SASS files in app>assets>sass>
- **application.scss** - default GOV.UK css plus some we added for GOVUK forms
- **erc.scss** - styles to support the council forms
- **sg.scss** - style to support the Social Security Scotland and Scottish Government forms
- **other.scss** - style for other forms

### Each form has a folder app>views>forms>

### Route.js app>

This file is key to introduce logic and validation to the forms. It is shared by all the forms.

## Examples of template page

### A GOV.UK page - desktop view
<br><br>

![screenshot of a GOV.UK page - desktop view](/app/assets/images/document-the-tool/screen-desktop-govuk.png)

<br><hr>

### A GOV.UK page - mobile view
<br><br>

![screenshot of a GOV.UK page - mobileview](/app/assets/images/document-the-tool/screen-mobile-govuk.png)

<br><hr>

### A basic council form
<br><br>

![screenshot of a council page](/app/assets/images/document-the-tool/screen-council.png)

<br><hr>

### A basic Scottish Government page
<br><br>

![screenshotof a Scottish Government page](/app/assets/images/document-the-tool/screen-sg.png)

<br><hr>

### A basic Social Security page - desktop view
<br><br>

![screenshot of Social Security - desktop vie](/app/assets/images/document-the-tool/screen-desktop-sss.png)

<br><hr>

### A basic Social Security page - mobile view
<br><br>

![screenshot of applying for a provisional licence](/app/assets/images/document-the-tool/screen-DVLA-1.png)

<br><hr>

### The start page for: Apply for a provisional driving licence
<br><br>

![screenshot of applying for a provisional licence - start page](/app/assets/images/document-the-tool/screen-DVLA-2.png)

