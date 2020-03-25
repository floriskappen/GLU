# Pollster App (Django Crash Course)

> Python Django app to create polls with questions/choices

## Quick Start

``` bash
# Install dependencies
pipenv install

```bash
# Create Venv
pipenv shell
```
cd pollster

```bash
# Run initial migrations
python manage.py migrate
```

```bash
# Using the shell
python manage.py shell

>>>  from polls.models import Question, Choice
>>>  from django.utils import timezone
>>>  Question.objects.all()
>>>  q = Question(question_text="What is your favorite Python Framework?", pub_date=timezone.now())
>>>  q.save()
>>>  q.id
>>>  q.question_text
>>>  Question.objects.all()
>>>  Question.objects.filter(id=1)
>>>  Question.objects.get(pk=1)
>>>  q = Question.objects.get(pk=1)
>>>  q.choice_set.all()
>>>  q.choice_set.create(choice_text='Django', votes=0)
>>>  q.choice_set.create(choice_text='Flask', votes=0)
>>>  q.choice_set.create(choice_text='Flask', votes=0)
>>>  q.choice_set.all()
>>>  quit()
```

```bash
# Serve on localhost:8000
python manage.py runserver
```

