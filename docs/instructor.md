---
layout: default
title: "UB Math Exams: Instructor's Guide"
splash: "'assets/images/jumbo_instructor_bgd.png'"
version: "2020.11.05"
---



<div class="alert alert-dismissible alert-info">
  <h4 class="alert-heading">Quick links</h4>
  <ul>
  <li> <a href="/exam_guides/index.html">Math Exams Student's Guide</a> - exam instructions for students.</li>
  <li> <a href="/exam_guides/proctor.html">Math Exams Proctors's Guide</a> - exam instructions for proctors.</li>
  <li> <a href="https://exams.math.buffalo.edu/zoom"> exams.math.buffalo.edu/zoom</a> - portal for accessing exam Zoom meeings (from phone/tablet).</li>
  <li> <a href="https://exams.math.buffalo.edu"> exams.math.buffalo.edu</a> - portal for accessing exam problems (from a computer).</li>
  <li> <a href="http://blue.math.buffalo.edu/exams_next_7_days.html"> Exam meetings for the next 7 days</a>.</li>
  </ul>
</div>


<br/>
<br/>

## Introduction

This document describes procedures for administering exams remotely. These procedures are  meant to enforce academic integrity
and curtail rampant cheating that majority of our instructors experienced during the online part of the spring 2020 semester.

**Here are the  main features of this systems:**

* Live proctoring of exams in relatively small groups of up to 30 students. All groups are taking the exam in parallel during
  the designated exam time. Each group is supervised by a proctor selected from among Math Department teaching assistants.
* Using students’ smartphones as video cameras during exams. This allows for positioning cameras in a way that provides a much better  
  view of each student and his/her work environment than it is possible with webcams built into computers.
* Using an exam server for distribution of  exams to students.  The exam server can individualize exams (e.g. by watermarking them)
  and can provide access for each student to his/her copy of the exam.


## Exam Preparation

#### Exam server

Benefits of using the Exam Server include logging exam access times, watermarking exams, and coloring of exams for easier proctoring.  
An account on the server has been created for every instructor. You log in with your UB username and password. A complete user's guide
is here: [Exam Server User's Guide](http://blue.math.buffalo.edu/nsm_exam_server.html).

The two ingredients needed to build an exam are:
* your exam pdf (or tex or docx)
* your class roster with PINs that was generated for you by the Associate Chair

With a VPN connection, upload these two files to your exams folder on the server, `yogiberra.sens.buffalo.edu`. Then log in, navigate to your exams
folder and run the watermark script:

```
watermark myexam.pdf myroster.csv
```

<br/>
It is extremely helpful to the exam proctors if the exam question paper has a strong distinctive color. This can be achieved
by adding a [hexadecimal color](https://htmlcolorcodes.com/){:target="_blank" rel="noopener"} specification:

```
watermark myexam.pdf myroster.csv color=00ffff
```
<br/>
Save and keep secret the exam password that is generated, which will look something like this:

```
Password: HWERXA
```

<br/>
To access their exam pdf, your students will go to [exams.math.buffalo.edu](https://exams.math.buffalo.edu){:target="_blank" rel="noopener"}
and enter their UBIT username, their personal exam server PIN, and the above exam password which should be kept secret until
it is delivered to the students at the moment you want them to start work on the exam.

#### UBlearns and Respondus eliminated

Live proctoring eliminates the need for Respondus Lockdown Browser and Monitor, which in turn entirely eliminates the need
to use UBlearns for the administration of exams. This greatly simplifies both the preparation process for instructors and
the access process for students, and removes our vulnerability to UBlearns service outages - which have been frequent recently.

#### Gradescope

Once the exam is completed, students will need to submit their work for grading. The recommended tool for this is Gradescope,
an online service facilitating submission and grading of student assignments.  Since many instructors used Gradescope in the spring
semester or are using it now, the students may be familiar with it already. Instructions on how to use Gradescope are available online
at [www.ubgradescope.info](https://www.ubgradescope.info){:target="_blank" rel="noopener"}.   

In order to use Gradescope for collecting exams you need to:
* create your course on Gradescope (if you have not done it already) and enroll your students in
  the course by uploading a csv course roster;
* create a Gradescope assignment for the exam;
* instruct students that they need to submit their work to Gradescope when the exam is over.

If you have not used Gradescope in your course before, it is useful to create a practice assignment before an exam, so students
can get some experience with the Gradescope submission process.

It is possible to use UBLearns, instead of Gradescope, to collect exams, but tools provided by UBLearns for exam collection and
grading are much more limited and less user friendly than what is available with Gradescope.




## Proctoring setup

<div class="container" style="padding-left:0">
     <div class="row">
        <div class="col-lg">
        <p>During an exam students will be proctored via a Zoom meeting which they  join using the Zoom app on their phone.
        This setup offers a better view of student environment than the one provided by a camera built into their computer.</p>

        <p>For proctoring purposes, your class will be split into groups of no more than 30 students. Each group will take the exam
        in a separate Zoom meeting, with all meetings running in parallel at the same time.  Each group has a TA assigned as the proctor.
        A table of meetings occurring in the next 7 days, with the Zoom links, is maintained
        <a href="http://blue.math.buffalo.edu/exams_next_7_days.html">here</a>). The complete current list of proctoring
        assignments is available here: <a href="http://blue.math.buffalo.edu/2209_exam_proctor_schedule_rev4b.xlsx">2209_exam_proctor_schedule_rev4b.xlsx</a>
        (sort by whichever columns are relevant to you).
        </div>
        <div class="col-lg">
        <img style='width:500px;' src="./assets/images/proctoring_setup.png" />
       </div>
    </div>
</div>


<br/>

## Preparation for proctoring

There are two pieces of information that you will need before an exam in order to proctor it:

* **A link to the exam Zoom meeting.** These meetings are centrally scheduled by the Math Department - proctors do not schedule these meetings.  
  When a meeting you are assigned to proctor is scheduled, you will receive an email from Zoom informing you that you have been made
  an Alternative Host of the meeting. You can also find the link to this meeting  here.
* **The exam password.** You will need to announce this password to students, so that they can access exam questions.  
  The password should be provided to you by the instructor of the course for which you are proctoring, ahead of the exam.

In addition, you should have access to the Math Department Discord Server, which will be used for communications
between proctors of various exam sessions and the course instructor during the exam. If you don't have access to this
Discord server contact John Ringland, the Associate Chair (ringland@buffalo.edu). Before you proctor an exam  please also
review the Exam Guide for Students so you are familiar how the exam is supposed to look from a student perspective.

<br/>


#### Zoom configuration

Most settings of exam Zoom meetings are automatically set when a meeting is scheduled.
However, the setting for recording of the meeting must be configured in your own account in order to work correctly:

1. Use the web browser interface for Zoom ([buffalo.zoom.us](https://buffalo.zoom.us){:target="_blank" rel="noopener"})
   to log in to your UB Zoom account.
2. In the Zoom account click on Settings and then on the **Recording** tab.
3. Turn ***Cloud Recording*** **ON**.
4. Make sure that the ***Record active speaker, gallery view and shared screen separately*** option is **SELECTED**.
5. Under this option make sure that:
   - ***Active speaker*** is **UNSELECTED**
   - ***Gallery view*** is **SELECTED**
   - ***Shared screen*** is **UNSELECTED**.

The image below shows the correct recording configuration.

<img style="border: 1px solid;" class="img-fluid" src="./assets/images/zoom_recording_settings.png">

<br/>

## Starting a proctoring meeting

1. Start the Zoom meeting at least 15 minutes prior to the start of the exam (20 if possible).

    <div class="alert alert-dismissible alert-info">
    <b>Note.</b> When you start a meeting you may see a pop-up box with the message "You have a meeting currently in-progress.
    Please end it to start a new meeting". This message is due to the way exam Zoom meetings are scheduled. Click on the "End Other Meeting" button.
    </div>

2. Once you start the meeting confirm that meeting settings are correct and adjust them if needed:
   - [Security](assets/images/zoom_security.png){:target="_blank" rel="noopener"}:  
     * Lock Meeting - **UNCHECKED**
     * Enable Waiting Room - **CHECKED**
     * Share screen - **UNCHECKED**
     * Chat - **CHECKED**
     * Rename Themselves - **UNCHECKED**
   - [Chat  → …  → Participant can chat](assets/images/zoom_chat.png){:target="_blank" rel="noopener"}: **with host only**
   - [Video settings](assets/images/zoom_video.png){:target="_blank" rel="noopener"}:
     * Always display participant name on their video - **CHECKED**
     * Hide non-video participants  - **UNCHECKED**  <span class="text-danger"> - <b>this is critical!</b></span>

3. Make sure that the meeting is being recorded. If not, start the recording in the cloud.

4. Go to the Proctoring Room in the Math Dept Discord Server whose number corresponds to your meeting number.
   Use Suite B if Suite A is already in use for a different exam. Post a message in the corresponding text channel that you started the meeting.

   <div class="alert alert-dismissible alert-info">
   <b>Note.</b> It is recommended that you use headphones during the exam to reduce the chance of accidentally letting students
   hear Discord communication. Keep yourself muted in Zoom except when you are deliberately talking to students.
   </div>

<br/>


## Admitting students to the meeting

**Admit students from the waiting room in small groups.** If you are using a Windows or a Mac computer,
you can reorder Zoom videos by dragging them in such way that all videos coming before your own will
be of students whose IDs have been checked already. In this way it will be easier to keep track who still needs to be checked.

**For each admitted student check their UB ID** (a government issued photo ID is acceptable as well):
* Compare the photo in the ID with student's face.
* Compare the name in the ID with the name displayed in Zoom.
* In case of irregularities - name mismatch, no ID etc. make a note in the proctoring text channel on Discord.

<br/>

<div class="jumbotron" style="padding-top:40px; padding-bottom:20px;">
<h2>Students' camera views</h2>
<p> As you are admitting students to the exam,  and also during the exam itself, make sure that students'
cameras are positioned correctly. Instruct students to make adjustments as needed.</p>

<br/>
<div class="container" style="padding-left:0">
     <div class="row">
        <div class="col-lg">
        <h4>Correct camera view</h4>
        <p>This is how that the view from a camera should look. The student, the work surface, and the computer screen are clearly visible.</p>
       </div>
       <div class="col-lg">
        <img style='width:500px;' src="./assets/images/camera_view_correct.png" />
       </div>
    </div>
</div>


<br/>

<h4>Examples of incorrect camera views</h4>
<div class="card-deck">

  <div class="card bg-light" style="min-width: 200px; margin-bottom:20px; padding:4px;">
    <img class="card-img-top" src="./assets/images/incorrect_1.png" alt="Card image cap">
    <div class="card-body">
      <p class="card-text"><span style="color:red;font-weight:600;">&#9888;</span> Work surface not visible.</p>
    </div>
  </div>
  <div class="card bg-light" style="min-width: 200px; margin-bottom:20px; padding:4px;">
    <img class="card-img-top" src="./assets/images/incorrect_2.png" alt="Card image cap">
    <div class="card-body">
      <p class="card-text"><span style="color:red;font-weight:600;">&#9888;</span> Camera too close.</p>
    </div>
  </div>
  <div class="card bg-light" style="min-width: 200px; margin-bottom:20px; padding:4px;">
    <img class="card-img-top" src="./assets/images/incorrect_3.png" alt="Card image cap">
    <div class="card-body">
      <p class="card-text"><span style="color:red;font-weight:600;">&#9888;</span> Part of the computer screen not visible.</p>
    </div>
  </div>
  <div class="card bg-light" style="min-width: 200px; margin-bottom:20px; padding:4px;">
    <img class="card-img-top" src="./assets/images/incorrect_4.png" alt="Card image cap">
    <div class="card-body">
      <p class="card-text"><span style="color:red;font-weight:600;">&#9888;</span> Camera oriented vertically, partial view of the monitor and work surface only.</p>
    </div>
  </div>
  <div class="card bg-light" style="min-width: 200px; margin-bottom:20px; padding:4px;">
    <img class="card-img-top" src="./assets/images/incorrect_5.png" alt="Card image cap">
    <div class="card-body">
      <p class="card-text"><span style="color:red;font-weight:600;">&#9888;</span> Face not visible.</p>
    </div>
  </div>
  <div class="card bg-light" style="min-width: 200px; margin-bottom:20px; padding:4px;">
    <img class="card-img-top" src="./assets/images/incorrect_6.png" alt="Card image cap">
    <div class="card-body">
      <p class="card-text"><span style="color:red;font-weight:600;">&#9888;</span> Video oriented vertically.  To fix this, pick up the phone, wave it around a bit, and set it back down.</p>
    </div>
  </div>
  <div class="card bg-light" style="min-width: 200px; margin-bottom:20px; padding:4px;">
    <img class="card-img-top" src="./assets/images/incorrect_7.png" alt="Card image cap">
    <div class="card-body">
      <p class="card-text"><span style="color:red;font-weight:600;">&#9888;</span> Computer screen not in the picture.</p>
    </div>
  </div>
  <div class="card bg-light" style="min-width: 200px; margin-bottom:20px; padding:4px;">
    <img class="card-img-top" src="./assets/images/incorrect_8.png" alt="Card image cap">
    <div class="card-body">
      <p class="card-text"><span style="color:red;font-weight:600;">&#9888;</span> Headphones/earbuds are not allowed.</p>
    </div>
  </div>

</div>
</div>

<br/>


## During the exam

#### Starting the exam

* **Immediately before the exam starts** announce what the exam checkout procedure is (see below).
* Announce the exam password. This will let the students access the exam from their computers through
  the website [exams.math.buffalo.edu](https://exams.math.buffalo.edu) and start working on the exams.

#### Once the exam has started

* Keep an eye on the waiting room for late-comers or students who drop out from the meeting and return.
  Anyone entering from the waiting room needs to have their ID checked (or re-checked). If you notice
  a student who dropped from the meeting and re-entered make a note in the Discord text channel.  

* Enforce video-on for all students throughout the exam. If a student's video is off, and they do not properly
  respond to request(s) to turn it on, remove them from the meeting and make a record that you did it in Discord.

* Be sure to keep your audio muted except when you need to speak to students.

* If any student's video does not show everything you need to see, have them correct it.

* If a student is willfully or repeatedly not complying with your instructions, let them know that if they do not
  comply within the next minute, they will be ejected from the meeting and get a 0 on the exam. If you do eject anyone,
  make a note in Discord.

* Monitor students carefully. Be on the alert for any form of cheating and actively communicate with students to correct
  any irregularities. Pin student's video for a closer view if needed.


<div class="alert alert-dismissible alert-danger">
<h4>Red flags</h4>
<ul>
<li> student is typing </li>
<li> student is scrolling a lot </li>
<li> student is looking at different documents on their computer </li>
<li> student is looking repeatedly at the Zoom camera (i.e. their phone) </li>
<li> student is looking repeatedly at any location other than computer screen or paper </li>
<li> student appears to be talking </li>
<li> student is wearing earbuds/headphones (not allowed) </li>
<li> student is using a virtual background (not allowed). </li>
</ul>


<p><b>In case of any suspicious behavior</b> make a note of the issue in the text channel of Discord.
Communicate with the student either verbally or in the Zoom chat - as appropriate. In case of text chat, inform
the student that they should check their chat messages.</p>
</div>


<br/>

## Exam checkout

* Students should use the Raise Hand feature to signal that they are ready to leave the exam. When you notice it,
  tell the student to show exam pages to the camera one by one. The student should position the camera over
  a stack of pages and remove pages one one stopping for about 1 second for each page.
  Here is a [short video](https://ub.hosted.panopto.com/Panopto/Pages/Viewer.aspx?id=1665fd0d-3d0a-4c76-9049-ac5b00e8a2da){:target="_blank" rel="noopener"}
  demonstration of this process.

* Once a student shows all exam pages tells the student that they may leave the Zoom meeting and upload their work
  to Gradescope.  

  **Note:** If there are several students waiting to be checked out, acknowledge that you see them by
  making an announcement that they will be checked out shortly.

When all students leave the Zoom meeting, close the meeting. Your  duties are finished!
