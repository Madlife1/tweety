.. _filter:

===============
Search Filters
===============

You can filter the `Search` function using these methods


Filter Latest Tweets
---------------------

.. py:class:: SearchFilters.Latest()

    :reference: `tweety.filters.SearchFilters.Latest`

    .. code-block:: python

        from tweety.filters import SearchFilters

        # Assuming `app` is Twitter Client Object

        app.search("#pakistan", filter_=SearchFilters.Latest())
        from tweet in tweets:
            print(tweet)

Filter Only Media Tweets
---------------------------

.. py:class:: SearchFilters.Media()

    :reference: `tweety.filters.SearchFilters.Media`

    .. code-block:: python

        from tweety.filters import SearchFilters

        # Assuming `app` is Twitter Client Object

        app.search("#pakistan", filter_=SearchFilters.Media())
        from tweet in tweets:
            print(tweet.media)


Filter Only Users
---------------------

.. py:class:: SearchFilters.Users()

    :reference: `tweety.filters.SearchFilters.Users`

    .. code-block:: python

        from tweety.filters import SearchFilters

        # Assuming `app` is Twitter Client Object

        app.search("#pakistan", filter_=SearchFilters.Users())
        from user in users:
            print(user)



===============
Tweet Audience Filter
===============

You can filter the created Tweet Comment Audience function using these methods


Filter Only People You Mention
--------------------------------

.. py:class:: TweetConversationFilters.PeopleYouMention()

    :reference: `tweety.filters.TweetConversationFilters.PeopleYouMention`

    .. code-block:: python

        from tweety.filters import TweetConversationFilters

        # Assuming `app` is Twitter Client Object

        app.create_tweet("Hi", filter_=TweetConversationFilters.PeopleYouMention())


Filter Only People You Follow
--------------------------------

.. py:class:: TweetConversationFilters.PeopleYouFollow()

    :reference: `tweety.filters.TweetConversationFilters.PeopleYouFollow`

    .. code-block:: python

        from tweety.filters import TweetConversationFilters

        # Assuming `app` is Twitter Client Object

        app.create_tweet("Hi", filter_=TweetConversationFilters.PeopleYouFollow())
