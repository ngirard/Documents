---
Original post: "https://www.reddit.com/r/Python/comments/zc3mvf/what_is_your_favorite_most_underrated_3rd_party"
---

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
