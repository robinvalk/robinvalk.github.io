---
title: "Family Backup Solution"
date: 2022-11-29T22:34:17+01:00
draft: true
---

When I was a child some important family pictures got lost because of a non-existing backup solution. Since my dad is making backups but still it isn't a solid thought through backup solution.

In this article I describe a little more what happened, what options I considered and how I plan to tackle this problem for my parents, siblings and myself using the 3-2-1 backup strategy.

I hope this article inspires to think about your backup strategy and maybe even pushes you into taking the necessary actions to also be confident about not losing any data.

## Introduction

Just like many other families my dad bought a digital camera once they became commonly available and affordable. Without thinking too much of it, like almost everyone was doing at the time, he kept the pictures on the family computer in the living room. Somehow, some day, the hard drive disk got corrupted. The exact reason I don't really know unfortunately.

// > I asked my parents what happened. It was a virus that corrupted most files on the disk.

I do know that there was no backup. Because there was no copy the data on this drive got lost, most valuable were the family pictures. He did try to recover the data with some tools. I tried the same a couple of years ago but also I didn't have any luck getting something useful from the disk. He started making backups of the computed on DVDs, later he bought random external hard drives of different brands, ages and capacity to make backups on.

There was and still is no plan of what drive is a copy of what, no automated backups, no schedule of when a backup should be created and there is no offsite backup. My dad did the best he knew an what he thought was necessary. Some version of the same setup is now the case for my siblings and even myself. Next to the external hard drives we also use some cloud services as Google Drive, OneDrive or iCloud.

This scenario is probably recognizable by quite some people. As I'm now the nerd in the family I want to setup a solution for everyone that's a more thought through and automated. What if the house burns down, you spill water over your laptop or your phone gets stolen or your PC gets infected with malware? Currently for a lot of my family members at least one of these things would result in a loss of data.

## 3-2-1 backups

With the realization this needs to change I started searching for recommendations and options. Doing so you quickly come to the topic of 3-2-1 backup strategy. This means you have at least three copies of your data, two locally (on-site) on different media (devices) and at least one off-site. If setup correctly you will not loose data in any of the example events I wrote above.

The simplest setup of the 3-2-1 backup strategy I came up with looks as follows: The first copy is your laptop, phone or PC. The second copy can be an external hard drive. The off-site copy can be a snapshot of the external hard drive on another hard drive that you bring to a relative's house.

These external hard drives are an affordable way to start. It's cheap to purchase and easy to setup. MacOS supports making a backup to an external drive when you connect it to your mac device for instance. But how can you update the off-site copy? You'll have to bring the drive home, mirror it based on the on-site backup drive and bring it back to the off-site location.

I know for sure I won't keep these disks up to date with recent backups. I'm pretty sure you wouldn't either. We need automation!

## Seconds local copy

Everyone has the initial first copy of the data they don't want to loose. It's stored on our phones, laptops or maybe even the smart fridge ;). But if your laptop dies, how will you recover the documents and continue your work? How will you get back the pictures on your phones that don't fit in iCloud? What if you accidentally permanently deleted the wrong file and you quickly want it back? That's were the second local copy on a different medium comes in.

### Options

#### Sync services

Using a second copy you can quickly access those files that otherwise would be gone. A lot of people use Google Drive, OneDrive, Dropbox, etc as their second copy. Sync services like these can resolve some problems, but they also have a few problems themselves:
- They are limited in size, this discourages its use. When you only have a few gigabytes to use you will not store the family pictures there. If you want more data you pay for the next tiers which gets quite expensive very quickly
- Not all of the sync services have a history feature, this means if you delete a file the deletion is synced everywhere and cannot be recovered
- When randsomeware or malware encrypts the files in your dropbox folder, that file will now be encrypted on the other locations as well.
- The data isn't self owned. Their policies can and will change which greatly impacts you. Google initiated Google Photos as an unlimited storage for all your pictures. Once they had everyone locked into their ecosystem they changed their policy whereby now only your allowed to store 15 gigabytes for free
- Restoring the data is limited by your internet speed, which is for a lot of people an issue still. It is missing the "local" part for a second local copy.

Don't get me wrong, sync services are great to use. But they don't replace backups.

#### External hard drive

An external hard drive can work if you can force yourself to do all the manual work required. Periodically plugging it in to make a full backup of your machine. Unfortunately this solution also doesn't work well with your phones pictures. You can move those to your laptop before backing up your laptop. But again, this requires a lot of planning and commitment. This will discourage making backups.

#### Network Attached Storage (NAS)

A NAS doesn't have most of the issues an external hard drive has. It connects to your network so your machines can automatically create a backup to it on a schedule!

The popular NAS ecosystems come with lots of apps and tools to backup your data. On your phone you can install their app to backup your pictures and videos to your NAS. It's basically your privately owned iCloud or Google Photos. For your laptop you can use the NAS ecosystem's applications or you can configure your laptop to do a full backup with time machine on MacOS or with Backups and Restore on Windows if you desire to do so.

If you do wish to continue using cloud sync services like Google Drive etc, you can setup your NAS to backup those to your NAS. But I would use the NAS itself as a sync service so you can save some money by cancelling third party subscriptions.

As the NAS is local it will not be limited by your internet speed but your internet network's speed. Often this is higher then the internet connection you have.

The last benefit of a NAS is the possibility for redundancy. The cheapest options already allow you to put in two hard drives. The NAS will allow you to setup redundancy so you can loose a drive but still have all the data.

#### Conclusion

It's no surprise that I am opting for a NAS setup:
- I will own the data;
- It is local;
- It will be faster;
- It brings many features.

The features supported on a NAS are really great nowadays. Synology Photos has support for facial recognition and can automatically make photo albums for persons. You can have Word and Excel like environments where you can collaborate live with other people in the documents, just like Google Docs or Office 364. The NAS itself can be backed-up to a cloud storage service or to another NAS device off-site.

## Third off-site copy

Still need off-site backup in case of house fire

### Cloud Storage Providers

- Expensive, cost didn't go down over the years.
- Slow to restore

### Another NAS

- Self owned
- Other family member can use the NAS as a NAS and backup to me.

- Family members can use other NAS
- Shared storage
- Doesn't only benefit me
- I'll manage the configuration
    - What if I die?
- Self owned!

## Conclusion
