# How to contribute | Logistics

This page outlines how the system is structured, followed by a description of the various roles. But first, a huge thank you to our new contributors. 

If you're interested in contributing to this effort, please feel free to [write to us](atul.singh.arora@gmail.com). 

## Contributors 

| Name | Role | Contribution period | 
| - | - | - |
| Arnab Ghorui | GitHub maintainer | Aug 2025–present | 
| Himanshu | YouTube maintainer | May 2025–present | 
| Niranjan | YouTube maintainer | Oct 2025–present | 
| Atul Singh Arora | Coordinator | Feb 2025–present | 
| Sreyas (Aryaman reserve) | (in-person) Equipment Coordinator | Oct 2025–present |
| Prerna (Niranjan reserve) | Quantum Talks Coordinator | Oct 2025–present | 


## Video Editing Contributions (post Oct, 2025)

This is for YouTube maintainers. Please update the following (descending order) and send a pull-request when you edit a video for a speaker.

NB. These records start October, 2025 onwards. Prior to this, Himanshu edited most videos.

| Speaker | Edited By | Event held on |
| - | - | - |
| Victor Albert | Atul | 19 February, 2026 |
| Alexander Schmidhuber | Atul | 18 February, 2026 |
| Victor Albert | Himanshu and Atul | 17 February, 2026 |
| Pavithran Iyer | Himanshu and Atul | 13 February, 2026 |
| Victor Albert | Himanshu and Atul | 12 February, 2026 |
| Aparna Gupte | Himanshu and Atul | 11 February, 2026 |
| Sreenath K Manikandan | Himanshu and Atul | 6 February, 2026 |
| Suvrat Raju | Atul | 23 January, 2026 | 
| Shota Yamada | Atul | 21 January, 2026 |
| Naresh Goud Boddu | Atul | 20 January, 2026 |
| Rukmani Bai | Atul | 19 January, 2026 |
| Marek Gluza | Niranjan and Atul | 13 January, 2026 | 
| Mohit Dilipbhai Rohida | Niranjan | 12 January, 2026 |
| Soumik Ghosh | Atul | 8 January, 2026 |
| Pranab Sen | Himanshu | 22 December, 2026 |
| Sreyas Saminathan | Niranjan | 11 December, 2025 |
| Xiangling Xu | Himanshu | 10 December, 2025 | 
| Sayantan Chakraborty | Himanshu | 9 December, 2025 |
| Alex Cojocaru | Niranjan | 8 December, 2025 | 
| Pedro Barrios | Himanshu | 3 December , 2025 |
| Pratibha Hegde | Niranjan | 21 November, 2025 |
| Kushagra Garg | Himanshu | 21 November, 2025 |
| Kunal Marwaha | Himanshu | 19 November, 2025 |
| Sreetama Das | Niranjan | 13 November, 2025 |
| Rajamani Vijayaraghavan | Himanshu | 11 November, 2025 |
| Riddhi Ghosal | Sreyas and Niranjan | 4 November, 2025 |  
| Timothée Hoffreumon | Niranjan | 3 November, 2025 |
| Tanuj Khattar | Himanshu | 28 October, 2025 |
| Zhiyan Ding | Himanshu | 27 October, 2025 |
| Indranil Chakraborty | Himanshu | 18 October, 2025 |
| Sebastian Zur | Himanshu | 15 October, 2025 | 
| Dominik Leichtle | Himanshu | 14 October, 2025 |

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
* **Quantum Talks Coordinator.**
   * Broadly, responsible for ensuring internal members present weekly.
   * Specific tasks
      * Maintaining a spreadsheet with all the members and the tentative week in which they intend to present.
      * Ensuring that they schedule a talk on the system at least a week prior (and at most two weeks prior) to their target presentation week.

   *Calendly tips.*
  * *Sending invites?* While the system should automatically prevent users from scheduling multiple events on the same day, it sometimes fails—since we have to allow events to be added manually. So, when you ask people to book a slot using Calendly, please also ask them to double check that the slot they are picking does not have an event already in the calendar on our [webpage](https://quantum-meets.github.io/). Saves us time.
  * *The speaker needs to reschedule?* To reschedule, it is often easier to ask them to use the “reschedule link”. This link sits at the bottom of the description of the event they create (which appears on our webpage’s calendar as well). If they are unable to find this link, you can copy paste it from the event and share it with them. That way, nobody has to delete events etc.
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
 
* **(in-person) Equipment Coordinator.**
  * *Load.* About thirty five minutes per seminar
  * *Task.*
     * Day before the event. Make sure the bluetooth speaker/mic and related equipment is charged. The laser pointer uses external batteries, so replace them if needed. Ensure we have a spare set.
     * Thirty minutes prior to the event. Arrive at the venue, setup the camera, the projector and try to use ethernet for a stable connection. Join on Teams and do a quick audio/video test. Inform the speaker to be careful to **not shine the laser into the camera**. You would be surprised how easy it is to do that accidentally.
     * During the event. Enjoy it! Occassionally make sure Teams is working fine—especially that the talk is getting recorded (unless the speaker doesn't want it recorded). And that the speaker is on "spotlight". Makes it much easier to edit videos later.
     * Equipment. If you are not going to be available for upcoming events, be sure to hand over the equipment to me or to another volunteer, before you leave. There is a checklist in the box, please use it to ensure we don't lose anything. 
