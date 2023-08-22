**r/Python** | Posted by u/Sandeev_Perera ⬆️ 680 _(2022-12-04 08:37:12)_

## What is your favorite ,most underrated 3rd party python module that made your programming 10 times more easier and less code ? so we can also try that out :-) .as a beginner , mine is pyinputplus

Original post: [https://www.reddit.com/r/Python/comments/zc3mvf/what_is_your_favorite_most_underrated_3rd_party/](https://www.reddit.com/r/Python/comments/zc3mvf/what_is_your_favorite_most_underrated_3rd_party/)

💬 ~ 191 replies

---

* 🟩 **[ArgoPanoptes](https://www.reddit.com/user/ArgoPanoptes)** ⬆️ 577 _(2022-12-04 11:01:57)_

	**tqdm** adds a progress bar when processing data with an estimated time of the finish and how many units it is processing every second. It is a lot useful when processing big data that can take several minutes. An example is processing big traffic capture files with **scapy**.

	* 🟨 **[EedSpiny](https://www.reddit.com/user/EedSpiny)** ⬆️ 51 _(2022-12-04 16:55:05)_

		Upvoted as I used this in a recent project that did transforms on relational data. Tqdm even has sub-progress bars so I could see progress per table as well as over all. 10/10 would tqdm again.

	* 🟨 **[benefit_of_mrkite](https://www.reddit.com/user/benefit_of_mrkite)** ⬆️ 22 _(2022-12-04 17:22:51)_

		I use Tqdm all the time - same with scapy.  Most of my code these days consumes REST APIs and almost all of it is Async - tqdm has built-in Async which shows overall task queue progress

		* 🟧 **[kraakmaak](https://www.reddit.com/user/kraakmaak)** ⬆️ 6 _(2022-12-04 18:07:35)_

			That sounds cool, could you share an example of async api calls with tqdm progressbar?

			* 🟦 **[benefit_of_mrkite](https://www.reddit.com/user/benefit_of_mrkite)** ⬆️ 8 _(2022-12-04 19:30:59)_

				About to head out of town but I’ll try to remember to respond when back in front of my computer.  There are good Async examples in the tqdm docs

	* 🟨 **[easyEggplant](https://www.reddit.com/user/easyEggplant)** ⬆️ 5 _(2022-12-04 23:18:20)_

		And it’s so damn simple. So simple that it took me awhile to figure it out if that makes any sense. Like “really? Just wrap an iterator?!?”

	* 🟨 **[This-Winter-1866](https://www.reddit.com/user/This-Winter-1866)** ⬆️ 0 _(2022-12-04 21:49:04)_

		REMOVED DUE TO CUSTOM FILTER(S)

		* 🟧 **[anti4r](https://www.reddit.com/user/anti4r)** ⬆️ 7 _(2022-12-04 23:22:52)_

			Why use idle when ipython/bpython exists?

			* 🟦 **[This-Winter-1866](https://www.reddit.com/user/This-Winter-1866)** ⬆️ 8 _(2022-12-04 23:34:09)_

				Because IDLE is extremely lightweight and works smoothly on my toaster.

		* 🟧 **[bobbruno](https://www.reddit.com/user/bobbruno)** ⬆️ 1 _(2022-12-05 02:55:09)_

			Try this: https://stackoverflow.com/questions/47995958/python-tqdm-package-how-to-configure-for-less-frequent-status-bar-updates

* 🟩 **[a4c2e4lm2o2p2rstuw2](https://www.reddit.com/user/a4c2e4lm2o2p2rstuw2)** ⬆️ 157 _(2022-12-04 12:04:45)_

	[Loguru](https://loguru.readthedocs.io/en/stable/overview.html) is my favorite module, hands down. Makes it so easy to handle logging. I haven't used print in years.

	* 🟨 **[deleted]** ⬆️ 66 _(2022-12-04 21:08:35)_

		Comment deleted by user

		* 🟧 **[MDTv_Teka](https://www.reddit.com/user/MDTv_Teka)** ⬆️ 3 _(2022-12-08 20:46:39)_

			Big brain time

	* 🟨 **[turner_prize](https://www.reddit.com/user/turner_prize)** ⬆️ 18 _(2022-12-04 15:23:11)_

		Same. Still use Print quite a lot when debugging but all of my regular logging is done through loguru.

		* 🟧 **[deleted]** ⬆️ 24 _(2022-12-04 15:57:19)_

			Debugger friend, so much more useful than print statements.

			* 🟦 **[skesisfunk](https://www.reddit.com/user/skesisfunk)** ⬆️ 7 _(2022-12-04 20:04:44)_

				Both approaches have their place

				* 🟪 **[RangerPretzel](https://www.reddit.com/user/RangerPretzel)** ⬆️ -13 _(2022-12-05 02:38:19)_

					REMOVED DUE TO CUSTOM FILTER(S)

					* 🟥 **[skesisfunk](https://www.reddit.com/user/skesisfunk)** ⬆️ 3 _(2022-12-05 03:51:44)_

						Print is generally just for printing to the console. The `logging` module is more specifically geared towards communicating something to a user. Even then its silly to say either of them cant be used for debugging,  do whatever works to get the job done! Sometimes printing a variables value is faster than setting up the debugger.

	* 🟨 **[thatdamnedrhymer](https://www.reddit.com/user/thatdamnedrhymer)** ⬆️ 10 _(2022-12-04 16:14:36)_

		How does it compare to structlog?

	* 🟨 **[boiledgoobers](https://www.reddit.com/user/boiledgoobers)** ⬆️ 11 _(2022-12-04 13:28:42)_

		You ever used logzero? It's usually my go to for logging, but I'm curious about this one now.

	* 🟨 **[foobarijk](https://www.reddit.com/user/foobarijk)** ⬆️ 6 _(2022-12-05 12:33:20)_

		What's wrong with python's logging?

	* 🟨 **[bioinfx](https://www.reddit.com/user/bioinfx)** ⬆️ 4 _(2022-12-04 19:42:24)_

		This looks amazing

* 🟩 **[sphen_lee](https://www.reddit.com/user/sphen_lee)** ⬆️ 99 _(2022-12-04 09:50:57)_

	Data validation libraries. Originally marshmallow and now pydantic

	* 🟨 **[TheAJGman](https://www.reddit.com/user/TheAJGman)** ⬆️ 35 _(2022-12-04 14:52:37)_

		All hail pydantic. It makes generators for tests and shit so much more readable.

	* 🟨 **[kalfa](https://www.reddit.com/user/kalfa)** ⬆️ 8 _(2022-12-04 12:57:19)_

		although pydantic is a parsing lib mainly, not validation library.
		
		might not change much for your use cases, but it could also mean you might better off with something else
		
		> pydantic is primarily a parsing library, not a validation library. Validation is a means to an end: building a model which conforms to the types and constraints provided.
		
		https://pydantic-docs.helpmanual.io/usage/models/

		* 🟧 **[sphen_lee](https://www.reddit.com/user/sphen_lee)** ⬆️ 20 _(2022-12-04 15:34:43)_

			I think they are just being pedantic (pun intended).
			
			Beginners won't think of what pydantic does as "parsing". The usage of that term came about from a blog "Parse, don't Validate" (I think the original is here: https://lexi-lambda.github.io/blog/2019/11/05/parse-don-t-validate/ ) so I wouldn't expect people to be familiar with it.
			
			I don't use pydantic for validating business rules (which seems to be what the pydantic docs are referring to?) but instead to validate the shape of the data. Once I get a model out of it I don't have to use `dict.get` or check for None on mandatory fields. I don't have to worry about substituting defaults, or worry about iterating a string instead of a list of strings. This is what I mean by "data validation".
			
			Marshmallow is a similar thing - I used it for generating JSON responses in my API. It's strength was in exporting: generating valid JSON from my objects.

		* 🟧 **[scotticusphd](https://www.reddit.com/user/scotticusphd)** ⬆️ 19 _(2022-12-04 13:12:22)_

			> ...
			> Although validation is not the main purpose of pydantic, you can use this library for custom validation.
			
			It does do validation though and I use it for that. Do you have a recommended alternative?

			* 🟦 **[danted002](https://www.reddit.com/user/danted002)** ⬆️ 1 _(2022-12-04 20:33:57)_

				Marshmallow.

		* 🟧 **[MrJohz](https://www.reddit.com/user/MrJohz)** ⬆️ 10 _(2022-12-04 15:30:52)_

			In fairness, "parsing" in this context is a form of data validation in the general sense, but with the principle that you validate the data only as it comes in and goes out, and rather than just validating that it's the correct shape, you also convert it into the shape that's most convenient for you (e.g. converting timestamp strings into datetime objects, converting other strings into enums where it makes sense, etc).
			
			Most of the time, when people are talking about validation, what they want to do is parsing, and the benefit of pydantic is that it is designed to encourage parsing even to do basic validation tasks.

* 🟩 **[fizzymagic](https://www.reddit.com/user/fizzymagic)** ⬆️ 69 _(2022-12-04 11:04:06)_

	more-itertools, in a heartbeat. Pandas is its own thing, as is pydantic.  They make new functionality rather than making things easier.  Just MO.

	I do like using tqdm.

	* 🟨 **[FlyingCow343](https://www.reddit.com/user/FlyingCow343)** ⬆️ 5 _(2022-12-05 00:30:30)_

		I really should download more-itertools, at the moment i just copy-paste the code from the docs

* 🟩 **[spidLL](https://www.reddit.com/user/spidLL)** ⬆️ 74 _(2022-12-04 11:54:20)_

	[Rich](https://github.com/Textualize/rich)

	* 🟨 **[sohang-3112](https://www.reddit.com/user/sohang-3112)** ⬆️ 2 _(2022-12-04 15:51:59)_

		Nice! Especially `rich.pretty.install()` looks quite interesting!

	* 🟨 **[Professional_Cook808](https://www.reddit.com/user/Professional_Cook808)** ⬆️ -50 _(2022-12-04 14:13:10)_

		REMOVED DUE TO CUSTOM FILTER(S)

		* 🟧 **[EclipseJTB](https://www.reddit.com/user/EclipseJTB)** ⬆️ 13 _(2022-12-04 22:02:18)_

			Then you haven't scratched the surface of what `rich` does.
			
			Progress bar? Yup.
			
			Tabular data? You got it.
			
			Colors? You know this one, but it's STUPID EASY.
			
			Custom print methods on classes? This is the magical one.

		* 🟧 **[spidLL](https://www.reddit.com/user/spidLL)** ⬆️ 30 _(2022-12-04 15:55:02)_

			I don’t remember asking you for a code review.

* 🟩 **[slapec](https://www.reddit.com/user/slapec)** ⬆️ 52 _(2022-12-04 14:40:50)_

	[stackprinter](https://pypi.org/project/stackprinter/) saved me many many times by printing all locals in the traceback. I use it in all my projects.

	* 🟨 **[Eggplantwater](https://www.reddit.com/user/Eggplantwater)** ⬆️ 3 _(2022-12-04 16:07:46)_

		Ohh that sounds handy. Thanks!

	* 🟨 **[sohang-3112](https://www.reddit.com/user/sohang-3112)** ⬆️ 2 _(2022-12-04 16:09:14)_

		Wow - never knew about this library - it's crazy useful! Thanks!!

	* 🟨 **[pratzc07](https://www.reddit.com/user/pratzc07)** ⬆️ 2 _(2022-12-04 18:26:55)_

		This is great thank you

	* 🟨 **[GeniusFrequency](https://www.reddit.com/user/GeniusFrequency)** ⬆️ 2 _(2022-12-05 00:26:43)_

		[loguru also supports this](https://loguru.readthedocs.io/en/stable/overview.html?highlight=traceback#fully-descriptive-exceptions)

	* 🟨 **[slapec](https://www.reddit.com/user/slapec)** ⬆️ 2 _(2022-12-05 11:15:26)_

		Maybe it's just for me, but my out of box experience with stackprinter is better than with [better-exceptions](https://github.com/Qix-/better-exceptions), which has 4 times more stars on github.  
		
		Consider this:
		
		```
		def fail(a):
		    crash = False
		    if a == 0:
		        crash = True
		    if crash:
		        raise NotImplementedError
		```
		
		Running with better-exceptions installed:
		
		```
		import better_exceptions
		better_exceptions.hook()
		fail(0)
		```
		
		Shows this traceback:
		
		```
		Traceback (most recent call last):
		  File "crash.py", line 10, in &lt;module>
		    fail(0)
		    └ &lt;function fail at 0x7f7fef77e710>
		  File "crash.py", line 6, in fail
		    raise NotImplementedError
		NotImplementedError
		```
		
		Which is not more useful than the plain traceback. However running with stackprinter:
		
		```
		File "crash.py", line 10, in &lt;module>
		    6            raise NotImplementedError
		    7    
		    8    import stackprinter
		    9    stackprinter.set_excepthook()
		--> 10   fail(0)
		    ..................................................
		     stackprinter = &lt;module 'stackprinter' from 'python3
		                     .10/site-packages/stackprinter/__init__.py'>
		     stackprinter.set_excepthook = &lt;function 'set_excepthook' __init__.py:250>
		    ..................................................
		
		File "crash.py", line 6, in fail
		    1    def fail(a):
		    2        crash = False
		    3        if a == 0:
		    4            crash = True
		    5        if crash:
		--> 6            raise NotImplementedError
		    ..................................................
		     a = 0
		     crash = True
		    ..................................................
		
		NotImplementedError
		```
		
		It just far more useful.
		(I know it's a crafted code snippet, in real-world examples better-traceback might be as good as stackprinter, also you might configure better-traceback to be as verbose as stackprinter, but straight after pip install, stackprinter is just simply better for my needs.)

* 🟩 **[kalebludlow](https://www.reddit.com/user/kalebludlow)** ⬆️ 118 _(2022-12-04 10:11:37)_

	Pygsheets for editing Google sheets, moviepy for wrapping ffmpeg easily, pymongo for MongoDB, pymiere and Photoshop-python for controlling premiere/Photoshop

	Beyond just modules, google Colab has been great for prototyping code, within an environment that is ready to go for 99% of scenarios. Anvil.works has also been an absolute boon for me, allowing me to create a rather complex system with UI and an API all in python. That probably deserves a post of it's own

	* 🟨 **[Inkosum](https://www.reddit.com/user/Inkosum)** ⬆️ 12 _(2022-12-04 10:26:25)_

		Didn't know about moviepy yet I have an idea for a future project using ffmpeg. Thanks!

		* 🟧 **[kalebludlow](https://www.reddit.com/user/kalebludlow)** ⬆️ 8 _(2022-12-04 10:27:54)_

			I needed to combine a bunch of separate video files together, and moviepy seems to be the easiest way to do it and still get all the control you need. One issue I've had is trying to pipe the progress bar from the console to a visual component, but that's the least of my worries

	* 🟨 **[MDTv_Teka](https://www.reddit.com/user/MDTv_Teka)** ⬆️ 2 _(2022-12-08 20:48:01)_

		Wait what? What can you do in Photoshop via Python? Like you have .psd templates and you auto edit them via Python?

		* 🟧 **[kalebludlow](https://www.reddit.com/user/kalebludlow)** ⬆️ 1 _(2022-12-08 20:50:07)_

			Yeah exactly right, can do 95% of all basic editing using photoshop-python-api. I'm using an app framework called Anvil.works which allows me to run code locally that is controlled by a webapp. Fully remote, automated Photoshop and premiere (using pymiere) with no user input. Set up your template and you're good to go. There's no headless mode, but can work around that

* 🟩 **[scotticusphd](https://www.reddit.com/user/scotticusphd)** ⬆️ 29 _(2022-12-04 13:07:10)_

	I found [icecream](https://github.com/gruns/icecream) in a post on this subreddit and still use it as an alternative to print for debugging.

	* 🟨 **[WesternGoldsmith](https://www.reddit.com/user/WesternGoldsmith)** ⬆️ 2 _(2022-12-04 16:01:01)_

		&amp;#x200B;
		
		This is what I wanted. Thanks for the suggestion. :)

	* 🟨 **[Impossible-Limit3112](https://www.reddit.com/user/Impossible-Limit3112)** ⬆️ 2 _(2022-12-04 17:13:49)_

		Found [PySnooper](https://github.com/cool-RR/PySnooper) the other day.

* 🟩 **[Present_Reaction8625](https://www.reddit.com/user/Present_Reaction8625)** ⬆️ 32 _(2022-12-04 13:17:50)_

	Arrow - date time manipulations, pydantic - data validation, fastapi - api server/flask alternative, typer - click alternative, loguru - second to none in logging capability.

	* 🟨 **[jmreagle](https://www.reddit.com/user/jmreagle)** ⬆️ 4 _(2022-12-04 21:11:10)_

		I use pendulum now over arrow.

		* 🟧 **[Present_Reaction8625](https://www.reddit.com/user/Present_Reaction8625)** ⬆️ 2 _(2023-05-02 12:18:03)_

			Pendulum hasn't been updated in ages and often breaks at building wheels. There's an alpha version of Pendulum 3 which is fixing these issues.

			* 🟦 **[jmreagle](https://www.reddit.com/user/jmreagle)** ⬆️ 2 _(2023-05-02 13:00:41)_

				Oh, I didn’t realize. I appreciate the API and hope it manages to survive.

* 🟩 **[livrem](https://www.reddit.com/user/livrem)** ⬆️ 32 _(2022-12-04 13:47:50)_

	[Lea](https://pypi.org/project/lea/), " a Python module aiming at working with discrete probability distributions in an intuitive way.

	It allows you modeling a broad range of random phenomena: gambling, weather, finance, etc. More generally, Lea may be used for any finite set of discrete values having known probability: numbers, booleans, date/times, symbols,… Each probability distribution is modeled as a plain object, which can be named, displayed, queried or processed to produce new probability distributions."

	Very useful. Maybe not making much of my programming easier, but for doing math related to hobby-gamedesign.

	* 🟨 **[brayellison](https://www.reddit.com/user/brayellison)** ⬆️ 1 _(2022-12-05 03:28:37)_

		Interesting, haven't heard of this one. How does it compare to numpyro and/or pymc?

		* 🟧 **[livrem](https://www.reddit.com/user/livrem)** ⬆️ 1 _(2022-12-05 17:36:59)_

			I never saw those two. Or possibly pymc. That one looks vaguely familiar. I probably should spend a bit of time comparing more different options, but back when I first saw Lea a few years ago I was happy to find something that allowed me to use Python instead of R for my calculations (that are never very complex). I did search a bit for alternatives, but did not really find anything else at that time, so I just used Lea since.

* 🟩 **[joszko](https://www.reddit.com/user/joszko)** ⬆️ 28 _(2022-12-04 14:14:32)_

	[Reloadium](https://reloadium.io/) \- hot reloading

	* 🟨 **[sohang-3112](https://www.reddit.com/user/sohang-3112)** ⬆️ 2 _(2022-12-04 16:39:30)_

		Wow - this is so useful!! This is the closest Python approximation I have found yet to the level of interactivity in Lisp.

* 🟩 **[aes110](https://www.reddit.com/user/aes110)** ⬆️ 24 _(2022-12-04 12:54:00)_

	Wouldn't say its my favourite, but one I like to bring up sometimes is [boltons](https://boltons.readthedocs.io/en/latest/)

	> Boltons is a set of pure-Python utilities in the same spirit as — and yet conspicuously missing from — the standard library

	Three really are some great stuff there that makes you wonder why its missing from the built-in library

	 

	My favorite is the [remap](https://boltons.readthedocs.io/en/latest/iterutils.html#boltons.iterutils.remap) function to recursively iterate and transform complex data structures.

	* 🟨 **[wewbull](https://www.reddit.com/user/wewbull)** ⬆️ 3 _(2022-12-04 18:59:49)_

		Thanks. I've written `remap` several times for different projects. I'm always amazed it's not in `itertools`.

	* 🟨 **[BossOfTheGame](https://www.reddit.com/user/BossOfTheGame)** ⬆️ 1 _(2022-12-05 02:44:06)_

		Checkout IndexableWalker in ubelt.

* 🟩 **[wWBigheadWw](https://www.reddit.com/user/wWBigheadWw)** ⬆️ 19 _(2022-12-04 11:49:11)_

	pydantic

* 🟩 **[wxtrails](https://www.reddit.com/user/wxtrails)** ⬆️ 14 _(2022-12-04 13:50:52)_

	`sh` ([pypi](https://pypi.org/project/sh/)) is a great `subprocess` replacement if you find yourself orchestrating lots of other processes in Python like I do.

	* 🟨 **[Baschg](https://www.reddit.com/user/Baschg)** ⬆️ 3 _(2022-12-04 16:38:50)_

		[universalwrapper](https://github.com/Basdbruijne/UniversalWrapper) works great for that too, and support async commands

	* 🟨 **[sohang-3112](https://www.reddit.com/user/sohang-3112)** ⬆️ 2 _(2022-12-04 16:36:28)_

		Thanks for sharing this - `subprocess` can be a real PITA sometimes!

* 🟩 **[yaxriifgyn](https://www.reddit.com/user/yaxriifgyn)** ⬆️ 12 _(2022-12-04 13:09:58)_

	**Send2Trash** is very handly when you want to let the end user have final say about file deletion. It works on  MS windows, Apple mac, and Linux.

* 🟩 **[agtoever](https://www.reddit.com/user/agtoever)** ⬆️ 11 _(2022-12-04 19:13:55)_

	[Networkx](https://networkx.org). The hard-to-find but very powerfull module for working with graphs (as in: 🕸️ networks, not as in: 📈📊 graphical charts).

* 🟩 **[tspier](https://www.reddit.com/user/tspier)** ⬆️ 9 _(2022-12-04 17:58:32)_

	Whether it's underrated or not, I really don't know, but definitely *prettytable* for me. I can neatly organize data in ASCII-style, perfectly-formatted tables or even export to HTML for more public-facing viewing.

* 🟩 **[aaronlyy](https://www.reddit.com/user/aaronlyy)** ⬆️ 38 _(2022-12-04 10:29:56)_

	Definitely click, had so much fun making cli's with it

	* 🟨 **[lordmauve](https://www.reddit.com/user/lordmauve)** ⬆️ 24 _(2022-12-04 12:06:31)_

		I've found click needs too much boilerplate and gets in the way too much. Now I recommend [defopt](https://defopt.readthedocs.io/en/latest/).

		* 🟧 **[squarepushercheese](https://www.reddit.com/user/squarepushercheese)** ⬆️ 5 _(2022-12-04 12:46:19)_

			That does look simple. Nice.

	* 🟨 **[deleted]** ⬆️ 13 _(2022-12-04 11:35:08)_

		[removed]

		* 🟧 **[thedji](https://www.reddit.com/user/thedji)** ⬆️ 1 _(2022-12-04 17:40:26)_

			+1. fire is lit.

	* 🟨 **[QuantumQuack0](https://www.reddit.com/user/QuantumQuack0)** ⬆️ 11 _(2022-12-04 13:28:23)_

		I personally prefer [typer](https://typer.tiangolo.com/). It makes clever use of python type hints.

	* 🟨 **[benefit_of_mrkite](https://www.reddit.com/user/benefit_of_mrkite)** ⬆️ 2 _(2022-12-04 17:32:01)_

		I’ve used click, fire, typer and more and I prefer click for deep CLi projects but typer is easier for a one off simple project where you don’t need much.
		
		Clicks context (ctx) is amazing

	* 🟨 **[OneMorePenguin](https://www.reddit.com/user/OneMorePenguin)** ⬆️ 3 _(2022-12-04 22:07:23)_

		I don't like click.  It's poorly documented and difficult to use if you have a lot of argument type processing to do at runtime.

* 🟩 **[ImpulseBadger](https://www.reddit.com/user/ImpulseBadger)** ⬆️ 8 _(2022-12-04 11:41:34)_

	[Taskipy](https://github.com/illBeRoy/taskipy)

	Absolute little gem of a project that we’ve fully integrated into our entire development, CI and deployment pipeline.

	* 🟨 **[glacierre2](https://www.reddit.com/user/glacierre2)** ⬆️ 2 _(2022-12-04 21:36:22)_

		I am torn between this (which i did not know) and nox. Anybody has compared them?

		* 🟧 **[AndydeCleyre](https://www.reddit.com/user/AndydeCleyre)** ⬆️ 2 _(2022-12-04 22:49:05)_

			I use both in a single project, where taskipy tasks are more user/dev facing and *mostly* trigger nox sessions, in ways that are useful for interactive development.

* 🟩 **[ekladev](https://www.reddit.com/user/ekladev)** ⬆️ 7 _(2022-12-04 15:05:41)_

	Sh [sh](https://amoffat.github.io/sh/) and outside python, watch [watch](https://linuxize.com/post/linux-watch-command/)

* 🟩 **[manueslapera](https://www.reddit.com/user/manueslapera)** ⬆️ 7 _(2022-12-04 22:15:35)_

	Have you ever had to deal with an api or dataset that looks like this:

	```

	data = {

	"a": {

	  "b": {

	     [

	       {

	         "c":[0,1,2]

	       }

	     ]

	  }

	}

	```

	And you have to parse it like this or any other unnested nasty code:

	```

	if 'a' in data:

	  if 'b' in data['a']:

	    ...omg i hate this

	```

	or even worse:

	```

	value_i_care = data.get('a',{}).get('b',[{}])[0]['c']

	```

	[glom](https://glom.readthedocs.io) to the rescue!

	with glom you can do something like this:

	```

	from glom import glom

	value_i_care = glom(data, 'a.b.c') 

	```

* 🟩 **[jsalsman](https://www.reddit.com/user/jsalsman)** ⬆️ 27 _(2022-12-04 13:09:02)_

	**dataset** made my core production code two thirds smaller and changed my life. https://dataset.readthedocs.io/en/latest/ The goal of dataset is to make basic database operations simpler, by expressing cross-platform SQL database operations in a Pythonic way. It has 4.2k stars on GitHub, is actively maintained, and has been stable for about ten years.

	Raw SQLAlchemy sucks: the lengthy and confusing OOP table declarations, the multi-line inscrutable database operations, the hoops you have to jump through to change a schema, and the lack of access to a simple and intuitive DDL or equivalent, just to name a few antipatterns. Dataset turns almost all your database operations into little more than dictionary or method syntax, whichever you prefer, and also lets you do raw SQL when you need a special query or database feature here and there. It is so much more maintainable, explainable, readable and writable, it's like night and day.

	The only barely legit critique of it I've seen is that it doesn't support async queries. It's not like those are easy or common in SQLAlchemy, but you can spawn a process to handle async dataset operations and pass the results back in a queue: https://docs.python.org/3/library/multiprocessing.html#exchanging-objects-between-processes -- You can use ``.wait(timeout=0)`` to check if they're ready or ``.wait(timeout=None)`` to block until they are. All the other possible complaints are listed in the docs' limitations list, and they all have easy and obvious work-arounds. If you need something from SQLAlchemy such as column types when you're creating a table (the effective DDL takes one line each for declaring columns and indexes, including PostgreSQL ARRAY columns) or supporting legacy code, that is not a problem because dataset is built on top of SQLAlchemy.

	* 🟨 **[boiledgoobers](https://www.reddit.com/user/boiledgoobers)** ⬆️ 10 _(2022-12-04 13:36:25)_

		Funny how different people like different things. The object oriented table definitions are SUCH a boon for me. I LOVE them.

		* 🟧 **[jsalsman](https://www.reddit.com/user/jsalsman)** ⬆️ 6 _(2022-12-04 13:43:13)_

			I know people must. I always get downvoted when I bring up dataset. Different strokes!

		* 🟧 **[NoDadYouShutUp](https://www.reddit.com/user/NoDadYouShutUp)** ⬆️ 2 _(2022-12-04 14:47:16)_

			Same

		* 🟧 **[reckless_commenter](https://www.reddit.com/user/reckless_commenter)** ⬆️ 1 _(2022-12-04 23:52:20)_

			For primitive fields, SQLAlchemy requires a lot of extra code without a lot of value. But for relationship types, SQLAlchemy is quite nice. It can model 1:n, n:1, m:n, and association-table relationships well, and when you materialize an object and examine its fields for related objects or lists, you get other materialized objects.
			
			On the other hand, SQLAlchemy is not very performant. Also, SQLAlchemy has some weird semantics about data caching that result in false Stale Data Errors, which can require a lot of debugging and sometimes just trial-and-error. But I forgive these limitations because of its overall maturity and general robustness.

			* 🟦 **[mok000](https://www.reddit.com/user/mok000)** ⬆️ 2 _(2022-12-05 00:30:49)_

				I am using the ORM of Django I find it much easier to use than SQLAlchemy.

	* 🟨 **[TheAJGman](https://www.reddit.com/user/TheAJGman)** ⬆️ 6 _(2022-12-04 14:57:23)_

		That's pretty sweet. I'm personally partial to the Django ORM and I really wish they had a ORM-only package for standalone use. You *can* just [ignore everything not ORM related](https://github.com/dancaron/Django-ORM), but it would be nice to have a smaller/cleaner package too.

	* 🟨 **[root45](https://www.reddit.com/user/root45)** ⬆️ 4 _(2022-12-04 14:43:30)_

		>All the other possible complaints are listed in the docs' limitations list, and they all have easy and obvious work-arounds.
		
		I maybe missed it, but what is the easy and obvious workaround for foreign keys and joined tables?

		* 🟧 **[jsalsman](https://www.reddit.com/user/jsalsman)** ⬆️ 1 _(2022-12-04 15:12:27)_

			I use ARRAY(Integer) columns to hold foreign keys in PostgreSQL, which is so much nicer than having another table as in https://stackoverflow.com/a/18854791 But if you don't have array columns, you can either declare such a table like that explicitly or keep your foreign keys encoded in a Text or LargeBinary column.
			
			For joining, just use raw SQL which is more concise and readable by orders of magnitude more people than SQLAlchemy's syntax.

			* 🟦 **[root45](https://www.reddit.com/user/root45)** ⬆️ 2 _(2022-12-04 15:50:20)_

				> I use ARRAY(Integer) columns to hold foreign keys in PostgreSQL
				
				I'm not sure I understand. Do you manage the relationship yourself this way? If you have `parent` and `child` tables, you keep a `children` array column on the `parent` table? And every time you add or remove a `child` row, you loop through the `children` column to remove that ID? Is that right?

	* 🟨 **[sohang-3112](https://www.reddit.com/user/sohang-3112)** ⬆️ 3 _(2022-12-04 16:26:29)_

		You mentioned that you have used `dataset` in production code, but this feature in its docs seems a bit problematic to me:
		
		> Automatic schema: If a table or column is written that does not exist in the database, it will be created automatically.
		
		I'm sure this is convenient during development - but in production code, IMO you *don't* want any implicit mutations. Not to mention, this won't work anyway for database users who don't have `UPDATE` permission in the database!

		* 🟧 **[jsalsman](https://www.reddit.com/user/jsalsman)** ⬆️ 2 _(2022-12-04 17:08:53)_

			It hasn't been a problem. Column names are usually simple and not easy to misspell. I use unit tests for virtually all my top level db operations, although now that I think about it my coverage is spotty when it comes to all the permutations of their logic.

		* 🟧 **[root45](https://www.reddit.com/user/root45)** ⬆️ 2 _(2022-12-04 17:21:36)_

			The documentation basically says it's not viable for things larger than toy projects. It doesn't even handle foreign keys and joins. I could maybe see this being useful for ad hoc scripting where you want to keep some temporary state. But outside of that I don't really see the use.

	* 🟨 **[AndydeCleyre](https://www.reddit.com/user/AndydeCleyre)** ⬆️ 2 _(2022-12-04 23:46:20)_

		I have definitely enjoyed using dataset to get things done. FYI peewee is a great project from a great developer that does a LOT of database things, and an extension is available that's basically [a dataset clone](http://docs.peewee-orm.com/en/latest/peewee/playhouse.html#dataset).

		* 🟧 **[jsalsman](https://www.reddit.com/user/jsalsman)** ⬆️ 1 _(2022-12-05 02:27:29)_

			Neat! Thanks!

* 🟩 **[colemaker360](https://www.reddit.com/user/colemaker360)** ⬆️ 19 _(2022-12-04 13:20:36)_

	[Arrow](https://github.com/arrow-py/arrow) makes dealing with dates and timezones way easier than the built-ins. Years ago I got sick of looking up how to use date types properly for the umpteenth time and found arrow, and I still use it all the time.

	* 🟨 **[sohang-3112](https://www.reddit.com/user/sohang-3112)** ⬆️ 12 _(2022-12-04 15:55:16)_

		IDK, `datetime` seems pretty intuitive to me

		* 🟧 **[deleted]** ⬆️ 7 _(2022-12-04 20:13:36)_

			Comment deleted by user

			* 🟦 **[sohang-3112](https://www.reddit.com/user/sohang-3112)** ⬆️ 2 _(2022-12-05 02:16:33)_

				> naive datetime
				
				Do you mean that it doesn't account for timezone by default? If that's what you mean, then I usually just set a global timezone via the environment variable `TZ`. But I suppose you might have an issue if dealing with many different timezones.

	* 🟨 **[WoodenNichols](https://www.reddit.com/user/WoodenNichols)** ⬆️ 4 _(2022-12-04 16:45:40)_

		Seconding arrow. Saves me lots of time.
		And I agree with the OP: pyinputplus is extremely useful.

* 🟩 **[public_radio](https://www.reddit.com/user/public_radio)** ⬆️ 17 _(2022-12-04 13:00:24)_

	I'll shamelessly share a couple I wrote that I'm proud of:  

	[flatsplode](https://github.com/amancevice/flatsplode) — flatten + explode nested JSON (works well with pandas)  

	[requests-iamauth](https://github.com/amancevice/requests-iamauth) — requests plugin for using AWS' sigv4 as an HTTP authorizer  

	[redpanda](https://github.com/amancevice/redpanda) — a SQLAlchemy plugin for pulling SQL data as pandas dataframes

	* 🟨 **[LankyXSenty](https://www.reddit.com/user/LankyXSenty)** ⬆️ 4 _(2022-12-04 13:54:36)_

		Thanks, definitely gonna try the flatsplode one out! Pandas.to_json is always a little bit try n error :D

		* 🟧 **[sohang-3112](https://www.reddit.com/user/sohang-3112)** ⬆️ 1 _(2022-12-04 16:31:39)_

			Me too! Being able to explore nested JSON in a `pd.DataFrame` would be super convenient!

			* 🟦 **[Dasher38](https://www.reddit.com/user/Dasher38)** ⬆️ 3 _(2022-12-04 17:29:02)_

				https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.json_normalize.html

				* 🟪 **[sohang-3112](https://www.reddit.com/user/sohang-3112)** ⬆️ 2 _(2022-12-04 18:39:53)_

					Thanks - I didn't know about this!

	* 🟨 **[root45](https://www.reddit.com/user/root45)** ⬆️ 3 _(2022-12-04 14:23:15)_

		I'm not sure I understand the benefit of redpanda. You can pass a SQLAlchemy query directly to `pd.read_sql` already.

		* 🟧 **[public_radio](https://www.reddit.com/user/public_radio)** ⬆️ 2 _(2022-12-04 15:58:30)_

			It’s definitely a little niche but it lets you take your existing SQLAlchemy ORM models and query them as DataFrames. pd.read_sql (as far as I know) takes raw SQL, but if you already have a whole ORM class with relations hooked up you can use the SQLAlchemy query syntax to get a DataFrame out. See the example [here](https://github.com/amancevice/redpanda/blob/main/redpanda/example.py)
			
			Edit — Oh I see from your comment that read_sql can take a SQLAlchemy query. It’s possible when I wrote this way back when it just took a string.

	* 🟨 **[Dasher38](https://www.reddit.com/user/Dasher38)** ⬆️ 1 _(2022-12-04 17:28:13)_

		Does flatsplode do anything more than this ?
		https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.json_normalize.html

		* 🟧 **[public_radio](https://www.reddit.com/user/public_radio)** ⬆️ 3 _(2022-12-04 17:39:47)_

			Looks very similar. Damn, pandas, adding  more features I needed after I wrote my own :)

			* 🟦 **[Dasher38](https://www.reddit.com/user/Dasher38)** ⬆️ 2 _(2022-12-04 18:19:13)_

				I also ended up with my own when trying to unpack  JSON-encoded array of Rust enums into a pandas dataframes. I used a JSON scheme to figure out the structure of the data in a generic way

	* 🟨 **[benefit_of_mrkite](https://www.reddit.com/user/benefit_of_mrkite)** ⬆️ 1 _(2022-12-04 17:30:23)_

		Will flatsplode send the data back to its original format or is it one-way only?

		* 🟧 **[public_radio](https://www.reddit.com/user/public_radio)** ⬆️ 1 _(2022-12-04 17:37:27)_

			One-way. It generates a new object, though so your input is unchanged.

* 🟩 **[phlooo](https://www.reddit.com/user/phlooo)** ⬆️ 6 _(2022-12-04 12:18:03)_

	Not so underrated but not so commonplace either: [Zarr](https://github.com/zarr-developers/zarr-python)

	It saved my ass quite a few times in threaded and IO critical applications, where other similar packages would simply all just be too slow or non thread safe at all

	* 🟨 **[Dasher38](https://www.reddit.com/user/Dasher38)** ⬆️ 1 _(2022-12-04 17:34:51)_

		How does it compare to arrow IPC or parquet ?

		* 🟧 **[CookingWithoutWater](https://www.reddit.com/user/CookingWithoutWater)** ⬆️ 2 _(2022-12-04 19:25:06)_

			Arrow and parquet are 2D; Zarr is ND. Depends on your data which is better

* 🟩 **[tathagatadg](https://www.reddit.com/user/tathagatadg)** ⬆️ 6 _(2022-12-04 14:25:02)_

	What do you all use for executing code over ssh these days? Is paramiko still the choice? There’s a lot of boilerplate to go just subprocess - the other pattern I’ve been following is running the script with ansible. Easy to keep the network io separate and pushed up to ansible - and if you have to scale out or different business logic depending on which server you are executing. Would be interesting to hear if there are other patterns people have used.

	* 🟨 **[vantasmer](https://www.reddit.com/user/vantasmer)** ⬆️ 11 _(2022-12-04 15:28:57)_

		Paramiko and Netmiko are generally regarded as the go-to for SSH connection.
		Napalm is also an option if you’re doing a lot of net config stuff

		* 🟧 **[benefit_of_mrkite](https://www.reddit.com/user/benefit_of_mrkite)** ⬆️ 1 _(2022-12-04 17:28:32)_

			100% agree with this statement have used all 3 libraries for many projects.

	* 🟨 **[cosmasterblaster](https://www.reddit.com/user/cosmasterblaster)** ⬆️ 2 _(2022-12-04 16:45:56)_

		I'm a Network Engineer and I use Netmiko whenever my scripts connect over SSH. Ansible or SaltStack are good for orchestrating which scripts to run, but at the core I use Netmiko.

		* 🟧 **[vantasmer](https://www.reddit.com/user/vantasmer)** ⬆️ 1 _(2022-12-04 18:29:14)_

			Have you tried Nornir? I like ansible and salt but this seems to be a more python native alternative.

	* 🟨 **[_azulinho_](https://www.reddit.com/user/_azulinho_)** ⬆️ 1 _(2022-12-05 02:23:08)_

		I use seantis/suitable best of the pack

* 🟩 **[ArabicLawrence](https://www.reddit.com/user/ArabicLawrence)** ⬆️ 11 _(2022-12-04 13:02:26)_

	For scraping: [requests-html](https://requests.readthedocs.io/projects/requests-html/en/latest/)

	* 🟨 **[sohang-3112](https://www.reddit.com/user/sohang-3112)** ⬆️ 6 _(2022-12-04 16:03:32)_

		What does this library offer over a combination of `requests` and `BeautifulSoup` libraries?

		* 🟧 **[benefit_of_mrkite](https://www.reddit.com/user/benefit_of_mrkite)** ⬆️ 3 _(2022-12-04 17:33:24)_

			Very simple to use and JavaScript support.  I’ve done some amazing projects with it

		* 🟧 **[ArabicLawrence](https://www.reddit.com/user/ArabicLawrence)** ⬆️ 5 _(2022-12-04 16:04:10)_

			Javascript rendering to scrape dynamic pages!

			* 🟦 **[sohang-3112](https://www.reddit.com/user/sohang-3112)** ⬆️ 3 _(2022-12-04 18:37:00)_

				So basically like Selenium with a headless browser?

				* 🟪 **[ArabicLawrence](https://www.reddit.com/user/ArabicLawrence)** ⬆️ 1 _(2022-12-04 18:41:51)_

					Yes, but it also auto-installs chromium and you don’t need to specify its installation path. Very nice if you are as noob as I was when I started.

		* 🟧 **[shawncaza](https://www.reddit.com/user/shawncaza)** ⬆️ 2 _(2022-12-04 17:20:16)_

			I like `scrapy` for scraping in most scenarios. To be honest I haven't tried BeautifulSoup as I haven't had a purpose for it. My impression as a beautifulsoup outsider is that Scrapy is purpose built with tools for organizing crawling/scraping projects in an efficient scale-able way that I don't think Beautifulsoup offers.

* 🟩 **[Legitimate_Hat_7852](https://www.reddit.com/user/Legitimate_Hat_7852)** ⬆️ 13 _(2022-12-04 09:43:05)_

	Only just starting out on my Python journey but Panda looks really useful

	* 🟨 **[Dasher38](https://www.reddit.com/user/Dasher38)** ⬆️ 6 _(2022-12-04 17:33:27)_

		You should also have a look at polars. The API is a lot more consistent. Pandas is full of weirdness, inconsistencies and keeps adding new cruft and deprecated other cruft. On top of that it's not so fast in the end, especially if interop is needed with anything else (and it is, as pandas does not have any native storage. The arrow/parquet ecosystem is a lot better and learnt from the mistakes of pandas)

	* 🟨 **[TheAJGman](https://www.reddit.com/user/TheAJGman)** ⬆️ 4 _(2022-12-04 14:59:49)_

		If you're starting out learn Pydantic. It's basically dataclasses with some validation and cool shit bolted on.

		* 🟧 **[twd000](https://www.reddit.com/user/twd000)** ⬆️ 3 _(2022-12-04 15:10:02)_

			Instead of pandas, or in addition to it?

			* 🟦 **[TheAJGman](https://www.reddit.com/user/TheAJGman)** ⬆️ 10 _(2022-12-04 15:24:10)_

				In addition. Pandas is mostly data manipulation while Pydantic is useful for custom datatype/datasets. It's ideal for replacing Dicts/NamedTuples or supplementing existing dataclasses and has strong typing and validation support.

* 🟩 **[ultraDross](https://www.reddit.com/user/ultraDross)** ⬆️ 3 _(2022-12-04 11:20:15)_

	pdbpp and remote-pdb

	That make terminal based debugging a little bit easier.

	* 🟨 **[sohang-3112](https://www.reddit.com/user/sohang-3112)** ⬆️ 1 _(2022-12-04 16:49:17)_

		> pdbpp and remote-pdb
		
		As I haven't used either of these, could you please explain the difference between them? Or are they meant to be used together?

		* 🟧 **[ultraDross](https://www.reddit.com/user/ultraDross)** ⬆️ 4 _(2022-12-04 19:49:40)_

			pdbpp enhances pdb; colour output more commands etc.
			
			Remote-pdb allows you to use pdb on remote servers. This is especially handy if you develop against a docker container as it allows you to debug within it easily.

* 🟩 **[sndwch](https://www.reddit.com/user/sndwch)** ⬆️ 6 _(2022-12-04 15:46:07)_

	I never see or hear much about [snoop](https://pypi.org/project/snoop/) but I use it constantly when I can’t be bothered to debug properly.

* 🟩 **[opossum787](https://www.reddit.com/user/opossum787)** ⬆️ 4 _(2022-12-04 19:14:48)_

	python-pptx. I build lots of data presentations at work, and it's made it super simple to swap client data in and out.

* 🟩 **[rainnz](https://www.reddit.com/user/rainnz)** ⬆️ 4 _(2022-12-04 19:28:31)_

	[polars](https://www.pola.rs) as a replacement for pandas

	[playwright-python](https://pypi.org/project/playwright/) as a replacement for Selenium

* 🟩 **[showtime087](https://www.reddit.com/user/showtime087)** ⬆️ 4 _(2022-12-04 20:09:56)_

	Xarray—when you have N dimensional data, need numpy-like performance, but need to align things properly. Interfaces seamlessly with pandas and standard visualization libraries.

* 🟩 **[ohkwarig](https://www.reddit.com/user/ohkwarig)** ⬆️ 3 _(2022-12-05 01:27:49)_

	I enjoy pysimplegui https://www.pysimplegui.org/en/latest/ so I don't have to mess with tkinter. It also gives you flexibility to switch to a web interface or even QT

* 🟩 **[ecapoferri](https://www.reddit.com/user/ecapoferri)** ⬆️ 8 _(2022-12-04 18:14:34)_

	This thread is great. Thanks to all the contributors. This is exactly why I subscribe to this sub. You should repost on r/learnpython.

* 🟩 **[shinitakunai](https://www.reddit.com/user/shinitakunai)** ⬆️ 3 _(2022-12-04 10:31:21)_

	Requests and mwclient for documentation

* 🟩 **[NoProfessor2268](https://www.reddit.com/user/NoProfessor2268)** ⬆️ 3 _(2022-12-04 11:56:18)_

	I wanted to work with my calendar and tried a few libraries but all raised errors on my huge Google calendar. So I decided to write one myself; [iCal-library](https://jorricks.github.io/iCal-library/). All calendar projects I did since have been super easy.

* 🟩 **[DrNASApants](https://www.reddit.com/user/DrNASApants)** ⬆️ 3 _(2022-12-04 16:06:44)_

	Pandas, GeoPandas and Rasterio basically transformed my field. But they would be nothing without GDAL

	* 🟨 **[deleted]** ⬆️ 1 _(2022-12-04 17:14:58)_

		Folium ftw

		* 🟧 **[DrNASApants](https://www.reddit.com/user/DrNASApants)** ⬆️ 1 _(2022-12-04 17:17:22)_

			🙌

* 🟩 **[Texas1911](https://www.reddit.com/user/Texas1911)** ⬆️ 3 _(2022-12-05 00:32:27)_

	I’ll take “3rd party apps that I love but know will shelved and unsupported at an inopportune time” for $500, Alex.

* 🟩 **[deleted]** ⬆️ 2 _(2022-12-04 17:32:02)_

	[convtools](https://github.com/westandskif/convtools) - I built this to generate ad-hoc data converters, but now what I like the most about it is the functional approach.

* 🟩 **[blademaster2005](https://www.reddit.com/user/blademaster2005)** ⬆️ 2 _(2022-12-04 18:13:37)_

	Hammock

	It's a dot chain rest uri builder for requests.

	It makes working with api's that don't have their own libraries so much easier

* 🟩 **[Present_Reaction8625](https://www.reddit.com/user/Present_Reaction8625)** ⬆️ 2 _(2022-12-04 21:12:46)_

	I do love to use pendulum but the last update was in 2020 and arrow essentially has everything and more than what pendulum offers at the moment

* 🟩 **[i_kant_spal](https://www.reddit.com/user/i_kant_spal)** ⬆️ 2 _(2022-12-04 21:31:42)_

	*parameterize* for easier unit testing with a bunch if different inputs.

	*parameterize.expand* allows automatically generating a new method for each input, while storing all inputs in a single variable. That makes it possible to test each case even if one (or more) of them fail and avoid using loops within test methods.

	* 🟨 **[Sillocan](https://www.reddit.com/user/Sillocan)** ⬆️ 4 _(2022-12-04 22:16:33)_

		Pytest has this built in, so this is a good alternative if you're using `unittest`

* 🟩 **[vorticalbox](https://www.reddit.com/user/vorticalbox)** ⬆️ 2 _(2022-12-04 22:14:59)_

	For me it was pipe https://pypi.org/project/pipe/

* 🟩 **[AndydeCleyre](https://www.reddit.com/user/AndydeCleyre)** ⬆️ 2 _(2022-12-04 23:31:31)_

	I've said many times before and I'll say it again: [plumbum](https://plumbum.readthedocs.io/en/latest/) is excellent and under-appreciated.

	* 🟨 **[alcalde](https://www.reddit.com/user/alcalde)** ⬆️ 1 _(2022-12-05 04:30:19)_

		I prefer its inverse, [xonsh](https://xon.sh/).

* 🟩 **[Viking_wang](https://www.reddit.com/user/Viking_wang)** ⬆️ 2 _(2022-12-04 23:33:18)_

	Surprised no one mentioned attrs yet.

	Dataclasses but so much better.

	I barely find my self writing a class that is not attrs and usually if i do, i change my mind after 20 minutes.

	We even pushed it into our coding standards. Unless there is a good reason why you cant use it (e.g. not a data class) you should use it.

	* 🟨 **[mr_cesar](https://www.reddit.com/user/mr_cesar)** ⬆️ 1 _(2022-12-05 00:44:43)_

		Same here.
		
		It seems to me people are more familiar with pydantic than with attrs.

* 🟩 **[its_dann](https://www.reddit.com/user/its_dann)** ⬆️ 2 _(2022-12-04 23:51:18)_

	Trafilatura it scrapes websites for their articles. Never have had an issue with it and instead of buildings scrapers I wrote 2 lines or code

* 🟩 **[deleted]** ⬆️ 2 _(2022-12-05 01:01:38)_

	nested_lookup was super useful to quickly search through different json web socket data to see if something existed at different nested levels. Library seemed a bit early / rough but worked for me!

* 🟩 **[Greenscarf_005](https://www.reddit.com/user/Greenscarf_005)** ⬆️ 2 _(2022-12-05 03:14:51)_

	[flupy](https://flupy.readthedocs.io/en/latest/), lets you use fluent interface, like

	```

	from flupy import flu

	result = (

	  flu(range(100))

	  .filter(lambda x: x &lt; 50)

	  .map(lambda x: x * 3)

	  .collect()

	)

	```

* 🟩 **[MilkyMilkerson](https://www.reddit.com/user/MilkyMilkerson)** ⬆️ 2 _(2022-12-05 00:14:21)_

	Beautiful Soup. Essential for web scraping.

	* 🟨 **[alcalde](https://www.reddit.com/user/alcalde)** ⬆️ 4 _(2022-12-05 04:27:29)_

		It's underrated?!?

* 🟩 **[vantasmer](https://www.reddit.com/user/vantasmer)** ⬆️ 1 _(2022-12-04 18:55:28)_

	Shout out to [python-o365](https://github.com/O365/python-o365) and [circuit-maintenance-parser](https://github.com/networktocode/circuit-maintenance-parser).  

	Narrow scopes but solve some difficult problems.

* 🟩 **[Inconsistent-n-Aloof](https://www.reddit.com/user/Inconsistent-n-Aloof)** ⬆️ 1 _(2022-12-04 15:23:24)_

	Pandas has been very useful in my case.

	* 🟨 **[sohang-3112](https://www.reddit.com/user/sohang-3112)** ⬆️ 2 _(2022-12-04 16:51:47)_

		It's one of the most popular Python libraries ever - definitely not underrated!

* 🟩 **[D-K-BO](https://www.reddit.com/user/D-K-BO)** ⬆️ 1 _(2022-12-04 18:22:03)_

	[sorcery](https://pypi.org/project/sorcery/) uses dark magic to allow things like

	    dict_of(foo, bar, spam=thing())

	instead of

	    dict(foo=foo, bar=bar, spam=thing())

* 🟩 **[QultrosSanhattan](https://www.reddit.com/user/QultrosSanhattan)** ⬆️ 1 _(2022-12-04 19:59:49)_

	def pygame.

	With proper math you can display almost everything on the screen.

* 🟩 **[Dubanons](https://www.reddit.com/user/Dubanons)** ⬆️ 0 _(2022-12-05 04:16:06)_

	REMOVED DUE TO CUSTOM FILTER(S)

* 🟩 **[dmart89](https://www.reddit.com/user/dmart89)** ⬆️ 1 _(2022-12-04 12:25:20)_

	Beanie - mongoDB ODM

* 🟩 **[smile_politely](https://www.reddit.com/user/smile_politely)** ⬆️ 1 _(2022-12-04 15:55:22)_

	A lot of interesting answers! Looks like pydantic is some of the favorites.

* 🟩 **[Cockroach-777](https://www.reddit.com/user/Cockroach-777)** ⬆️ 1 _(2022-12-04 18:47:05)_

	Selenium and webdriver_wait are my favourite modules through which I can automate browsing and scape data using CSS tags

* 🟩 **[ZeroSilence1](https://www.reddit.com/user/ZeroSilence1)** ⬆️ 1 _(2022-12-04 19:17:57)_

	Pyinputplus looks excellent, thanks! I just wrote a bunch of functions to for input validation lol. This will make it a lot easier.

	Python is about continually finding ways to do something with less and less code.

* 🟩 **[spidLL](https://www.reddit.com/user/spidLL)** ⬆️ 1 _(2022-12-04 19:21:28)_

	I need to save this post, I discovered so many interesting modules &lt;3

* 🟩 **[dashdanw](https://www.reddit.com/user/dashdanw)** ⬆️ 1 _(2022-12-04 19:48:08)_

	‘click’ makes sexy cli utilities

* 🟩 **[Sensitive-Ad9351](https://www.reddit.com/user/Sensitive-Ad9351)** ⬆️ 1 _(2022-12-04 20:33:34)_

	If you’re trying to write a programming / configuration language, Lark is really nice. You can basically just write bnf notation for a language and it gives you a parser.

* 🟩 **[jmakov](https://www.reddit.com/user/jmakov)** ⬆️ 1 _(2022-12-04 21:08:50)_

	ray.io, multi and distributed processing. Should be in the standard lib IMO.

* 🟩 **[metaldark](https://www.reddit.com/user/metaldark)** ⬆️ 1 _(2022-12-04 21:42:32)_

	Requests but I’m sure it’s not underrated.

* 🟩 **[pedrobis](https://www.reddit.com/user/pedrobis)** ⬆️ 1 _(2022-12-04 23:08:19)_

	Pyteserract to make ocr

* 🟩 **[pkkid](https://www.reddit.com/user/pkkid)** ⬆️ 1 _(2022-12-04 23:58:50)_

	*requests_cache* - Drop it in a long side requests and it makes development against rest apis so much faster and easier.

* 🟩 **[mattkatzbaby](https://www.reddit.com/user/mattkatzbaby)** ⬆️ 1 _(2022-12-05 00:10:48)_

	Two that I haven’t seen here and have saved me tons of time are [pudb](https://documen.tician.de/pudb/), a great debugger and [petl](https://petl.readthedocs.io/en/stable/) a simple powerful ETL toolkit. 

	Both do things you can do with other tools but are a damn pleasure to use.

* 🟩 **[vladusatii](https://www.reddit.com/user/vladusatii)** ⬆️ 1 _(2022-12-05 01:54:07)_

	DBM!!! It made database scheming so much faster. And it’s really fast.

* 🟩 **[gravity_rose](https://www.reddit.com/user/gravity_rose)** ⬆️ 1 _(2022-12-05 02:26:59)_

	[typer](https://typer.tiangolo.com/) \- 

	Makes command line interfaces from function definitions and type hints.  No more argparse, or other BS.  Make sophisticated interfaces easy.  Plus includes pretty-printed stack traces on dump (with locals).

* 🟩 **[putneyj](https://www.reddit.com/user/putneyj)** ⬆️ 1 _(2022-12-05 02:50:59)_

	It’s a toss up between `tqdm` for progress bars while iterating (especially when doing multi-threaded iteration) or  `questionary` for getting specific input from a user from the command line.

* 🟩 **[c_alash](https://www.reddit.com/user/c_alash)** ⬆️ 1 _(2022-12-05 05:26:31)_

	Ipdb allows you to run a debugger in collab. Usefull af

* 🟩 **[calihunlax](https://www.reddit.com/user/calihunlax)** ⬆️ 1 _(2022-12-05 14:55:11)_

	**[Markdown](https://pypi.org/project/Markdown/)** converts Markdown markup into HTML, with extensions for code highlighting, table of contents, etc.

* 🟩 **[TornadoPro2712](https://www.reddit.com/user/TornadoPro2712)** ⬆️ 1 _(2022-12-05 17:52:17)_

	pygame is my fav

* 🟩 **[okazdal](https://www.reddit.com/user/okazdal)** ⬆️ 1 _(2022-12-17 08:34:12)_

	[Redbird](https://red-bird.readthedocs.io/en/latest/)

	Repository pattern is a technique to abstract the data access from the domain/business logic. In other words, it decouples the database access from the application code. The aim is that the code runs the same regardless if the data is stored to an SQL database, NoSQL database, file or even as an in-memory list.

* 🟩 **[WoodenNichols](https://www.reddit.com/user/WoodenNichols)** ⬆️ 1 _(2023-03-03 17:23:41)_

	pyinputplus is indeed a good one, but my favorite is arrow (the improved datetime one).
