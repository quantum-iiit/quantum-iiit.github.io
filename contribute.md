# How to contribute

(in progress)

Here's an outline of how the system is structured, followed by a description of the various roles. 

## Current structure
(updated: Sunday, April 6, 2025)

* Gaggle is used to create mailing lists. There are two such mailing lists: quantum-seminars and quantum-meets at gaggle.email. The latter is for internal use (includes all events, including in-person events) and the former for announcing events that can be attended online.
* The backbone of the setup are 
    * The Google calendar called “Quantum Meets | IIIT”
    * Calendly
    * The GitHub webpage (quantum-iiit.github.io)
    * Google Apps Script
* Google calendar
    * Use older events to stay consistent with the format
    * The phrase “Quantum Tea” (not case sensitive) and the emoji 🏫 are used to declare the event as in person only
    * Quantum Meets Ghost | Events here are treated as “busy” or “unavailable” when new events are scheduled
* Calendly
    * Send this link https://calendly.com/toatularora/quantum-seminar to speakers to select
    * Change available slots (signed in using toAtulArora@gmail.com)
* GitHub webpage
    * The tags ```<!-- SKIP_START -->``` and ```<!-- SKIP_END -->``` are used to determine what is excluded from the email
    * The “Title” and the “About” section is automatically excluded from the email
* Google Apps Script
    * Weekly email: 
        * This scrapes from quantum-iiit.github.io and prepares a nice email
        * It checks whether there are any events in the coming week—and if not, doesn’t send an email
        * Sent to both quantum seminar and quantum meets
    * One day reminder:
        * Checks for events the next day
        * If so, 
            * sends to quantum seminar
            * If all events are in person, does not send to quantum seminar
                * Otherwise sends to quantum seminar as well
    * 4 hour reminder:
        * Similar to the one above—except it is triggered every hour
* The final piece is Outlook
    * It forwards emails from quantum seminar
        * to Faculty and Students
    * It forwards emails from quantum meets
        * to CQST

So when we make things multi-institute, we only need to change the last piece.

I am using toAtulArora@gmail.com for all of these. The sign in in Calendly and in gaggle are through toAtulArora@gmail.com

## Roles

* **Coordinator.** 

* **Web maintainer.**
  * *Load.* About twenty minutes a week.
  * *Task.*
    * Calendar. (when requested) Get the abstract and title from the link. Leave the venue as TBA.
    * GitHub page. (every Fri or Saturday) 

* **Video Editor.** 
  * *Load.* After familiarity with the tools, about twenty minutes (excluding export/upload/download) time.
  * *Task.* Blur out everyone except the speaker and the slides. Upload to YouTube with the correct metadata. (TODO: expand)
