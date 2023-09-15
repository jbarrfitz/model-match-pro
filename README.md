# Model-Match-Pro

## A Full-Stack 3-Tier Web App by

- Deiosha Sparks: [Github](https://github.com/Deiosha), [LinkedIn](https://linkedin.com/in/deiosha-sparks-954882251/)
- Jerry Barrows-Fitzgerald: [Github](https://github.com/jbarrfitz), [LinkedIn](https://linkedin.com/in/jbarrowsfitzgerald/)
- Lauren Main: [Github](https://github.com/elleem), [LinkedIn](https://linkedin.com/in/laurenmain28/)
- Manuch Sadri: [Github](https://github.com/mcsadri), [LinkedIn](https://linkedin.com/in/manuch-sadri/)

## Overview

- What is the vision of this product?
  - Model-Match-Pro enables its users to submit a single Large Language Model (LLM) prompt and then simltaneously compare the responses from multiple models to find which one(s) best match their use case.
- What pain point does this project solve?
  - With the recent proliferation of Large Language Models, many users pick their favorite and then try to engineer their prompts to work for their use case. Currently, there are very few, if any, applications that allow users to simltaneously compare results from multiple LLMs. Oftentimes, LLM users must test each LLM individually, and attempt to compare the responses through inefficient means.
- Why should we care about your product?
  - Model-Match-Pro will be one of the few products providing a method to compare the results from multiple LLMs within the same web browser tab using a single prompt submission.

## Links

- [Model Match Pro](https://model-match-fe.vercel.app/search)

## Set-up

- In terminal (assumes git, python3.11, and npm are previously installed):
  - Clone repo from GitHub:
    - $ ```git clone https://github.com/Match-Makers/model-match-pro.git```

### Backend

#### Backend Set-up

- Change directory to the backend folder in the cloned local repo:
  - $ ```cd model-match-pro/backend```
- Create & run virtual environment:
  - $ ```python3.11 -m venv .venv```
  - $ ```source .venv/bin/activate```
- Install requirements:
  - $ ```npm install -r requirements.txt```
- Get secrets from project team for `/model-match-pro/backend/model_match_proj/.env`.
- Start dev server:
- $ ```python manage.py runserver```
- In browser (to run locally):
  - Django REST Framework default web pages:
    - http://localhost:8000/ - home
    - http://localhost:8000/admin/ - admin panel
    - http://localhost:8000/api/v1/model_match_app

#### Backend Tests

- Open new terminal window or tab.
- Change directory to the backend folder in the cloned local repo:
  - $ ```cd model-match-pro/backend```
- Create & run virtual environment:
  - $ ```source .venv/bin/activate```
- Run tests:
  - $ ```python manage.py test model_match_app.tests```
- Run coverage.py:
  - $ ```coverage run --source=model_match_app manage.py test model_match_app.tests```
- To generate the coverage report:
  - $ ```coverage report```

### Frontend

#### Frontend Set-up

- Open new terminal window or tab.
- Change directory to the frontend folder in the cloned local repo:
  - $ ```cd model-match-pro/frontend```
- Install all the dependencies:
  - $ ```npm install```
- Get secrets from project team for `/model-match-pro/frontend/.env`.
- Run local environment:
  - $ ```npm run dev```
- In browser (to run locally):
  - http://localhost:3000

#### Frontend Tests

- Open new terminal window or tab.
- Change directory to the frontend folder in the cloned local repo:
  - $ ```cd model-match-pro/frontend```
- Run Playwright tests:
  - With new user registration:
    - $ ```node ./tests/pw-new-user.js```
  - With existing user:
    - $ ```node ./tests/pw-existing-user.js```
