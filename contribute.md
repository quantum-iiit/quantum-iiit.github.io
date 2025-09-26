# How to contribute | Logistics

This page outlines how the system is structured, followed by a description of the various roles. But first, a huge thank you to our new contributors. 

If you're interested in contributing to this effort, please feel free to [write to us](atul.singh.arora@gmail.com). 

## Contributors 

| Name | Role | Contribution period | 
| - | - | - |
| Arnab Ghorui | GitHub maintaner | Aug 2025–present | 
| Himanshu | YouTube maintainer | May 2025–present | 
| Atul Singh Arora | Coordinator | Feb 2025–present | 


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
    * Send a calendly link to speakers to select a suitable slot
       * This also asks the speaker to provide a title, abstract, pre-print etc.
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
   * Broadly, responsible for ensuring the entire system runs fine.
   * Specific tasks
      * *Logistics.* Ensure the calendars are up to date, the venues are booked (and with help from the rest of the team when available), ensure the webpage and YouTube channel are up to date.
      * *Academic programme.* Review arXiv regularly and invite speakers.
* **GitHub maintainer.**
  * *Load.* About twenty minutes a week.
  * *Task.*
    * Calendar. (when requested) Get the abstract and title from the link. Leave the venue as TBA. Match the formatting.
    * GitHub page. (every Friday or Saturday)
       * Move "Upcoming" events that have already happened to "Past".
          * Add a YouTube link if it is already available (check the YouTube channel).
          * Otherwise, add a OneDrive link (check with the Coordinator if you don't have the link).
       * Move relevant events from "Pipeline" to "Upcoming".
       * Create new events as and when they are added on the public calendar.

   *Caveats.*
    * The formatting needs to be consistent (especially easy to forget: (in-person/online-only) etc.)
    * The links from Calendly can be a bit messy (they sometimes reroute from calendly instead; so be careful to copy the correct link)
    * Use TBA for venue when not known (and similarly for other fields)
    * Make sure ```<!-- SKIP_START -->``` is appropriately placed—ideally, only includes about three upcoming talks prior to this tag. 

* **YouTube maintainer.** 
  * *Load.* After familiarity with the tools, about twenty minutes (excluding export/upload/download) time.
  * *Task.*
     * Bare. Add the metadata to videos uploaded to our YouTube channel 
     * Video editing. Blur out everyone except the speaker and the slides. 
 

