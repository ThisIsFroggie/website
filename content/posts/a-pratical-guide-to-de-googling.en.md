+++
date = '2025-03-04T13:20:00Z'
title = 'A pratical guide to de-googling'
+++

For quite a few years now Google has been having dubious and problematic behaviors. It's been spying
on users who opted out of data collection[^spying], secretly having contracts with the ICE[^ice] and
the IDF[^idf], to rigging the ads business with Meta to favor each other against other ad
sellers[^jedi], and so much more, not counting the enshittification[^enshittification] its products
have gone through.

It's in our best interest to move away from their services, but they're entrenched in so many parts
of our daily lives that it feels a herculean task to do so. If you use any of these, you are using a
Google product or within Google's control:

- Google search
- Gmail, Calendar, Docs and Drive
- "Sign-in with Google" buttons
- Chrome browser
- Any ads you see and interact with online
- Google Maps
- Google Translate
- All smartphones not made by Apple (even Samsung, Xiaomi, and all the other brands)
- YouTube
- and more

Migrating away isn't easy and requires compromises.

In this article, I'm going to suggest alternatives that are as easy to set up and use as I could
find. They may not be the most private, or they may not be the easiest, but I'll try to provide you
those caveats in each section when I'm aware, and color code them on difficulty. Pick sections of
the article as you feel like, and even if you can't migrate everything, doing the effort to migrate
some of the things already has a large impact on Google and on your privacy.

Special mention goes to [Janet Vertesi](https://hachyderm.io/@cyberlyra) and her work [The Cyber
Cleanse - Opt Out
Project](https://www.optoutproject.net/the-cyber-cleanse-take-back-your-digital-footprint/). I took
a bit of inspiration from there, and if you want a more thorough approach to fully getting rid of
products from all biggest major tech companies, you should check her work. I'm also going to give a
mention to [European Alternatives](https://european-alternatives.eu/), where I found a few of the
suggested alternatives I mention in this article, and to
[r/degoogle](https://www.reddit.com/r/degoogle/) on reddit, where so many of my searches for this
article fell on.

Now on to the migration!

## Search 🟢

The search engine is among the easiest things to change. A caveat is that most alternatives are just
making your search in Microsoft’s Bing and returning you its results. Indexing all the websites on
the internet is a long, slow and expensive process, and most alternatives try to work around that.

This means that unfortunately you're switching from a large tech company to another different large
tech company. It might still be worth it for the privacy preserving changes these 3rd parties do
though.

- [Qwant](https://www.qwant.com/) is a French search engine that has its own search index. It's also
  **the only search engine that I found that doesn't fully rely on Google or Bing under the hood**,
  having its own indexing. It only falls back to Bing when it doesn't have enough information for
  your search.
- [Ecosia](https://www.ecosia.org/) is a search engine by a German non-profit that uses Bing and
  plants trees for every search you make.
- [DuckDuckGo](https://duckduckgo.com/) is an U.S. based search engine that uses Bing and anonymizes
  your searches so you can’t be tracked.

![Screenshot of the Qwant home page](/img/posts/2025/03/qwant.png)

Switching in this case is easy. When you visit each one’s website, they will suggest you add their
search engine to your browser, and all searches from then on will be done on it!

If you see this and think “oh I’m not going to use Bing, it sucks!” well… yes, it does, but Google’s
quality got much worse in the last few years[^worse] (and Google did it on purpose[^purpose]). It
got so much worse that by my subjective experience, Bing is roughly on-par with Google right now.

**Note:** there’s also Startpage, which anonymizes Google searches, but given it uses Google under
the hood the same way others use Bing, I decided not to include it here.

## Browsers 🟢

Chrome is a Google browser! Google is pushing for more tracking and more advertising in your
browser[^fingerprint], with harder opt outs, and harming ad blockers on purpose[^adblocker].

Almost all other browsers out there actually use Chrome's code and adapt it a bit, so they run the
risk of suffering the same issues as Google's browser.

One of the bigger exceptions is [Firefox](https://www.mozilla.org/firefox/), which has a completely
independent source code maintained by the U.S. non-profit Mozilla Foundation (and for-profit Mozilla
Corporation, it's messy). While their parent company Mozilla has been struggling a bit to find a
sustainable business model and doing some questionable decisions, like removing their promise not to
sell user data[^firefoxpolicy], I think their browser is still the less bad option. There are more
private alternatives, but using them might cause websites to break too much.

![Screenshot of the Firefox web browser](/img/posts/2025/03/firefox-browser.png)

Because Firefox might rarely not work with some webpages, having a backup browser is a reasonable
option. [Vivaldi](https://vivaldi.com/) is a Norwegian Chrome-based web browser, and while using a
Chrome based browser isn’t as good as using Firefox, it’s a good fallback when Firefox doesn’t work,
and it doesn’t send your data to Google (although you might have to tweak its privacy settings).

To migrate all of your data [you will need to use a
PC](https://support.mozilla.org/en-US/kb/import-bookmarks-google-chrome). On first use, Firefox will
offer to import all of your Chrome data from that PC. You can then use Firefox Sync to sync that
data to your phone as well.

**Note:** One browser to avoid is Brave. U.S. company Brave Software is owned by Brendan Eich, who
donated to an anti-gay marriage proposition in California[^brendaneich], he is also a COVID
denialist. While pretending to be a private browser, it also has been found in scandal after scandal
breaking user's privacy, scamming the owners of websites, or both. You can see a thorough
description of the issues in [Stop using Brave
Browser](https://www.spacebar.news/stop-using-brave-browser/).

## Ads 🟢

You might be thinking, what do you mean, finding alternatives to ads?

Well, Google owns the biggest ad platform in the world, and because it uses the information from all
its products to target ads to you, it effectively owns a monopoly in the ad industry[^antitrust]. It
is in their interest to spy on you to sell ads. Most ads you see on the internet or in apps will be
chosen by Google for you to see based on the spying they do on you.

Because of this, blocking ads is a necessity to preserve your privacy. The only reliable ad blocker
I can recommend is [uBlock Origin](https://ublockorigin.com/), maintained by independent developer
Raymond Hill. Most other ad blockers have deals with different ad providers to let them slip through
or replace ads from one provider with others that will pay them instead of the website owner.

To install uBlock Origin go to the developer’s website, and it’ll offer you an installation process
for your browser of choice.

Note that Google forbid the technology used by uBlock Origin from being used in Chrome[^adblocker]
to prevent ad-blockers in Google Chrome from being as effective, and recently even removed uBlock
Origin from the Chrome web store[^ublock], so in the long term the only browser that will
effectively block ads and tracking will be Firefox and its derivatives.

## Password manager 🟢

You probably were saving passwords in Google Chrome, and might not want Google to have access to
that information. The easiest option is to use Firefox's password manager, it’ll be a similar
experience.

A different alternative might be to use [Bitwarden](https://bitwarden.com/). It's an U.S. owned
password manager that uses cryptography to ensure that the company cannot see the passwords you save
on it. This kind of feature, cryptography that allows you to save data online without the parent
company knowing what it is, is called **end-to-end encryption**. It's guarantees are better than any
company's pinky promise not to look at your data, and I will use this term from now on for other
services that do the same. Most modern password managers do this, but the source code for Bitwarden
is open and has been verified independently.

An alternative in Europe is [Proton Pass](https://proton.me/pass), owned by Swiss non-profit Proton
Foundation. It also had end-to-end encryption and the servers are fully located in Europe. Proton
also has replacements for other Google products described later on. There are some reservations
about Proton I will mention in the section about e-mail.

One important note about these services that use end-to-end encrpytion is that if you forget your
password to access them, you lose access to your data, in this case, **all your other passwords**.
Your password is used in the special mathematical formulas to keep your data safe, so it's critical
that you don't lose it. If you must, keep it in a piece of paper, in a vault, locked in a private
place.

To migrate you might need to use a PC, but there you'll be able to export Chrome's passwords and
import them to your alternative of choice. Each provider has instructions on their website on how to
migrate ([Firefox](https://support.mozilla.org/en-US/kb/import-login-data-file),
[Bitwarden](https://bitwarden.com/help/import-from-chrome/), [Proton
Pass](https://proton.me/support/pass-import-chrome)). You can then install their mobile apps to
auto-fill on your phone and browser add-ons to auto fill on your PC.

**Note:** Another tool to avoid is LastPass. For a long time it was widely used and famous, but they
have suffered multiple security breaches since 2022[^lastpassbreach] and are not a good alternative.

## E-mail 🔴 and calendar 🟡

This is where things start to get tricky. There are quite a few alternatives, but switching e-mail
providers requires creating a new e-mail and a long process of updating all online accounts and
informing all your contacts about the new e-mail. We'll get back to this in a moment.

First, some alternative providers:

- [Tuta](https://tuta.com/) is a German company that provides e-mail and calendar with end-to-end
  encryption on email contents and calendar events.
- [Proton](https://proton.me/mail) is a Swiss non-profit that provides e-mail, calendar, drive,
  password manager and a few more services. Like Tuta, they also have end-to-end encrpytion on email
  contents, calendar events, cloud synced files and password data.
- [Startmail](https://www.startmail.com/) is a Dutch based provider that provides an e-mail service.
- [Mailfence](https://mailfence.com/) is a Belgian e-mail and calendar provider with end-to-end
  encryption for email contents.

Creating an account should be the easy part. But that is not enough.

To make things easier, you can import all your existing e-mails from Gmail to either
[Tuta](https://tuta.com/support#mail-import) or
[Proton](https://proton.me/support/switch-from-gmail-to-proton), and you can set up a redirect so
all emails from Gmail go to your new e-mail ([Tuta](https://tuta.com/support#how-to-forward),
[Proton](https://proton.me/support/automatic-forwarding-gmail)). Their websites have instructions
for each one on how to do that. This way you don't need to use both Gmail and the new provider, you
can rely on your new provider to manage all e-mails.

The part that will take more time will be to go over your online accounts, one by one, and updating
it to use the new email, and to notify all your contacts as well. Take your time on this, don't rush
it. If you do it slowly over the course of a few weeks or months, you can get most of your accounts
moved to the new e-mail! You can update them one by one by checking your password manager for the
places you need to update.

All of these services also provide Calendars, and allow you to import your existing Google Calendars
with ease.

**Disclaimer about Proton:** in December 2024, Proton's CEO Andy Yen praised the republican choice
of Gail Slater as Assistant Attorney General for the Antitrust Division[^andyyen] for being more
inclined to take on big tech monopolies (which is false). Proton quickly distanced itself from the
CEO's position and from being pro-republican. Although historically it seems that Andy Yen and
Proton's position about this subject does not reflect their overall position on human rights, this
might still discourage you from using it. If there are other practical alternatives for e-mail,
calendar, password management and cloud file syncing you can vouch for, let me know so I can add
them 😁

## Sign-in with Google 🟡

You've seen those buttons on websites, next to the login box, that say "Sign in with Google" or
Meta, or other big providers. To move away from Google, you also need to replace those sign-ins with
alternative approaches.

To find what websites do you sign in with Google, follow go to your Google Account > Security >
[Your connections to third-party apps & services](https://myaccount.google.com/connections). Here
you should have a list of all websites.

![Screenshot of the Google's page on third party apps](/img/posts/2025/03/3rd-party-apps.png)

Now, for each one, you should visit the website, go to its settings, and find a way to set a new
e-mail and password (which you can save in your new password manager), and when that is done, unlink
it from Google.

Each website will be unique, some will be easier, some will be much trickier to take care of. But
although it might be a long process, it should not be impossible. When you are done, all of those
websites should use your new email, have a unique password saved in your password manager, and no
longer use Google to sign in.

## Drive 🟡

Google Drive allows you to sync files and photos over multiple different devices. It's quite
practical.

I could not find a lot of more independent alternatives, but what I did find was:

- [Proton](https://proton.me/drive), once again, has a service in this area with end-to-end
  encrypted documents.
- [Mailfence](https://mailfence.com/) also provides a service in this area.
- ~~[Murena](https://murena.com/workspace/) is a French company that builds privacy-centered phones
  and also has a service in cloud storage.~~ It seems their cloud storage is not working at the
  moment.

Migrating your own files should be easy. [Proton has instructions on automating the migration
process for their service](https://proton.me/support/import-files-google-drive), and copying things
from Google Drive to your PC and from your PC to your new alternative should be easy, if a bit slow.

Migrating shared files might be more complicated. If you can get away with sharing links, you can
inform people of the new link for the files they need from your cloud storage. If you need the other
person to also be able to modify the files, they will need to make an account there as well.

## Docs 🟡/🔴

Google Docs is a bit tricky to migrate away from…

If you don’t need the real time collaboration features, you can get away with using your drive space
from the previous section and a local document editor.

One option is [OnlyOffice Documents](https://www.onlyoffice.com/download-desktop.aspx), a
Latvian-based open-source office suite available for both PC and mobile.

Alternatively, there is [LibreOffice](https://libreoffice.org/) for PC, which is a fully featured
open-source office suite maintained by an independent community and led by a German non-profit.
And [Collabora Office](https://www.collaboraonline.com/collabora-office-android-ios/) for mobile, a
product from a British company, based on the LibreOffice code.

If you need the real time collaboration features, [OnlyOffice
Docs](https://www.onlyoffice.com/office-suite.aspx) seems the most fully featured of the
options. [Proton Drive](https://proton.me/drive) has limited support for written documents, but no
spreadsheet or presentation support. [Murena](https://murena.com/workspace/) also supports real time
collaboration, based on the OnlyOffice code.

The biggest caveat is that for people to do real time collaborative editing, they will need to make
an account in the platform you use, which might be a source of attrition. If you have existing
documents or receive documents owned by other people, you might not have a choice but to use Google
for those specific documents.

## Photos 🟡

If you own a non-iPhone, you probably have an Android-based phone, and it probably has a Gallery
app. It might be the manufacturer's app, or it might be Google Photos, that neatly syncs photos over
the internet.

But Google scans your photos for criminal content (which has led to false child abuse allegations in
the past[^childabuse]) and possibly also uses them to train their AI models (they don't explicitly
mention it, but they also don't deny it, and it wouldn't be the first time Google was caught using
data without permission[^spying]).

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
PC when you are on your home Wi-Fi. There's Danish [FolderSync](https://foldersync.io/) and
German [PhotoSync](https://www.photosync-app.com/). I have not used either product so I cannot vouch
for their quality. There also used to be the open source tool [Syncthing](https://syncthing.net/),
but [the Android app stopped being
maintained](https://github.com/syncthing/syncthing-android?tab=readme-ov-file#discontinued). If an
alternative syncthing app for Android appears, I will update this article.

## Notes 🟢

Google Keep is very practical, but there are alternatives!

- [Joplin](https://joplinapp.org/) is a note taking app with end-to-end encryption, maintained by
  British developer Laurent Cozic.
- [Standard Notes](https://standardnotes.com/) is the app developed by Proton with end-to-end
  encryption. Disclaimer, unlike all other products in the Proton family, this one requires a
  separate subscription for the paid features (but it does have a free tier).
- [Obsidian](https://obsidian.md/) is a Canadian end-to-end encrypted note app with cloud sync
  support.

Both Standard Notes and Obsidian provide ways to import notes from Google Keep ([Standard
Notes](https://standardnotes.com/help/35/how-can-i-import-my-notes-from-google-keep),
[Obsidian](https://help.obsidian.md/import/google-keep)).

## Translation 🟢

Google Translate is ubiquitous, but there are quite a few reasonable alternatives.

If you just need webpages to be translated, Firefox supports [on-device
translation](https://www.mozilla.org/en-US/firefox/features/translate/). This means translations
happen on your PC, without ever going to the internet, and all of them are private. It’s easy to
use, it is private, and it works well!

To translate other snippets of text, German-owned [DeepL](https://www.deepl.com/en/translator) is a
set of high quality translation models, with mobile apps you can install. Unlike Firefox’s on-device
translation, this will be sent to their servers to translate, but it is the most convenient high
quality option I could find for mobile at the time.

If you’re not afraid of software still under development and prefer on-device and open source
alternatives, you can try and download [RTranslator](https://github.com/niedev/RTranslator), an app
from independent developer Luca Martino.

![Screenshot of the Deepl service](/img/posts/2025/03/deepl.png)

## Maps 🟡/🔴

Finding a good alternative to Google Maps was a pain. To understand the scale of the difficulty, a
good alternative has to:

- Have accurate and up to date maps of all over the world.
- Provide good driving and walking suggestions.
- Have an extensive knowledge of the public transportation system of most cities to provide good
  public transport suggestions.

The first two requirements are already difficult to fulfil, but the 3rd one makes it almost
impossible!

Eventually I found a reasonable alternative that *seems* to check all the boxes, at least where I
live. [HERE WeGo](https://www.here.com/products/wego) is a very complete maps application owned by
Dutch company HERE. It is actually the successor to Nokia Maps! In my recent experience with it, it
was able to provide accurate information, good routes, both walking and in transportation, and the
mobile app feels polished and useful.

If you don’t prioritize public transportation so much and want to use a more community owned
alternative, [OpenStreetMap](https://www.openstreetmap.org/) is a community based map people can
contribute to like in Wikipedia, and it has multiple mobile applications, with the most famous and
most polished probably being Dutch [OsmAnd](https://osmand.net/). While it is an acceptable
alternative in some cases, its coverage of public transport is spottier and it might be a deal
breaker for some people, as it was for me.

As far as I was able to check, I didn't find a way to import Google Maps lists to none of the
options here. In addition to that, the information on the various places and businesses might not be
as complete as in Google Maps.

## Android 🔴/⚫️

I have bad news, every single alternative has serious compromises here. You can switch to Apple‘s
iPhone, and accept giving your data to another big tech company, as well as to deal with their
walled garden.

You can use [EFF’s privacy guide for Android
phones](https://ssd.eff.org/module/how-to-get-to-know-android-privacy-and-security-settings), but it
has minimal impact and doesn’t actually prevent Google from spying on your phone.

If your phone allows it, you can switch to a Google-less flavour of Android, such
as [“e”](https://e.foundation/), [LineageOS](https://lineageos.org/), or others. But installing a
new OS on your phone is not an easy task, it might not be possible depending on your phone brand,
and if you do it there’s no guarantee that all functionality will continue working bug free.

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
any videos in general, you might find what you’re looking for
there. [FediVideo](https://social.growyourown.services/@FediVideo) curates high quality instances
and accounts in PeerTube that you can follow.

## Cleanup and conclusion

After you finish each one of these migrations, you will probably want to go over each of the
services you just migrated, and clean up all the data you have there.

In an ideal world, you might get to a point where you are sure you deleted everything, and delete
your Google account altogether. In reality, you might take a lot longer, or you might have blockers
that prevent you from migrating 100%. That's okay though, any changes to your habits where you use
less services or use them less often are an improvement. Even those small changes have an impact and
reduce Google's revenue and influence.

And if you feel inspired, you should continue detangling your life from other big tech. Look at [The
Cyber Cleanse](https://www.optoutproject.net/the-cyber-cleanse-take-back-your-digital-footprint/)
for an overall guide, consider moving away from Microsoft, Amazon and Meta services and products.
Look for privacy preserving alternatives to the tools and services you use, and take back control of
your life.

[^spying]: Jon Brodkin, "Google loses in court, faces trial for collecting data on users who opted
    out," Ars Technica, January 9, 2025,
    https://arstechnica.com/tech-policy/2025/01/google-loses-in-court-faces-trial-for-collecting-data-on-users-who-opted-out/
[^ice]: Caroline Haskins, "Google, Amazon, and Microsoft have taken advantage of a commonly used but
    little-known tool to quietly enter dozens of contracts with ICE and CBP," Business Insider,
    October 4, 2021,
    https://www.businessinsider.com/google-amazon-microsoft-ice-cbp-third-party-contracts-cloud-2021-10
[^idf]: Billy Perrigo, "Exclusive: Google Contract Shows Deal With Israel Defense Ministry," TIME,
    April 12, 2024, https://time.com/6966102/google-contract-israel-defense-ministry-gaza-war/
[^jedi]: Natasha Lomas, "‘Jedi Blue’ ad deal between Google and Facebook sparks new antitrust probes
    in EU and UK," TechCrunch, March 11, 2022,
    https://techcrunch.com/2022/03/11/google-meta-jedi-blue-eu-uk-antitrust-probes/
[^enshittification]: Cory Doctorow, "How monopoly enshittified Amazon," Nov 28, 2022,
    https://doctorow.medium.com/how-monopoly-enshittified-amazon-83f42a585c3c
[^worse]: Thomas Germain, "You’re Not Imagining It: Google Search Results Are Getting Worse, Study
    Finds," Gizmodo, January 17, 2024,
    https://gizmodo.com/google-search-results-are-getting-worse-study-finds-1851172943
[^purpose]: Jordi Pérez Colomé, "The day Google started to get worse: ‘We are getting too close to
    money’," El País, May 5, 2024,
    https://english.elpais.com/technology/2024-05-05/the-day-google-started-to-get-worse-we-are-getting-too-close-to-money.html
[^fingerprint]: Pieter Arntz, "Google now allows digital fingerprinting of its users," MalwareBytes,
    Feburary 19, 2025,
    https://www.malwarebytes.com/blog/news/2025/02/google-now-allows-digital-fingerprinting-of-its-users
[^adblocker]: Ron Amadeo, "Google Chrome will limit ad blockers starting June 2024," Ars Technica,
    November 21, 2023,
    https://arstechnica.com/gadgets/2023/11/google-chrome-will-limit-ad-blockers-starting-june-2024/
[^firefoxpolicy]: Jon Brodkin, "Firefox deletes promise to never sell personal data, asks users not
    to panic," Ars Technica, February 28, 2025,
    https://arstechnica.com/tech-policy/2025/02/firefox-deletes-promise-to-never-sell-personal-data-asks-users-not-to-panic/
[^brendaneich]: Casey Newton, "Mozilla CEO resigns amid controversy over donation to anti-gay
    marriage proposition," The Verge, April 3, 2014,
    https://www.theverge.com/2014/4/3/5578984/mozilla-ceo-resigns-amid-controversy-over-donation-to-anti-gay
[^antitrust]: Lauren Feiner, "How Google made the ad tech industry revolve around itself," The
    Verge, Spetember 24, 2024,
    https://www.theverge.com/2024/9/24/24253293/google-ad-tech-antitrust-trial-doj-case
[^ublock]: Martin Brinkmann, "Google claims that uBlock Origin is no longer available for Chrome:
    but that is not true," ghacks.net, November 28, 2024,
    https://www.ghacks.net/2024/11/28/google-claims-that-ublock-origin-is-no-longer-available-for-chrome-but-that-is-not-true/
[^lastpassbreach]: Anthony Spadafora, "Millions stolen from LastPass users in massive attack — what
    you need to know," Tom's Guide, December 18, 2024,
    https://www.tomsguide.com/computing/password-managers/millions-stolen-from-lastpass-users-in-massive-hack-attack-what-you-need-to-know
[^andyyen]: Andy Yen (@andyyen), "[Screenshot of Donald Trump's post announcing Gail Slater as
    Assistant Attourney General for the Antitrust Division at the Department of Justice] Great pick
    by @realDonaldTrump. 10 years ago, Republicans were the party of big business and Dems stood for
    the little guys, but today the tables have completely turned. People forget that the current
    antitrust actions against Big Tech were started under the first Trump admin.", Twitter (now X),
    December 4, 2024, https://x.com/andyyen/status/1864436449942110660
[^childabuse]: Joe Mullin, "Google’s Scans of Private Photos Led to False Accusations of Child
    Abuse", Electronic Frontier Foundation, August 22, 2022,
    https://www.eff.org/deeplinks/2022/08/googles-scans-private-photos-led-false-accusations-child-abuse