+++
date = '2025-02-25T21:59:37Z'
draft = true
title = 'A pratical guide to de-googling'
+++

Google is a privacy hellscape, abusing your personal data to sell ads and train their AI, signing
contracts with dubious entities, as well as so many other issues. From a privacy, ecological and
ethical standpoint, it's in our best interest to move away and even boycott their services. But
they're entrenched in so many parts of our daily lives, that doing so can be terrifying. This is my
attempt at making it possible.

Special mention goes to [Janet Vertesi](https://hachyderm.io/@cyberlyra) and her work [The Cyber
Cleanse - Opt Out
Project](https://www.optoutproject.net/the-cyber-cleanse-take-back-your-digital-footprint/). I took
a bit of inspiration from there, and if you want a more thorough approach to fully getting rid not
only of Google but of all nefarious technology from all biggest major tech companies, and fully
clean your digital fingerprint, you should check her work instead. This article makes concessions
that she does not for the sake of practicality and ease for the end user, and its scope is much more
limited.

## Disclaimers

Google and a few other large companies have a de-facto monopoly in a big chunk of the internet, and
very few alternatives exist that won't impact your quality of life in some way. Migrating away isn’t
easy and requires compromises.

My target audience with this is people who use technology daily, but who might not have the
knowledge, time and patience to set up perfectly private alternatives, or who might not accept the
limitations of those alternatives. Any change is better than no change, so I’m suggesting what I
find reasonable, but not perfect, alternatives, and I’ll raise shortcomings if I know them. I’ll
often raise the companies that sell these alternatives and what’s their jurisdiction, if they are
for-profit or non-profit, so you have the information you need to make your decisions.

This is also a very subjective guide, I don’t know your use cases, everyone draws their line at
compromises differently, and I might not know better alternatives or some issues for some of the
services, so I'll happily accept suggestions and feedback 😄

This also isn’t an extensive step-by-step. This is an incomplete list of Google services you have to
migrate, and some alternatives that might work, with hints on how much effort you will need to do
for each one and what you can do to make it easier.

Now on to the migration!

## Google's reach

First, a sense of how much Google owns. All of these features are owned or controlled by Google
somehow:

* Google Search (duh)  
* Gmail, Google Calendar and Contacts  
* Chrome Browser  
* Almost all ads you see on the internet and in apps  
* Google Drive  
* Photos app (especially if you sync photos online)  
* Google Maps  
* Google Translate  
* All smartphones that aren't iPhones (yes, even Samsung, Huawei, and all other brands)  
* Youtube  
* and more (this is just the tip of the iceberg)

To avoid feeling overwhelmed, the tactic is going to be to tackle each one at a time. You pick an
item from the list, you go to the section talking about it, and you follow the steps to migrate
those. I’m also going to add little (subjective) indicators on each section to indicate if they are
easy 🟢, medium 🟡, hard 🔴 or downright impossible ⚫️to move away from. You can use these
indicators to choose a topic based on how ready you are to tackle.

## Search 🟢

The search engine is among the easiest things to change. A caveat is that most alternatives are just
making your search in Microsoft’s Bing and returning you its results. Indexing all the websites on
the internet is a long, slow and expensive process, and most alternatives try to work around that.

This means that unfortunately you're switching from a large tech company to another different large
tech company. It might still be worth it for the privacy preserving changes these 3rd parties do
though.

* [Qwant](https://www.qwant.com/) is a French search engine that has its own search index, it only
  falls back to Bing when it can’t find your search query.  
* [Ecosia](https://www.ecosia.org/) is a search engine by a German non-profit that uses Bing and
  plants trees for every search you make.  
* [DuckDuckGo](https://duckduckgo.com/) is an U.S. based search engine that uses Bing and anonymizes
  your searches so you can’t be tracked.

Switching in this case is easy. When you visit each one’s website, they will suggest you add their
search engine to your browser, and all searches from then on will be done on it!

If you see this and think “oh I’m not going to use Bing, it sucks!” well… yes, it does, [but
Google’s quality got much worse in the last few
years](https://gizmodo.com/google-search-results-are-getting-worse-study-finds-1851172943) ([and
Google did it on
purpose!](https://english.elpais.com/technology/2024-05-05/the-day-google-started-to-get-worse-we-are-getting-too-close-to-money.html)).
It got so much worse that by my subjective experience, Bing is roughly on-par with Google right now.

**Note:** there’s also Startpage, which anonymises Google searches, but given it uses Google under
the hood the same way others use Bing, I decided not to include it here.

## Browsers 🟢

Chrome is a Google browser! [Google is pushing for more tracking and more advertising in your
browser](https://www.malwarebytes.com/blog/news/2025/02/google-now-allows-digital-fingerprinting-of-its-users),
with harder opt outs, and [harming ad blockers on
purpose](https://arstechnica.com/gadgets/2023/11/google-chrome-will-limit-ad-blockers-starting-june-2024/).

Almost all other browsers out there actually use Chrome's code and adapt it a bit, so they run the
risk of suffering the same issues as Google's browser.

One of the bigger exceptions is [Firefox](https://www.mozilla.org/firefox/), which has a completely
independent source code maintained by the U.S. non-profit Mozilla Foundation (and for-profit Mozilla
Corporation, it's messy). While their parent company Mozilla has been struggling a bit to find a
sustainable business model and focusing on things like AI and privacy-preserving ads, which are
questionable decisions, I think their browser is still the most reasonable option to use.

Because Firefox might rarely not work with some webpages, having a backup browser is a reasonable
option. [Vivaldi](https://vivaldi.com/) is a Norwegian Chrome-based web browser, and while using a
Chrome based browser isn’t as good as using Firefox, it’s a good fallback when Firefox doesn’t work,
and it doesn’t send your data to Google (although you might have to tweak its privacy settings).

To migrate all of your data you will need to use a PC. On first use, Firefox will offer to import
all of your Chrome data from that PC. You can then use Firefox Sync to sync that data to your phone
as well.

**Note:** One browser to avoid is Brave. U.S. company Brave Software is owned by Brendan Eich, who
donated to foundations trying to lobby to make gay marriage illegal in the US, he is also a COVID
denialist. While pretending to be a private browser, it also has been found in scandal after scandal
breaking user's privacy, scamming the owners of websites, or both. You can see a thorough
description of the issues in [Stop using Brave
Browser](https://www.spacebar.news/stop-using-brave-browser/).

## Ads 🟢

You might be thinking, what do you mean, finding alternatives to ads?

Well, Google owns the biggest ad platform in the world, and because it uses the information from all
its products to target ads to you, [it effectively owns a monopoly in the ad
industry](https://www.theverge.com/2024/9/24/24253293/google-ad-tech-antitrust-trial-doj-case). It
is in their interest to spy on you to sell ads. Most ads you see on the internet or in apps will be
chosen by Google for you to see based on the spying they do on you.

Because of this, blocking ads is a necessity to preserve your privacy. The only reliable ad blocker
I can recommend is [uBlock Origin](https://ublockorigin.com/), maintained by independent developer
Raymond Hill. Most other ad blockers have deals with different ad providers to let them slip through
or replace ads from one provider with others that will pay them instead of the website owner.

To install uBlock Origin go to the developer’s website, and it’ll offer you an installation process
for your browser of choice.

Note that [Google forbid the technology used by uBlock Origin from being used in
Chrome](https://arstechnica.com/gadgets/2023/11/google-chrome-will-limit-ad-blockers-starting-june-2024/)
to prevent ad-blockers in Google Chrome from being as effective, and recently even [removed uBlock
Origin from the Chrome web
store](https://www.ghacks.net/2024/11/28/google-claims-that-ublock-origin-is-no-longer-available-for-chrome-but-that-is-not-true/),
so in the long term the only browser that will effectively block ads and tracking will be Firefox
and its derivatives.

## Password manager 🟢

You probably were saving passwords in Google Chrome, and might not want Google to have access to
that information. The easiest option is to use Firefox's password manager, it’ll be a similar
experience.

A different alternative might be to use [Bitwarden](https://bitwarden.com/). It's an U.S. owned
password manager that uses cryptography to ensure that the company cannot see the passwords you save
on it. Most modern password managers do this, but the source code for Bitwarden is open and has been
verified independently.

An alternative in Europe is [Proton Pass](https://proton.me/pass), owned by Swiss non-profit Proton
Foundation. It has the same type of privacy and the servers are fully located in Europe. Proton also
has replacements for other Google products described later on. There are some reservations about
Proton I will mention in the section about e-mail.

To migrate you might need to use a PC, but there you'll be able to export Chrome's passwords and
import them to your alternative of choice. Each provider has instructions on their website on how to
migrate. You can then install mobile apps to auto-fill on your phone and browser add-ons to auto
fill on your PC.

**Note:** Another tool to avoid is LastPass. For a long time it was widely used and famous, but they
[have suffered multiple security breaches since
2022](https://www.tomsguide.com/computing/password-managers/millions-stolen-from-lastpass-users-in-massive-hack-attack-what-you-need-to-know)
and are not a good alternative.

## E-mail 🔴 and calendar 🟡

This is where things start to get tricky. There are quite a few alternatives, but switching e-mail
providers requires creating a new e-mail and a long process of updating all online accounts and
informing all your contacts about the new e-mail. We'll get back to this in a moment.

First, some alternative providers:

* [Tuta](https://tuta.com/) is a German company that provides e-mail and calendar that use
  cryptography to ensure they cannot see the contents of your emails.  
* [Proton](https://proton.me/mail) is a Swiss non-profit that provides e-mail, calendar, drive,
  password manager and a few more services. Like Tuta, they also use cryptography to ensure the
  content of your e-mail is private to only you.  
* [Startmail](https://www.startmail.com/) is a Dutch based provider that provides an e-mail service.  
* [Mailfence](https://mailfence.com/) is a Belgian e-mail and calendar provider that also uses
  cryptography to make the e-mails private.

Creating an account should be the easy part. But that is not enough.

To make things easier, you can import all your existing e-mails from Gmail to either Tuta or Proton,
and you can set up a redirect so all emails from Gmail go to your new e-mail. Their websites have
instructions for each one on how to do that. This way you don't need to use both, you can rely on
your new e-mail to manage all e-mails.

The part that will take more time will be to go over your online accounts, one by one, and updating
it to use the new email, and to notify all your contacts as well. Take your time on this, don't rush
it. If you do it slowly over the course of a few weeks or months, you can get most of your accounts
moved to the new e-mail! You can update them one by one by checking your password manager for the
places you need to update.

All of these services also provide Calendars, and allow you to import your existing Google Calendars
with ease.

**Disclaimer about Proton:** in December 2024, Proton's CEO [Andy Yen praised the republican choice
of Gail Slater as Assistant Attorney General for the Antitrust
Division](https://x.com/andyyen/status/1864436449942110660) for being more inclined to take on big
tech monopolies (which is false). Proton quickly distanced itself from the CEO's position and from
being pro-republican.

This might discourage you from using it, understandably. I still keep this option here as
historically both Proton and Andy himself have both been shown to be critical of the republican
party and supportive of progressive causes. While his opinion here might have been distasteful, it
seems it does not reflect Proton’s and Andy’s overall views, and using their product is still a
better alternative than using Google. If there are other practical alternatives for e-mail,
calendar, password management and cloud file syncing you can vouch for, let me know so I can add
them 😁

## Drive 🟡

Google Drive allows you to sync files and photos over multiple different devices. It's quite
practical.

I could not find a lot of more independent alternatives, but what I did find was:

* [Proton](https://proton.me/drive), once again, has a service in this area.  
* [Mailfence](https://mailfence.com/) also provides a service in this area.  
* [Murena](https://murena.com/workspace/) is a French company that builds privacy-centered phones
  and also has a service in cloud storage.

Migrating your own files should be easy. Proton has instructions on automating the migration process
for their service, and copying things from Google Drive to your PC and from your PC to your new
alternative should be easy, if a bit slow.

Migrating shared files might be more complicated. If you can get away with sharing links, you can
inform people of the new link for the files they need from your cloud storage. If you need the other
person to also be able to modify the files, they will need to make an account there as well.

## Docs 🟡/🔴

Google Docs is a bit tricky to migrate away from…

If you don’t need the real time collaboration features, you can get away with using your drive space
from the previous section and a local document editor.

For PC, there’s [LibreOffice](https://libreoffice.org/), which is a fully featured office suite
maintained by an independent community and led by a German non-profit, whose source code is fully
available for people to review and modify.

For mobile there’s [OnlyOffice Documents](https://www.onlyoffice.com/download-desktop.aspx#mobile),
an open source application maintained by a Latvian company, and [Collabora
Office](https://www.collaboraonline.com/collabora-office-android-ios/), a product from a British
company, based on the LibreOffice code.

If you need the real time collaboration features, [OnlyOffice
Docs](https://www.onlyoffice.com/office-suite.aspx) seems the most fully featured of the options.
[Proton Drive](https://proton.me/drive) has limited support for written documents, but no
spreadsheet or presentation support. [Murena](https://murena.com/workspace/) also supports real time
collaboration, based on the OnlyOffice code.

The biggest caveat is that for people to do real time collaborative editing, they will need to make
an account in the platform you use, which might be a source of attrition.

## Photos 🟡

If you own a non-iPhone, you probably have an Android-based phone, and it probably has a Gallery
app. It might be the manufacturer's app, or it might be Google Photos, that neatly syncs photos over
the internet.

But Google scans your photos for criminal content (which has led to [false child abuse allegations
in the
past](https://www.eff.org/deeplinks/2022/08/googles-scans-private-photos-led-false-accusations-child-abuse))
and probably also uses them to train their AI models (they don't explicitly mention it, but they
also don't deny it).

The first thing to do is to disable Google's Backup and Sync by going to the app's settings. Then
you should install an alternative app.

Alternatives to the Google Photos app are [Aves
Gallery](https://play.google.com/store/apps/details?id=deckers.thibault.aves) and [Fossify
Gallery](https://play.google.com/store/apps/details?id=org.fossify.gallery). Both of these make
their source code available, and don't do anything to your photos besides showing them to you.

To replace the cloud sync, you can use one of the Drive alternatives from before. Proton Drive has
the ability to automatically sync photos to your Proton account, others should also have similar
features.

If you don't want your photos to touch the internet at all, you can use a tool to sync them to your
PC when you are on your home Wi-Fi. There's Danish [FolderSync](https://foldersync.io/) and German
[PhotoSync](https://www.photosync-app.com/). I have not used either product so I cannot vouch for
their quality. There also used to be the open source tool [Syncthing](https://syncthing.net/), but
[the Android app stopped being
maintained](https://github.com/syncthing/syncthing-android?tab=readme-ov-file#discontinued), and
until an easy to use alternative arises, I can't recommend it.

## Notes 🟢

Google Keep is very practical, but there are alternatives!

* [Joplin](https://joplinapp.org/) is a note taking app that also has an encrypted cloud syncing
  solution, maintained by British developer Laurent Cozic.  
* [Standard Notes](https://standardnotes.com/) is the app developed by Proton, that also encrypts
  and syncs your notes over multiple devices. Disclaimer, unlike all other products in the Proton
  family, this one requires a separate subscription for the paid features (but it does have a free
  tier).  
* [Obsidian](https://obsidian.md/) is a Canadian encrypted note app with cloud sync support.

Both Standard Notes and Obsidian provide ways to import notes from Google Keep, which should make
the transition easy and painless.

## Translation 🟢

Google Translate is ubiquitous, but there are quite a few reasonable alternatives.

If you just need webpages to be translated, Firefox supports [on-device
translation](https://www.mozilla.org/en-US/firefox/features/translate/). This means translations
happen on your PC, without ever going to the internet, and all of them are private. It’s easy to
use, it is private, and it works well!

To translate other snippets of text, German [DeepL](https://www.deepl.com/en/translator) is a set of
high quality translation models, with mobile apps you can install. Unlike Firefox’s on-device
translation, this will be sent to their servers to translate, but it is the most convenient high
quality option I could find for mobile at the time.

If you’re not afraid of software still under development and prefer on-device and open source
alternatives, you can try and download [RTranslator](https://github.com/niedev/RTranslator), an app
from independent developer Luca Martino.

## Maps 🟢/🟡

Finding a good alternative to Google Maps was a pain. To understand the scale of the difficulty, a
good alternative has to:

* Have accurate and up to date maps of all over the world.  
* Provide good driving and walking suggestions.  
* Have an extensive knowledge of the public transportation system of most cities to provide good
  public transport suggestions.

The first two requirements are already difficult to fulfil, but the 3rd one makes it almost
impossible!

Eventually I found a reasonable alternative that *seems* to check all the boxes, at least where I
live. [Here WeGo](https://www.here.com/products/wego) is a very complete maps application owned by
Dutch company Here. It is actually the successor to Nokia Maps! In my recent experience with it, it
was able to provide accurate information, good routes, both walking and in transportation, and the
mobile app feels polished and useful.

If you don’t prioritise public transportation so much and want to use a more community owned
alternative, [OpenStreetMap](https://www.openstreetmap.org/) is a community based map people can
contribute to like in Wikipedia, and it has multiple mobile applications, with the most famous and
most polished probably being Dutch [OsmAnd](https://osmand.net/). While it is an acceptable
alternative in some cases, its coverage of public transport is spottier and it might be a deal
breaker for some people, as it was for me.

## Android 🔴/⚫️

I have bad news, every single alternative has serious compromises here. You can switch to Apple‘s
iPhone, and accept giving your data to another big tech company, as well as to deal with their
walled garden.

You can use [EFF’s privacy guide for Android
phones](https://ssd.eff.org/module/how-to-get-to-know-android-privacy-and-security-settings), but it
has minimal impact and doesn’t actually prevent Google from spying on your phone.

If your phone allows it, you can switch to a Google-less flavour of Android, such as
[“e”](https://e.foundation/), [LineageOS](https://lineageos.org/), or others. But installing a new
OS on your phone is not an easy task, it might not be possible depending on your phone brand, and if
you do it there’s no guarantee that all functionality will continue working bug free.

Even worse, almost all Android apps, with very few exceptions, were forced in some way or another to
use Google specific code in them to be able to have the functionality they need. This is called the
Google Play Services, and it is used for location information, notifications, and many other things.
If one of the applications you use depends on this functionality and you try to use it in a
Google-less Android flavour, the application might be buggy or not even work at all.

And to make it even worse than all of this, many banking apps (and a few others) are now using a
feature in that code called the [Google Play Integrity
API](https://developer.android.com/google/play/integrity). This anti-feature checks if your phone’s
operating system was modified in some way. And if this feature finds out you are using a phone where
you installed an alternative flavour of Android on, it’ll fail the check and the app will refuse to
launch.

This is one of the worst user-hostile anti-features that causes a lock-in to Android as made by
Google, and prevents people from leaving it, resulting in a true monopoly.

While moving to Apple might not be much better, it might still be an improvement, and [their privacy
settings actually
work](https://ssd.eff.org/module/how-to-get-to-know-iphone-privacy-and-security-settings). If moving
to Apple is not an option, by principle or in practice, you can consider installing a Google-less
brand of Android on your phone if you don’t have apps that depend on Google features. The third
option is to get an old-school feature phone and put the smartphone in the drawer to let it gather
dust.

There’s no easy solution here, and until larger governments such as the EU or the US decide to
actually force Google to detangle Android from themselves, or a new alternative gains traction and
becomes a real alternative, it won’t get any better.

## Youtube ⚫️

And YouTube is not much better. Hosting a video site is expensive and migrating away depends on the
creators you follow having alternative sources for their videos somewhere else.

The best solution will be to check what each creator promotes. Some have paid tiers in Patreon where
you can see the videos before they’re released. Some have their own websites where you can subscribe
to see videos there directly. Some might be on alternative platforms such as Nebula.

Some people might also want to consider [PeerTube](https://joinpeertube.org/), which is a
decentralised alternative to YouTube developed by a French non-profit. Its user base is much smaller
than YouTube, and the number of creators there is minimal in comparison, but if you’re looking for
any videos in general, you might find what you’re looking for there.
[FediVideo](https://social.growyourown.services/@FediVideo) curates high quality instances and
accounts in PeerTube that you can follow.

## Cleanup and conclusion

After you finish each one of these migrations, you will probably want to go over each of the
services you just migrated, and clean up all the data you have there.

In an ideal world, you might get to a point where you are sure you deleted everything, and delete
your Google account altogether. That might take some time though.

But even if you don’t get to a point where you can delete your Google account altogether, reducing
your usage of them has an impact, it makes them less powerful and it has an influence, so any small
change and small cleanup you do is a win. Using very small steps at a time, you will be able to
slowly detangle Google from your life.

---

_The opinions expressed in this website are my own and may not reflect the views of my employer._