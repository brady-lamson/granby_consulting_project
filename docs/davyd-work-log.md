- 2026-02-13 Friday (1 hour)
    - Had initial call with Chris Michalowski at 10:00am. Had recap with Brady after the call.
    - Chris sent documents related to the project shortly after the call.

- 2026-02-17 Tuesday (3 hours)
    - Met with Brady in person 2:00-5:00pm.
    - Initial look at the two documents Chris had sent over last week. These were the SGM engineering form report and the CDOT report.
    - Understood the relevant geography and streets by reading the documents and looking up streets in maps. Agate St is what highway 40 becomes once it enters downtown Granby. 4th, 5th, 6th, and Mesa St intersect Agate from the north.
    - Understood the motivations for each report. CDOT document was centered more on vehicle congenstion in 4th-6th street. SGM report was focused on implementing potential safety measures around the Agate and Mesa intersection, which is close to the Granby schools.
    - Understood the basic premise of simulation modeling done in the CDOT document (Synchro and SimTraffic). Initial vehicle flow rate parameters are observed from real life, and are then inputed into simulation software to determine other important values like the average wait time for a vehicle at an intersection. Looked into some underlying math of the program and realized its baed on concepts I had covered in my Probabilistic Modeling class from Fall 2024. Things like M/M/1 queues, Poisson arrival times, and exponential gaps between arrivals.
    - created my work log (davyd-work-log.md) and also a folder for notes that I will take like my statistical concepts document, and other isolated topics I summarize as I go. I decided that the notes will be in the form of pdf documents that I will create in google docs and then upload to the github repo. This will make it easier to format and add screenshots.

- 2026-02-24 Tuesday (4 hours)
    - Met with Brady in person.
    - Check in with Erin over zoom. He gave us some clarity about how we should focus on the traffic/pedestrian volumes visualization first because it is something to show the client and also will give us additional ideas as we go. 
    - went over the SGM 4-6th street traffic simulation tables. We made progress on understanding the underlying data and
    tossed around ideas on what data to start extracting into data structures for visualizations.
    - Brady looked into the Synchro software with a youtube tutorial. It was very helpful for understanding the variables
    produced from simulation
    - figured out how to properly manage github. I have to clone instead of make forks like ive been doing previously...

- 2026-02-24 Thursday (30 minutes)
    - Met with Brady in person before consulting class
    - Briefly discussed some ideas about the simulation data and next steps.
    - Still waiting on Chris's response about where the traffic safety measures actually being built.

-2026-03-01 Sunday (5 hours)
    - Chris had answered on Friday and said that there are 2 measures being implemented. Bulbouts will be on Mesa intersection (for pedestrain safety) and a signal on 4-6th area. Our job is to quantify reduction in pedestrian risk
    and justify the costs of those meaures. He shared the expense estimates too.
    - I looked into how to quantify pedestrian risk (docs/davyd_notes/ways_to_quantify_pedestrain_risk.txt). Learned that 
    we can either quantify direct crash rate before and after those measures with a pre made regression model, or simulate
    "conflicts" which are much more common than direct crashes and could be more informative.
    - I learned there is a free modeling software combination to simulate vehicle paths (SUMO) and then quantify conflict (SSAM). 
    - Actually crudely implemented the crash rate given our set of parameters in the Mesa Area. Had to find the right .xlsx
    document and udnerstand the variables in it. We are working with the suburban version because of the 5 lane road, whcih is considered bigger than the traditional rural roads src/HSM_CPM_UrbanSuburbanArterials_v3.2.xlsx
    - NEXT STEPS:
        - Fully understand the .xlsx sheet and input the correct variables from our data. Figure out what coefficeints to multiply by to find the crash rate after bulbouts are installed. Do same for 4-6th street?
        - Discuss and think about whether the conflict simulation approach is worth implementing.
        - Get the McDowel report from Chris, and any other possible data he may have.
        - convert .txt notes into .docx and then resolve merge conflicts on github


