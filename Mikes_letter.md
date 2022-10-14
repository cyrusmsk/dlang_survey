# Some non-technical ideas

Hi, Mike. Sorry to disturb you, I'm just decided to write this letter personally to the community manager instead post it on the forums. And please excuse me for all grammar errors - I'm not the native English.

First of all, let me thank you for all your work and especially for Future of D development article. Mostly on Forum people posting very technical issues, and this post a little bit about other side of the language, its environment and community.

Please consider to revise ideas below - I will be happy if you find at least one of them as useful :)

## TLDR: D needs ..

1) More precise future milestones and global vision details;
2) More attention to package management (libraries supported by dlang-community flag);
3) More attention to applications, not only language itself;
4) More surveys and structured feedback from the community;
5) Advertisement, company announcements and community work;

Most of the above mentioned items are connected and could be generalized as community management.

## Extra details:

1. In my opinion it is really great that now the community has the Vision document (https://github.com/dlang/vision-document). But in my opinion it lacks one major aspect - application. Of course, D is general purpose language and it is possibly to imagine any type of software that can be developed with D lang. But as the time of universal mathematicians have past, I believe the time of universal languages also have the same situation. Many languages have their own niches and let me say "most effective" area. Languages that do not have such details just hardly chosen by companies, hobbyists and enthusiasts. D have really broad area from high level OOP to low level betterC. But most of the people prefer to choose "right instrument for each task". And what is the D area? If we should use only couple of words.

2. The first idea is about betterC mode. Currently there is no flag in the code.dlang.io - and it is not possible to filter packages that support betterC. Maybe some other additional filters could be helpful (this could be asked from community through the survey - more details will be in item 4).
   The second thing is pretty poor description of the package details on the main page of code.dlang.io. And there is no any other information about that. And moreover sometimes it is just so many packages if try to search some popular key-words (like 'json', 'postgreSQL', 'raylib'). A lot of packages of different kind of fresh (based on last date of update). And user just do not know what to choose. He should try by hand some of them and only then make his decision.

   What is situation in other "more popular and mainstream" languages: there are different examples, but usually they have official implementation, supported by tech company or paid software engineer, or they have one or two most popular decisions (libraries) and some other hobby\enthusiast different realizations. The majority of community is choosing most popular or even official library to use in their projects. Because it is guarantee high cover of functionality, maintainability and fast delivery of new releases.

   In D situation is completely different. It is quite rarely we have some support (usually from kaleidic and symmetry) for payed realisation or even official support of the library. More commonly is a lot of different packages by different people with different type of quality and API cover.

   Also another example is a lot of "one-man" projects, instead of some packages which are developed by the bunch of community. Adam's example is most hypertrophy... Maybe he is really great developer, but his package is completely one man project which is really suffer of high risk of bus factor. No one from real business or even independent researcher likes such kind of libraries. 

   But not only his example. Also etcimon packages. Ettiene makes a lot of useful libraries and a lot of hard job, but at the last time (unfortunately) he doesn't have time or lost his interest in supporting and maintaining all his packages. So them just couldn't be correctly installed via DUB, and pull-requests are not accepted. It is quite significant libraries: memutils, libasync, botan, libhttp2, windows-headers, etc.

   Just decision of one man breaks a lot of dependencies and programs in the whole D eco-system.

   So the idea is create some kind of "dlang application committee", from proffesional of different areas. And they will choose some packages from DUB packages and selected package will have flag "supported by dlang-community". So that packages will be forked by dlang-community github account and be supported by community.

3. Mostly on Dlang Forum people are discussing language design and comparison of some language decisions. But not only the language but also selected applications could be highlighted. Currently D has only several widely used and popular (based on stars on github) applications in open-source (OneDrive and Tilix) and some data science projects (tsv-utils and vectorflow, which is abandoned). But for example Rust (which is now become overhyped and widely used) has several explicit targets for improvement (https://blog.rust-lang.org/2018/03/12/roadmap.html) in his roadmap of 2018. Here community could discussed the direction of improvement between **area leaders** (which were mentioned in item 2). The **area leaders** are professionals from different areas, who are ready to share their experience and competence with the community.
   I can name some of the examples (but I'm sure you know better those names than me):

   Web backend - author of vibe.d

   Data Science - @lempiji, @ShigekiKarita, author of vectorflow

   GPU/CUDA - Nicholas Wilson, John Colvin

   Scientific computing - 9il (Ilya)

   Portability - Brian Callahan

   Audio - Guillaume Piola

   Data Bases - someone who if professional of PostgreSQL, MySQL, etc

   etc..

   So the users will start choosing the same applications/libraries, combine the effort in bug reporting, document writing and examples, some extra support for the packages.

   And D Foundation with area leaders should decided which is some great area for D (the questions from item 1)

4. Even quite popular languages (like Go) making surveys of developers (https://go.dev/blog/survey2021-results). Smaller and younger languages also could have an improvements from that kind of information. The last official survey was in 2019 AFAIK. The last was made by WebFreak, but it was not about the whole language, but only IDE experience. In this repo you could find the questions and answers of small (~180 users) telegram chat of russian-speaking Dlang community, that was made by me (we got answers only from around 12 users). The questions were re-worked version of Nim survey with similar D technologies and libraries. Of course it could be just the base and type/quality of the question could be improved.

   The price of this activity is pretty low (Google Forms could make almost everything). And after that the answers could be used for "best area" identification and roadmap creations.

5. Marketing is quite major in our days (look and Apple). But D is really lack of this kind of activities. For example, Zig making livestreams of popular IT-bloggers, the author of the language makes streams in Twitch and Vimeo. So if someone who really good in D shows in livestreams: how mane problems could be elegantly solved in D - it could raise a new wave of newcomers to community.
   The other aspect is current community. We just do not know our "rock-stars". Even great libraries and github repos have too low numbers of stars. Maybe you could ask someone to make streams - with D lang development. Or we could find some IT streamer who is interested in that kind of activities.
   Next is companies. Of course companies highly related on D quite low (maybe even two: symmetry and funkwerk). But at least those who just use D with other languages in their stack could try to write it in their web-sites. Because page https://dlang.org/orgs-using-d.html is just not relevant. Paul Graham wrote in his abstracts about hackers and start-ups: do not look at the site of the company - look at their carrers page - whom are they hiring. And I've checked "hiring" pages of many companies from "orgs using D" - almost none of them have any D vacations. In community we knew that WEKA is using D - but you just can't find even one mentioning of the D at their main or hiring page. And community should also do something with that.

   And the last but not least point is community-management. Forum is nice... but because of different reasons not all D users could participate in the forum. And most of the communities are located in their specific regions. Most of the core-devs are from US. I think we have a big community in China (they have their own forum in chinese and user zjh could be the presenter of their community). Another big communities are in Japan and Germany. Bucharest univercity.. For example one the "legendary grand master" (which is quite cool) of competitive programming at platform codeforces who use D in competitions is japanese girl - https://codeforces.com/profile/hos.lyric?locale=en. Also we have several communities in Turkey and russian-speaking (Russia, Ukraine, Belarus). But these communities are fragmented and do not have a common goal and connections. And community-manager should also make something with it :)

Thank you if you spent your time and read it all. I hope those ideas and information that was prepared by me will be helpful. I'm not a great developer, but I hope I can help with those questions.

Have a nice day. D rocks!
