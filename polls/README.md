# polls

`polls` is a Django app to conduct web-based voting via polls.

## quick start

- Add "polls" to your project's `INSTALLED_APPS` in `settings.py`:

```python
INSTALLED_APPS = [
    # Other apps ...
    'polls'
]
```

- Also include its URLconf to `urlpatterns` in `urls.py`:

```python
path('polls/', include('polls.urls')),
```

- Run `python3 manage.py migrate` to create this package's models
- Enable the admin app and create new questions at http://127.0.0.1:8000/admin/
- https://docs.djangoproject.com/en/4.1/ref/contrib/admin/#overview
- Visit http://127.0.0.1:8000/polls/ to vote for the questions' choices.
