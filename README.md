# FEUP

Here are the most relevant projects I developed during my Masters in Electronics and Computers at FEUP.

Each project has a README with the appropriate course information.

For group projects I specify which part I authored.


Java-- compiler:
  I took this course as an extension to my masters. Since I knew nobody I joined a group of 3 other people, all of which eventually stopped attending the course leaving me to do the final project all by myself.

  Nonetheless the final project was complete with all features and almost all optimizations. A notable bug was "this" not being accepted as a variable, which unfortunately my tests didn't catch.

  The professors allowed me to fix this on the fly. This project was graded 20/20 due to its' completeness and the overall dificulty of the challenge.

Network Protocol:
  This course was done in conjunction with 40 other people divided into 4 teams!
  I was named leader of the Network Protocol team.

  The overall project involved creating wind sensors that, when deployed, could automatically perform discovery and routing via custom protocols and transmit the data all the way from each node, into a main one, which then passed it on to another team for parsing and visualization.

  I ended up doing the following tasks:
    Full design of all the versions of the "protocol stack";

    Development of the core protocol program;

    Development of a testsuite that simulated a live network, allowing noise to test recovery strategies;

    Separation of the packet [de]serialization functionality into work packages for my colleagues;

    Overall management of the work done and coordination with the the RF (antenna), WS (wind sensor) and data handling teams.

  Thanks to the testsuite, even though the antennas were only available mere days before delivery, the whole thing worked as intended.

Arduino window manager
  Fun little project to have a versatile window manager for Arduino with a small LCD
  My team member @rycostinha created pong which then could be set to play inside any of the dynamically generated windows


Arduino JTAG bitbang
  