---
title: "My Blog Setup"
date: 2022-11-06T19:01:33+01:00
draft: false
---

Let me start my blog with a meta topic, my blog setup itself. Inspired by some blogs of fellow nerds I wanted to keep the setup simple.

As far as I can tell the requirements for owning a blog are straightforward. You need a blogging platform, hosting and some content. My personal preference goes to a simplistic design that focusses on the content. If you are reading this post you can tell that even I managed to get a blog up and running. You can use this post to inspire yourself to create your own. Don't expect this to be a tutorial or to have a real conclusion at the end. It will just give some insights on my decisions and it links you to some resources that will allow you to get your own blog started, if you desire to do so ofcourse.


## Blogging platform

### Requirements

I want to keep it simple. I don't care about an admin interface, automatic posting to social media, a hotmap on how my users interact with the website or any other features that don't really matter and half the time invade our privacy anyways. I want it to be managed by myself and not use a system like Medium.

Markdown is my prefered format for writing so the tool should support that. It should be easy and cheap to host because I have enough expensive and time consuming hobbies already. _FYI: bugfixing a blog is not a hobby I'd like to pick up on._ Another important requirement for me is that it comes with pre-made themes so I hardly have to touch the HTML and CSS. Last but not least, it should be free!

- Self managed
- Simple create and maintain
- Markdown support
- Easy and cheap (if not free) to host
- Pre-made themes
- Free to use

### Options

After some quick research using Google and getting blog platform usage inspiration from other blogs I came to the following options:

#### 1. WordPress

I've made some WordPress websites in the past. It's a powerfull system and definitely has it's deserved place in the market. But I know it's not for me.

A tweet by one of my colleagues reminded me of some bad old memories with WordPress.

{{< tweet user="radzikowski_m" id="1586759431588663298" >}}

[_Make sure to read Maciej's articles if you're into AWS!_](https://betterdev.blog)

The shiver while you press the update button of the plugins, hoping at least nothing would break this time. I'm sure WordPress also came a long way since then, but it did too much damage to me ;).

__I don't want a new hobby of maintaining and bugfixing my blog.__


#### 2. Ghost

Somehow Ghost had a good impression in my head. That's why it was one of the items on the list to check it out.

Looking at their landing page they went the commercial direction. I guess that's good for them but not so much for me. They show a really slick admin environment with membership statistics as a big graphic on their website. The design looks really nice!

I'm not focused on monetization and making money with my blog. So for me Ghost is not a match. If you are, in their words, a "new-media creator to publish, share, and grow a business around your content", then I would definitely check them out.


#### 3. Jykyll

I have to be honest and say that I didn't spend a lot of effort into researching this option. The pre install requires Ruby which I'm somehow hesitant for. Then I saw that one of my favorite blogs uses the next option so I didn't look into Jykyll much further.

#### 4. Hugo

One of the blogs I'm always looking forward to read is https://berthub.eu/articles/. This guy knows what he is talking about and somehow manages to find interesting topics everywhere. The blog itself is easy to read as it's very clean and "peaceful".

So what you do when you get jealous of another blog setup?! You copy their setup! No that's not exactly what I did but I did check what system he is using. The sourcecode contained the following snippet:

```html
<meta name="generator" content="Hugo 0.102.3" />
```

After quickly looking at Hugo it seems to check all the boxes. It's simple to install, easy to get up to speed with, supports markdown, it is free and open source, it is easy to deploy, it has theming support with over 300 themes available and many more features that I don't need but aren't a burden by default.

In fact it was so simple to start using Hugo, that the first draft of this page was created only 30 minutes after playing around with it. Picking a theme was the difficult part as I want the same clean feel as Bert has on his blog. But once I was done picking a theme, I also really was done deciding on the blogging platform. Hugo it is!

## Hosting

Like most nerds I have some domain names registered and have succesfully neglected them with a `Hello World!` placeholder.

_(Secretly this blog is just an excuse to extend at least one domain name a little longer. Don't judge me!)_

This `Hello World!` page was running using Github Pages for more then 4 years for free. So this time I'm using it again.

With the following documentation of Hugo and Github the blog was online in no-time:
- https://gohugo.io/hosting-and-deployment/hosting-on-github/
- https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages

All you really need, to have yourself your own website for free, is repo named according to your Github profile. In the repo settings you can then enable Github Pages. If you also want a custom domain, then you'll have to setup some DNS records and point them to the Github's servers. But that's really it.


## Content

Maybe the most important and difficult part of a blog is the content. Finding topics is not easy, it's even more difficult to write a nice article about it that is pleasant to read. Yet that doesn't mean it's not worth a try!

Reading blogs gives a great amount of joy, at least for me. You always learn something new, discover new topics, find interests that you didn't know you had. Often you read about things that you don't deal with on a day to day basis but still somehow find it interesting enough to read a long article about.

I need a place to dump my thoughts on the many interests I have and topics I come accross. Hopefully this blog will be just the right place. Thank you!

