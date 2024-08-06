```bash
                               cntrb_id                created_at  month  year  repo_id repo_name       login             action  rank  yearmonth  new_contributors    quarter    type  differences
5   010000c3-bd00-0000-0000-000000000000 2023-02-24 02:45:37+00:00      2  2023        1     augur     gliptak  open_pull_request     1 2023-02-01                 1 2023-01-01  repeat       139393
69  01006530-0700-0000-0000-000000000000 2023-05-24 17:28:24+00:00      5  2023        1     augur      Seltyk  open_pull_request     1 2023-05-01                 1 2023-04-01  repeat      4065003
75  010074e2-4e00-0000-0000-000000000000 2024-02-06 15:22:16+00:00      2  2024        1     augur  GaryPWhite  open_pull_request     1 2024-02-01                 1 2024-01-01  repeat       781490
2024-08-06 13:36:05 agentk augur.api.server[83963] ERROR Exception on /api/unstable/contributor_reports/returning_contributors_pie_chart/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/contributor_reports.py", line 1036, in returning_contributors_pie_chart
    p = figure(plot_height=450, plot_width=plot_width, title=title,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_height' to figure, similar attributes are outer_height, height or min_height


2024-08-06 13:36:06 agentk augur.api.server[83964] ERROR Exception on /api/unstable/pull_request_reports/average_comments_per_PR/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 672, in average_comments_per_PR
    p = figure(y_range=y_groups, plot_height=450, plot_width=plot_width,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_height' to figure, similar attributes are outer_height, height or min_height
2024-08-06 13:36:06 agentk augur.api.server[83957] ERROR Exception on /api/unstable/contributor_reports/new_contributors_bar/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/contributor_reports.py", line 735, in new_contributors_bar
    p = figure(x_range=data['dates'], plot_height=400, plot_width=plot_width,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_height' to figure, similar attributes are outer_height, height or min_height
2024-08-06 13:36:06 agentk augur.api.server[83958] ERROR Exception on /api/unstable/contributor_reports/returning_contributors_stacked_bar/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/contributor_reports.py", line 1212, in returning_contributors_stacked_bar
    p = figure(x_range=data['dates'], plot_height=500, plot_width=plot_width,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_height' to figure, similar attributes are outer_height, height or min_height
     dates  open_pull_request  pull_request_comment  commit  issue_closed  issue_opened  issue_comment
0  2023-01                6.0                   0.0     0.0           1.0           0.0            0.0
1  2023-04                3.0                   0.0     0.0           1.0           0.0            0.0
2  2023-07                9.0                   0.0     0.0           0.0           0.0            0.0
3  2023-10                3.0                   0.0     0.0           0.0           0.0            0.0
4  2024-01                2.0                   0.0     0.0           0.0           0.0            0.0
5  2024-04                1.0                   0.0     0.0           1.0           0.0            0.0
6  2024-07                0.0                   0.0     0.0           1.0           0.0            0.0
2024-08-06 13:36:06 agentk augur.api.server[83961] ERROR Exception on /api/unstable/contributor_reports/new_contributors_stacked_bar/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/contributor_reports.py", line 935, in new_contributors_stacked_bar
    p = figure(x_range=data['dates'], plot_height=400, plot_width=plot_width,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute '  ' to figure, similar attributes are outer_height, height or min_height
2024-08-06 13:36:07 agentk augur.api.server[83964] ERROR Exception on /api/unstable/pull_request_reports/mean_response_times_for_PR/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 1033, in mean_response_times_for_PR
    p = figure(toolbar_location=None, y_range=sorted(driver_df[y_axis].unique()), plot_width=plot_width,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_width' to figure, similar attributes are outer_width, width or min_width
2024-08-06 13:36:07 agentk augur.api.server[83963] ERROR Exception on /api/unstable/pull_request_reports/PR_counts_by_merged_status/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 860, in PR_counts_by_merged_status
    p = figure(x_range=x_groups, plot_height=350, plot_width=plot_width,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_height' to figure, similar attributes are outer_height, height or min_height
[2024-08-06 13:36:08,013: ERROR/MainProcess] consumer: Cannot connect to amqp://augur:**@rabbitmq:5672/augur_vhost: [Errno 8] nodename nor servname provided, or not known.
Trying again in 4.00 seconds... (2/100)

2024-08-06 13:36:08 agentk augur.api.server[83958] ERROR Exception on /api/unstable/pull_request_reports/mean_days_between_PR_comments/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 1319, in mean_days_between_PR_comments
    pr_closed = filter_data(pr_closed, pr_closed_needed_columns)
                ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 427, in filter_data
    df = get_needed_columns(df, needed_columns)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 402, in get_needed_columns
    return df[list_of_columns]
           ~~^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/pandas/core/frame.py", line 3813, in __getitem__
    indexer = self.columns._get_indexer_strict(key, "columns")[1]
              ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/pandas/core/indexes/base.py", line 6070, in _get_indexer_strict
    self._raise_if_missing(keyarr, indexer, axis_name)
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/pandas/core/indexes/base.py", line 6133, in _raise_if_missing
    raise KeyError(f"{not_found} not in index")
KeyError: "['average_time_between_responses'] not in index"
[2024-08-06 13:36:08,202: ERROR/MainProcess] consumer: Cannot connect to amqp://augur:**@rabbitmq:5672/augur_vhost: [Errno 8] nodename nor servname provided, or not known.
Trying again in 4.00 seconds... (2/100)

2024-08-06 13:36:08 agentk augur.api.server[83957] ERROR Exception on /api/unstable/pull_request_reports/average_commits_per_PR/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 560, in average_commits_per_PR
    p = figure(x_range=FactorRange(*x), plot_height=450, plot_width=plot_width, title=title,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_height' to figure, similar attributes are outer_height, height or min_height
2024-08-06 13:36:08 agentk augur.api.server[83961] ERROR Exception on /api/unstable/pull_request_reports/PR_time_to_first_response/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 1506, in PR_time_to_first_response
    p = figure(x_range=(
        ^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_width' to figure, similar attributes are outer_width, width or min_width
2024-08-06 13:36:08 agentk augur.api.server[83963] ERROR Exception on /api/unstable/pull_request_reports/Average_PR_duration/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 1851, in Average_PR_duration
    p = figure(plot_width=plot_width, plot_height=300,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_width' to figure, similar attributes are outer_width, width or min_width
[2024-08-06 13:36:08,762: ERROR/MainProcess] consumer: Cannot connect to amqp://augur:**@rabbitmq:5672/augur_vhost: [Errno 8] nodename nor servname provided, or not known.
Trying again in 2.00 seconds... (1/100)

2024-08-06 13:36:08 agentk augur.api.server[83964] ERROR Exception on /api/unstable/pull_request_reports/average_PR_events_for_closed_PRs/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 1690, in average_PR_events_for_closed_PRs
    p = figure(y_range=y_groups, plot_height=500, plot_width=plot_width, x_range=x_groups,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_height' to figure, similar attributes are outer_height, height or min_height
```


## After Changing code
```bash
2024-08-06 13:48:10 agentk augur[95823] INFO Starting facade worker processes with concurrency=15
                                cntrb_id                created_at  month  year  repo_id repo_name       login             action  rank  yearmonth  new_contributors    quarter    type  differences
5   010000c3-bd00-0000-0000-000000000000 2023-02-24 02:45:37+00:00      2  2023        1     augur     gliptak  open_pull_request     1 2023-02-01                 1 2023-01-01  repeat       139393
69  01006530-0700-0000-0000-000000000000 2023-05-24 17:28:24+00:00      5  2023        1     augur      Seltyk  open_pull_request     1 2023-05-01                 1 2023-04-01  repeat      4065003
75  010074e2-4e00-0000-0000-000000000000 2024-02-06 15:22:16+00:00      2  2024        1     augur  GaryPWhite  open_pull_request     1 2024-02-01                 1 2024-01-01  repeat       781490
2024-08-06 13:48:21 agentk augur.api.server[96225] ERROR Exception on /api/unstable/contributor_reports/returning_contributors_pie_chart/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/contributor_reports.py", line 1036, in returning_contributors_pie_chart
    p = figure(height=450, plot_width=plot_width, title=title,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_width' to figure, similar attributes are outer_width, width or min_width
2024-08-06 13:48:21 agentk augur.api.server[96220] ERROR Exception on /api/unstable/pull_request_reports/average_commits_per_PR/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 560, in average_commits_per_PR
    p = figure(x_range=FactorRange(*x), height=450, plot_width=plot_width, title=title,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_width' to figure, similar attributes are outer_width, width or min_width
2024-08-06 13:48:21 agentk augur.api.server[96221] ERROR Exception on /api/unstable/contributor_reports/returning_contributors_stacked_bar/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/contributor_reports.py", line 1212, in returning_contributors_stacked_bar
    p = figure(x_range=data['dates'], height=500, plot_width=plot_width,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_width' to figure, similar attributes are outer_width, width or min_width
2024-08-06 13:48:21 agentk augur.api.server[96222] ERROR Exception on /api/unstable/contributor_reports/new_contributors_bar/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/contributor_reports.py", line 735, in new_contributors_bar
    p = figure(x_range=data['dates'], height=400, plot_width=plot_width,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_width' to figure, similar attributes are outer_width, width or min_width
     dates  open_pull_request  pull_request_comment  commit  issue_closed  issue_opened  issue_comment
0  2023-01                6.0                   0.0     0.0           1.0           0.0            0.0
1  2023-04                3.0                   0.0     0.0           1.0           0.0            0.0
2  2023-07                9.0                   0.0     0.0           0.0           0.0            0.0
3  2023-10                3.0                   0.0     0.0           0.0           0.0            0.0
4  2024-01                2.0                   0.0     0.0           0.0           0.0            0.0
5  2024-04                1.0                   0.0     0.0           1.0           0.0            0.0
6  2024-07                0.0                   0.0     0.0           1.0           0.0            0.0
2024-08-06 13:48:21 agentk augur.api.server[96223] ERROR Exception on /api/unstable/contributor_reports/new_contributors_stacked_bar/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/contributor_reports.py", line 935, in new_contributors_stacked_bar
    p = figure(x_range=data['dates'], height=400, plot_width=plot_width,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_width' to figure, similar attributes are outer_width, width or min_width
2024-08-06 13:48:22 agentk augur.api.server[96220] ERROR Exception on /api/unstable/pull_request_reports/average_comments_per_PR/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 672, in average_comments_per_PR
    p = figure(y_range=y_groups, height=450, plot_width=plot_width,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_width' to figure, similar attributes are outer_width, width or min_width
2024-08-06 13:48:22 agentk augur.api.server[96225] ERROR Exception on /api/unstable/pull_request_reports/PR_counts_by_merged_status/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 860, in PR_counts_by_merged_status
    p = figure(x_range=x_groups, height=350, plot_width=plot_width,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_width' to figure, similar attributes are outer_width, width or min_width
2024-08-06 13:48:22 agentk augur.api.server[96221] ERROR Exception on /api/unstable/pull_request_reports/mean_response_times_for_PR/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 1033, in mean_response_times_for_PR
    p = figure(toolbar_location=None, y_range=sorted(driver_df[y_axis].unique()), plot_width=plot_width,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_width' to figure, similar attributes are outer_width, width or min_width
2024-08-06 13:48:22 agentk augur.api.server[96222] ERROR Exception on /api/unstable/pull_request_reports/mean_days_between_PR_comments/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 1319, in mean_days_between_PR_comments
    pr_closed = filter_data(pr_closed, pr_closed_needed_columns)
                ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 427, in filter_data
    df = get_needed_columns(df, needed_columns)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 402, in get_needed_columns
    return df[list_of_columns]
           ~~^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/pandas/core/frame.py", line 3813, in __getitem__
    indexer = self.columns._get_indexer_strict(key, "columns")[1]
              ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/pandas/core/indexes/base.py", line 6070, in _get_indexer_strict
    self._raise_if_missing(keyarr, indexer, axis_name)
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/pandas/core/indexes/base.py", line 6133, in _raise_if_missing
    raise KeyError(f"{not_found} not in index")
KeyError: "['average_time_between_responses'] not in index"
2024-08-06 13:48:23 agentk augur.api.server[96223] ERROR Exception on /api/unstable/pull_request_reports/PR_time_to_first_response/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 1506, in PR_time_to_first_response
    p = figure(x_range=(
        ^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_width' to figure, similar attributes are outer_width, width or min_width
2024-08-06 13:48:23 agentk augur.api.server[96220] ERROR Exception on /api/unstable/pull_request_reports/average_PR_events_for_closed_PRs/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 1690, in average_PR_events_for_closed_PRs
    p = figure(y_range=y_groups, height=500, plot_width=plot_width, x_range=x_groups,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_width' to figure, similar attributes are outer_width, width or min_width
/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/xgboost/compat.py:31: FutureWarning: pandas.Int64Index is deprecated and will be removed from pandas in a future version. Use pandas.Index with the appropriate dtype instead.
  from pandas import MultiIndex, Int64Index
/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/xgboost/compat.py:31: FutureWarning: pandas.Int64Index is deprecated and will be removed from pandas in a future version. Use pandas.Index with the appropriate dtype instead.
  from pandas import MultiIndex, Int64Index
/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/xgboost/compat.py:31: FutureWarning: pandas.Int64Index is deprecated and will be removed from pandas in a future version. Use pandas.Index with the appropriate dtype instead.
  from pandas import MultiIndex, Int64Index
/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/xgboost/compat.py:31: FutureWarning: pandas.Int64Index is deprecated and will be removed from pandas in a future version. Use pandas.Index with the appropriate dtype instead.
  from pandas import MultiIndex, Int64Index
/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/xgboost/compat.py:31: FutureWarning: pandas.Int64Index is deprecated and will be removed from pandas in a future version. Use pandas.Index with the appropriate dtype instead.
  from pandas import MultiIndex, Int64Index
2024-08-06 13:48:23 agentk augur.api.server[96225] ERROR Exception on /api/unstable/pull_request_reports/Average_PR_duration/ [GET]
Traceback (most recent call last):
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 2073, in wsgi_app
    response = self.full_dispatch_request()
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1518, in full_dispatch_request
    rv = self.handle_user_exception(e)
         ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask_cors/extension.py", line 178, in wrapped_function
    return cors_after_request(app.make_response(f(*args, **kwargs)))
                                                ^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1516, in full_dispatch_request
    rv = self.dispatch_request()
         ^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/flask/app.py", line 1502, in dispatch_request
    return self.ensure_sync(self.view_functions[rule.endpoint])(**req.view_args)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/chaoss/augur/augur/api/routes/pull_request_reports.py", line 1851, in Average_PR_duration
    p = figure(plot_width=plot_width, height=300,
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/plotting/_figure.py", line 196, in __init__
    self._raise_attribute_error_with_matches(name, names | opts.properties())
  File "/Users/sean/github/virtualenvs/augur-test/lib/python3.11/site-packages/bokeh/core/has_props.py", line 377, in _raise_attribute_error_with_matches
    raise AttributeError(f"unexpected attribute {name!r} to {self.__class__.__name__}, {text} attributes are {nice_join(matches)}")
AttributeError: unexpected attribute 'plot_width' to figure, similar attributes are outer_width, width or min_width
```