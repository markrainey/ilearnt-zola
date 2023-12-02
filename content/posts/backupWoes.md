+++
title="Assumptions can be dangerous"
description="Sometimes we should not trust our assumptions."
date=2023-12-02
authors = ["Mark Rainey"]
[taxonomies]
categories=["technology","biography"]
tags=[]
+++

There is a quote "A backup is not a backup unless you have recently performed a restore from it"; I got to find this out the hard way.

<!-- more -->

One of the roles I had at my first job after university was to look after the nightly backups for the whole company. 

Back in the early 1990s there was no cloud backup or ability to copy to removable drives. It was performed using three tape drives running one after the other and took all night to run. It needed that many drives as there was too much to fit on one. There were hundreds of tapes that would rotated in a set plan and each night I would take the latest backups home so we had at least one set "off site" and place the previous ones back in the fire safe.

It was a boring process occasionally made interesting by a failed backup. If it failed we would just wait for the next night to run - which usually worked - as it would take too long to run during the day.

I had done selective restores of files for people who had accidentally deleted them but as storage was expensive I had never done a full restore of a drive. 

One day things didn't go quite as planned. All the drives were connected to a single server that the whole company used. On this day one of the drives failed. We had a network engineer who looked after these sort of things so it fell into his lap. Obviously as it would involve restoring data it would also need my input.

<img src="/posts/BackupWoes.png" title="Backup Woes" class="mid-image"></img><p></p>

The restore took a few hours to run so we informed everyone and they waited. Just before it was due to finish it failed - definitely something you don't want to happen. At this point we informed the management, who clearly were not very happy about the situation, and they decided everyone else may as well go home as it was already mid-afternoon. 

This left just the two of us to fix it.

The next three or four runs failed as well. By now it was late in the evening and things were looking very serious. If we could not restore the data then there was a good chance that it could be terminal for the company as key files and data would be lost.

To take our minds off this, I had my unicycle in the office (don't ask) and he had his skateboard so we spent some of the waiting time unicycling or skateboarding around all the corridors in the building. Every couple of hours we would check to see if the restore worked and if not we would kick off another one.

We gave the backup one last run and it finally worked and we managed to go home at about 1am - extremely relieved and very tired. If it hadn't worked I am really not sure what the next steps would have been.

Shortly after that I passed on the backup responsibilities to someone else and I never want to go through that again.

I learned to never assume that something is going to work - always test it. Assumptions can be dangerous.

